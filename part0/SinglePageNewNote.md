```mermaid
sequenceDiagram
    participant user
    participant browser
    participant server

    user->>browser: Clicks Save button
    browser-->>user: Render note list

    browser->>server: POST https//studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 created
    deactivate server
```