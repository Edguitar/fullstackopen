sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: [{ content: "eddy", date: "2025-10-16T01:35:26.054Z" }]
    deactivate server
     Note right of browser: Note created


    Note right of browser: Rendering in the same page