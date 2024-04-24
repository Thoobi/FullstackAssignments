:::mermaid
   sequenceDiagram
    participant User
    participant WebBrowser
    participant Server

    User->>WebBrowser: Writes something into the text field
    WebBrowser->>WebBrowser: Updates UI with the note
    User->>WebBrowser: Clicks Save button
    WebBrowser->>Server: Sends the note data (POST /exampleapp/notes)
    Server-->>WebBrowser: Responds with status code 200 OK