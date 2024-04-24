:::mermaid
sequenceDiagram
    participant User
    participant WebBrowser
    participant Server

    User->>WebBrowser: Enters URL "https://studies.cs.helsinki.fi/exampleapp/spa"
    WebBrowser->>Server: Requests single-page app
    Server-->>WebBrowser: Responds with HTML, CSS, and JavaScript files
    WebBrowser->>WebBrowser: Renders single-page app UI