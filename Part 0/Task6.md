:::mermaid
sequenceDiagram
    participant User
    participant WebBrowser
    participant Server

    User->>WebBrowser: Enters note content
    WebBrowser->>WebBrowser: Updates UI with note content
    User->>WebBrowser: Clicks Save button
    WebBrowser->>Server: Sends note data (POST /api/notes)
    Server-->>WebBrowser: Responds with success message (200 OK)
    WebBrowser->>WebBrowser: Updates UI with success message
