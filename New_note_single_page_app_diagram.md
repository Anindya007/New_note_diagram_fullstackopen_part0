sequenceDiagram
    participant browser
    participant server

    Note right of browser: The browser executing JavaScript code to insert the note in place on form submission. Then the browser executes AJAX code to persist the note to the server. 

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 created status code
    deactivate server

    
