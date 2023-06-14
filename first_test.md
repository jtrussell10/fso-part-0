```mermaid
sequenceDiagram
    participant browser
    participant server
    browser->>server: HTTP POST to new_note
    server->>browser: HTTP status code 302
    browser->>server: GET notes
    server->>browser: HTML document
    browser->> server: GET css
    server->> browser: css file 
    browser->> server: GET js  
    server->> browser: JavaScript file
    browser->>server: GET json
    server->>browser: json
```