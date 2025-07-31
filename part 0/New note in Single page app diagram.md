```mermaid
sequenceDiagram
    participant browser
    participant server


    Note right of browser: The spa page has been loaded    
    Note right of browser: The user writes a new note and hits the "Save" button

    browser->>+server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    server-->>-browser: Status code 201 Created ()

    Note right of browser: The browser updates the list of notes dynamically using JavaScript, without reloading the page
```
