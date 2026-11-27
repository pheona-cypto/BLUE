```mermaid
flowchart TB
    Providers["<b>Student Provider</b></br>Creates profiles and list skills or products"]
    Consumers["<b>Student Consumers</b><br/>Searches, browses, sends requests/bookings, and reviews"]
    Admin["<b>Administrator</b><br/>Campus Moderator<br/>Reviews reported listings and handles disputes"]

    GG["<b>Campus Connect</b><br/>Software System<br/>Connects verified students to offer, search,<br/>and request skills or products on campus"]

    Verify["<b>Identity Verification</b><br/>External System<br/>Verifies student status (school email / matric number)"]
    Messaging["<b>Messaging / WhatsApp</b><br/>External System<br/>Private communication and request updates"]
    Media["<b>Media Storage</b><br/>External System<br/>Stores listing photos"]
    Payments["<b>Payments / Finance (Open)</b><br/>External System<br/>Only if in-app/external flow is confirmed"]

    Providers -->|"Creates listings and manages requests"| GG
    Consumers -->|"Browses and contacts sellers"| GG
    Admin -->|"Reviews reported listings"| GG

    GG -->|"Checks student verification status"| Verify
    GG -->|"Routes notifications / links chat channel"| Messaging
    GG -->|"Stores and retrieves listing images"| Media
    GG -.->|"Handles payments or fees (if confirmed)"| Payments
```
Gist & Grind connects verified students on campus—starting at Babcock University—so providers can offer skills, products, 
or services while buyers can search, browse, and send exchange or booking requests, with administrators reviewing 
reported listings and external services handling identity verification, media storage, messaging/notifications, and (if later confirmed) payments.
