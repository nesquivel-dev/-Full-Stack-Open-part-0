```mermaid
sequenceDiagram
    participant browser
    participant server

    Note left of browser: User types note and clicks save
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    Note right of browser: The payload is: "{content: "oh well, a test", date: "2026-04-06T19:25:15.286Z"}"
    server-->>browser: {"message":"note created"}
    deactivate server
    



    
```