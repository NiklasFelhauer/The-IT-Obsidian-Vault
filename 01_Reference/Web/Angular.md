## Installation

1. Install Angular CLI globally:
    
    ```shell
    npm install -g @angular/cli
    ```
    

## Create a New Project

1. Create a new Angular application:
    
    ```shell
    ng new my-angular-app
    ```
    
2. Navigate into the project folder:
    
    ```shell
    cd my-angular-app
    ```
    
3. Serve the application:
    
    ```shell
    ng serve
    ```
    

## Generate Components, Services, and More

1. Generate a new component:
    
    ```shell
    ng generate component my-component
    ```
    
2. Generate a new service:
    
    ```shell
    ng generate service my-service
    ```
    
3. Generate a new module:
    
    ```shell
    ng generate module my-module
    ```
    
4. Generate a new directive:
    
    ```shell
    ng generate directive my-directive
    ```
    
5. Generate a new pipe:
    
    ```shell
    ng generate pipe my-pipe
    ```
    

## Build and Deploy

1. Build the project for production:
    
    ```shell
    ng build --configuration=production
    ```
    
2. Build with Ahead-of-Time (AOT) compilation:
    
    ```shell
    ng build --aot
    ```
    
3. Deploy using Angular CLI:
    
    ```shell
    ng deploy
    ```
    

## Testing

1. Run unit tests:
    
    ```shell
    ng test
    ```
    
2. Run end-to-end (E2E) tests:
    
    ```shell
    ng e2e
    ```
    

## Debugging in Chrome DevTools

Here are a few useful commands for live Angular debugging in Chrome:

1. **Inspect a component instance from the DOM**
    
    ```js
    ng.getComponent($0)
    ```
    
    Select an Angular component in the Elements tab, then run this to get its instance and inspect properties like `tableColumns`, `rowData`, etc.
    
2. **Check a property value**
    
    ```js
    ng.getComponent($0).tableColumns
    ```
    
    Directly view or debug any public variable on the selected component.
    
3. **Log row data from a component**
    
    ```ts
    console.table(this.tableRows)
    ```
    
    Add this inside your component to print your row data in a nice tabular format in the console.
    

> 💡 Tip: Use browser breakpoints and `debugger` statements inside methods to pause and inspect live code.