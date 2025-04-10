## Refined Chatbot Prompt

### Context

Hello ChatGPT,

A fresh day, a fresh start! I'm currently working on an Angular application and would like your assistance in refining and aligning the row selection behavior of my new grid component with that of the legacy implementation.

I’ve appended my Angular code to a component named `codeui`, and I’d like you to review it for context.

### Objective

The primary goal is to ensure that the following function:

```ts
onRowSelected(event: RowSelectedEvent): void {
  console.log('RowSelected:', event);
}
```

—which is triggered by the new grid's row selection event—effectively replicates the behavior of the following legacy method:

```ts
onRowSelect(row: any): void {
  if (this.selectedRow !== row && !this.controls.tableSelectMode) {
    this.selectedDocPDFViewer = '';
    this.selectedRow = row;

    // Ensure only one row is selected at a time
    this.tableRows.forEach(row => row.selected = false);

    this.loadCanvasImage(this.selectedRow);

    /* Reset the selected cell if only a row is selected 
       and not a specific cell within the row */
    if (this.selectedRow && !Object.values(this.selectedRow).includes(this.selectedCell)) {
      this.selectedCell = null;
    }
  }
}
```

This `onRowSelect` method is defined in the canvas component TypeScript file.

### Request

Please assist me in achieving the following:

1. Adapt the new grid’s `onRowSelected` function so that it invokes the behavior encapsulated in `onRowSelect`.
    
2. Ensure that selecting a row behaves identically to the legacy implementation, including image loading and single-row selection enforcement.
    
3. Guide me through the necessary steps to accomplish this, in a clear and structured manner.
    

Please proceed step by step.

Thank you!