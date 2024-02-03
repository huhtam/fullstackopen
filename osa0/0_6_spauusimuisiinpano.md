````mermaid
sequenceDiagram
    participant browser
    participant server
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server-->>browser: Status: 201 Created
    deactivate server

    Note right of browser: No redirecting. Default (redirecting) prevented.