Bot

Space Bot API Investigation Sheet
**Total Marks: 30**
**Part 1: Collect Required API Documentation**
This investigation sheet helps you gather key technical information from the three
APIs required for the Space Bot project: **Webex Messaging API**, **ISS Current
Location API**, and a **Geocoding API** (LocationIQ or Mapbox or other), plus the
Python time module.
---
Webex api: MDIzZGJmN2QtMDFkOS00MDhkLWEwNzQtZjMzYWMxN2FjNjhjYzkwZWY3MTItNjBj_P0A1_bdd2aed2-da17-481d-bd6f-b43037ee90b7

| Criteria | Details |
|---------|---------|
| API Base URL | https://webexapis.com/v1//
| Authentication Method | `bearer token` |
| Endpoint to list rooms | `/rooms` |
| Endpoint to get messages | `/messages` |
| Endpoint to send message | `/messages ` |
| Required headers | `__Authorisation and content type` |
| Sample full GET or POST request | `{
    "items": [
        {
            "id": "Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL1JPT00vMzMzM2IwNjAtYWYyZC0xMWYwLTllMTItYTdlMDg1ODg0Nzhl",
            "title": "BOT",
            "type": "group",
            "isLocked": false,
            "lastActivity": "2025-10-22T10:15:00.228Z",
            "creatorId": "Y2lzY29zcGFyazovL3VzL1BFT1BMRS8yNzg0YTk3NS01MjRkLTQ5MzAtYjEzZi1lNmRkZDc2NDUyY2U",
            "created": "2025-10-22T09:55:11.590Z",
            "ownerId": "Y2lzY29zcGFyazovL3VzL09SR0FOSVpBVElPTi9iZGQyYWVkMi1kYTE3LTQ4MWQtYmQ2Zi1iNDMwMzdlZTkwYjc",
            "isPublic": false,
            "isReadOnly": false
        },
        {
            "id": "Y2lzY29zcGFyazovL3VybjpURUFNOnVzLXdlc3QtMl9yL1JPT00vODgxMjNjNDAtYTQyZi0xMWYwLWEzYTQtNzczM2UyOGI1MWIw",
            "title": "Naesha's space",
            "type": "group",
            "isLocked": false,
            "lastActivity": "2025-10-08T10:14:10.180Z",
            "creatorId": "Y2lzY29zcGFyazovL3VzL1BFT1BMRS8yNzg0YTk3NS01MjRkLTQ5MzAtYjEzZi1lNmRkZDc2NDUyY2U",
            "created": "2025-10-08T10:14:10.180Z",
            "ownerId": "Y2lzY29zcGFyazovL3VzL09SR0FOSVpBVElPTi9iZGQyYWVkMi1kYTE3LTQ4MWQtYmQ2Zi1iNDMwMzdlZTkwYjc",
            "isPublic": false,
            "isReadOnly": false
        }
    ]
}
` |
---
## Section 2: ISS Current Location API (3 marks)
| Criteria | Details |
|---------|---------|
| API Base URL | `_______________________________` |
| Endpoint for current ISS location | `_______________________________` |
| Sample response format (example JSON) |
```
```
|
---
## Section 3: Geocoding API (LocationIQ or Mapbox or other) (6 marks)
| Criteria | Details |
|---------|---------|
| Provider used (circle one) | **LocationIQ / Mapbox/ other -provide detail** |
| API Base URL | `_______________________________` |
| Endpoint for reverse geocoding | `_______________________________` |
| Authentication method | `_______________________________` |
| Required query parameters | `_______________________________` |
| Sample request with latitude/longitude | `_______________________________` |
| Sample JSON response (formatted example) |
```
```
|
---
## 🚀 Section 4: Epoch to Human Time Conversion (Python time module) (2 marks)
| Criteria | Details |
|---------|---------|
| Library used | `_______________________________` |
| Function used to convert epoch | `_______________________________` |
| Sample code to convert timestamp |
```
```
|
| Output (human-readable time) | `_______________________________` |
---
## 🚀 Section 5: Web Architecture & MVC Design Pattern (12 marks)
### 🚀 Web Architecture – Client-Server Model
- **Client**:
- **Server**:
- (Explain the communication between them & include a block diagram )
### 🚀 RESTful API Usage
-
-
-
### 🚀 MVC Pattern in Space Bot
| Component | Description |
|------------|-------------|
| **Model** | |
| **View** | |
| **Controller** | |
#### Example:
- Model:
- View:
- Controller:
---
### 🚀 Notes
- Use official documentation for accuracy (e.g. developer.webex.com, locationiq.com
or Mapbox, open-notify.org or other ISS API).
- Be prepared to explain your findings to your instructor or demo how you retrieved
them using tools like Postman, Curl, or Python scripts.
---
### Total: /30


