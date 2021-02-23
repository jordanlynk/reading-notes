# View Components

- Similiar to partial views, however much more powerful. View components don't use model binding and only depend on the data provided when calling into it. 
- Consists of 2 parts: *The class* and *the result it returns*
- View components:
    - Renders a chunk, rather than a whole response
    - Includes the same separtation of concerns & testability benefits found between a controller and view.
    - Can have parameters and business logic
    - Invoked from a layout page (typically)
- Intended to utilize anywhere you have resuable rendering logic:
    - Dynamic nav menus
    - Tag cloud 
    - Login panel
    - Shopping cart
    - Recently published articles
    - Sidebar content on a typical blog 
