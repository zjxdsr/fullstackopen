# part0

## Execise 0.4

```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST new_note
    activate server
    server-->>browser: 302 code (found)
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    activate server
    server-->>browser: Notes HTML document
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: CSS file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>browser: the JavaScript file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>browser: [{"content": "dd","date": "2023-10-18T08:52:56.422Z"},...]
    deactivate server
```

## Exercise 0.5

```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server-->>browser: HTML document
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: the css file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    activate server
    server-->>browser: the JavaScript file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>browser: [{"content": "lelele", "date": "2023-10-20T08:07:08.146Z"}, ... ]
    deactivate server
```

## Exercise 0.6

```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST new_note_spa
    activate server
    server-->>browser: 201 code (created)
    deactivate server
```