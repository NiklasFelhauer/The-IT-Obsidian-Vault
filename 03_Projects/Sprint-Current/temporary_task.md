# Task Description: Enhancing the Symbol Text Save Endpoint

I am currently working on an important task that is critical to our processing pipeline. The task involves refining the logic of a specific API endpoint responsible for updating and saving symbol-text associations.

## Provided Files

Before proceeding, please review the following files to understand the relevant data structures and schema definitions:

- **`pid_api_part1.txt`**
- **`payload_to_be_saved.txt`**
- **`pid_schema.py`**  
- **`PIDModel_control_loop_two_instruments.json`**

These files provide essential context, especially regarding the expected structure of the `PIDSchema`.

## Objective

Enhance the `update_and_save` endpoint to handle symbol-text association files more intelligently.

### Endpoint to be Adjusted

```python
@app.post(
    "/pid-tasks/symbol-text-save/{file_name}",
    summary="Update and save symbol text association",
    description=(
        "Updates and saves the symbol text association for the given file name.\n\n"
        "**Note:** The uploaded Body must conform to the Pydantic `PIDSchema`.\n"
        "You can inspect the schema definition at the bottom of this documentation under **Schemas → PIDSchema**."
    ),
    tags=["Processing Utility"],
)
@handle_exceptions
async def update_and_save(
    request: Request,
    file_name: str = Path(..., description="The exact file name to update and save"),
    payload: PIDSchema = Body(...),
):
    xipidtenant = await getTenantID(request)
    return await update_manager.update_and_save(payload, file_name, xipidtenant)
```

## Functional Requirements

The `update_and_save` function must:

1. **Identify Payload Type**  
   Determine whether the incoming payload represents a symbol-text association file by checking for the presence of `symbols` and `words` arrays.

2. **Read the Existing File**  
   If it's a symbol-text association, open the corresponding file from storage, which shares the same `PIDSchema` structure as the payload.

3. **Perform Merging Logic**  
   - Iterate over the elements in the payload (`symbols`, `words`, etc.).
   - For each element:
     - **If the `id` already exists** in the corresponding array in the existing file, **overwrite** the element.
     - **If the `id` does not exist**, **append** the new element to the corresponding array.

4. **Example**

### Matching Element Update

**Incoming Payload:**
```json
{
  "id": "1160e4e3-4f46-4f88-9c98-f369902a7845",
  "text": "PICTest",
  "bbox": {
    "point1": [86, 271],
    "point2": [115, 287]
  },
  "confidence": 91,
  "rotation": 0,
  "state": "modified",
  "decision": "accepted"
}
```

**Storage Before:**
```json
{
  "id": "1160e4e3-4f46-4f88-9c98-f369902a7845",
  "text": "PIC",
  "bbox": {
    "point1": [86, 271],
    "point2": [115, 287]
  },
  "confidence": 91,
  "rotation": 0,
  "state": "recognized",
  "decision": "undecided"
}
```

**Storage After:**
```json
{
  "id": "1160e4e3-4f46-4f88-9c98-f369902a7845",
  "text": "PICTest",
  "bbox": {
    "point1": [86, 271],
    "point2": [115, 287]
  },
  "confidence": 91,
  "rotation": 0,
  "state": "modified",
  "decision": "accepted"
}
```

## Completion Criteria

If all updates are processed successfully, the system should return a success status code along with a confirmation message indicating a successful save.