To complete this Space Bot API Investigation Sheet, follow the steps below section by section, ensuring you extract accurate data from the official API documentation of each service. This will help you understand the APIs used in your Space Bot project, and be prepared for integration and testing.
________________________________________
✅ Section 1: Webex Messaging API (7 marks)
What to Do:
1.	Go to https://developer.webex.com.
2.	Log in with a Cisco Webex account.
3.	Navigate to the "Docs" or "API Reference" section.
Fill in:
Criteria	What You Should Do
API Base URL	Look for the root URL used in all API calls (e.g. https://webexapis.com/v1).
Authentication Method	Usually uses Bearer tokens (OAuth 2.0).
Endpoint to list rooms	Find the endpoint to retrieve a list of Webex rooms (e.g. GET /rooms).
Endpoint to get messages	Find the endpoint to read messages from a room (GET /messages).
Endpoint to send message	The POST endpoint for sending a message (POST /messages).
Required headers	Typically includes Authorization: Bearer <token> and Content-Type: application/json.
Sample full GET or POST request	Provide an example request with method, endpoint, headers, and sample body if needed. Use cURL, Postman, or Python requests.
________________________________________
🛰️ Section 2: ISS Current Location API (3 marks)
What to Do:
1.	Visit: http://open-notify.org/Open-Notify-API/ISS-Location-Now/
Fill in:
Criteria	What You Should Do
API Base URL	Usually http://api.open-notify.org.
Endpoint for current ISS location	Typically /iss-now.json.
Sample response format	Copy and paste an example JSON response, e.g.:
{
  "message": "success",
  "timestamp": 1633036200,
  "iss_position": {
    "latitude": "45.0",
    "longitude": "-122.3"
  }
}
``` |

---

## 🗺️ Section 3: Geocoding API (LocationIQ, Mapbox, or other) (6 marks)

### What to Do:


### Fill in:
| Criteria | What You Should Do |
|---------|--------------------|
| Provider used | Circle the one you’re using (LocationIQ, Mapbox, or other). |
| API Base URL | Example for LocationIQ: `https://us1.locationiq.com/v1`. |
| Endpoint for reverse geocoding | e.g. `/reverse.php` (LocationIQ) or `/geocoding/v5/mapbox.places/{lon},{lat}.json` (Mapbox). |
| Authentication method | Usually API key as a query parameter or header. |
| Required query parameters | Include things like `lat`, `lon`, `key`, and `format=json`. |
| Sample request | Include a full URL with sample lat/lon and key (mask your real key). |
| Sample JSON response | Copy a real example of the response (shortened if necessary). |

---

## ⏰ Section 4: Epoch to Human Time Conversion (Python time module) (2 marks)

### What to Do:
1. Use Python’s built-in `time` or `datetime` module to convert an epoch (Unix) timestamp to a readable format.

### Fill in:
| Criteria | What You Should Do |
|---------|--------------------|
| Library used | Most commonly `time` or `datetime`. |
| Function used | `time.ctime()`, `datetime.fromtimestamp()` or similar. |
| Sample code | Example:
```python
import time
epoch = 1633036200
readable = time.ctime(epoch)
print(readable)
or
from datetime import datetime
dt = datetime.fromtimestamp(1633036200)
print(dt.strftime('%Y-%m-%d %H:%M:%S'))
|
| Output | What the output of the code looks like, e.g. "Wed Sep 30 22:30:00 2021" |
________________________________________
🧩 Section 5: Web Architecture & MVC Design Pattern (12 marks)
🌐 Web Architecture – Client-Server Model
What to Do:
•	Define the client (e.g., user interface, browser, or chat interface like Webex).
•	Define the server (your Python backend, Flask app, etc.).
•	Explain how they interact via HTTP requests and API responses.
•	Draw or describe a simple block diagram:
[Client (Webex Bot UI)] <---> [Server (Python App with Flask)] <---> [APIs (Webex, ISS, LocationIQ)]
________________________________________
🔁 RESTful API Usage
What to Do:
•	Explain how RESTful principles are applied:
o	Use of HTTP methods (GET, POST, etc.)
o	Statelessness
o	Resource-oriented URLs
o	JSON-formatted responses
________________________________________
🧠 MVC Pattern in Space Bot
What to Do:
•	Map your project parts to Model, View, and Controller:
| Component | Description |
|------------|-------------|
| Model | Logic for interacting with APIs (e.g., ISS data, geolocation data). |
| View | Output to the user, e.g., messages sent to the Webex chat. |
| Controller | Logic that handles user input from Webex and determines what to do (e.g., what data to fetch, how to respond). |
Example:
•	Model: Function to get ISS coordinates.
•	View: Webex message showing location/address.
•	Controller: Webhook handler responding to incoming message events.
________________________________________
Final Tips:
•	Use Postman, Python requests, or curl to test actual API calls.
•	Use official docs only—do not copy from random blogs.
•	If doing this for a demo, be ready to show live API responses or sample code.
Let me know if you'd like example code, official documentation links, or help with testing these APIs.

