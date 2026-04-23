This project implements a RESTful API that allows users to manage a collection of playing cards. The API supports standard CRUD operations:

Create a new card

Read all cards

Read a specific card

Update a card (PUT / PATCH)

Delete a card


JSON formatted responses

🚀 Installation & Setup
1️⃣ Clone or Download Project

Extract the project folder.

2️⃣ Install Dependencies
pnpm install

or

npm install
3️⃣ Run the Server
pnpm run dev

or

node index.js
4️⃣ Open in Browser
http://localhost:3000
📌 API Endpoints
🔹 GET /cards

Fetch all cards.

Response:

[
  {
    "id": 1,
    "suit": "Hearts",
    "value": "Ace"
  }
]
🔹 GET /cards/:id

Fetch a specific card by ID.

Status Codes:

200 → Success

404 → Card not found

🔹 POST /cards

Create a new card.

Request Body:

{
  "suit": "Spades",
  "value": "King"
}

Status Codes:

201 → Created

400 → Invalid input

🔹 PUT /cards/:id

Replace an existing card completely.

🔹 PATCH /cards/:id

Update partial card data.

🔹 DELETE /cards/:id

Delete a card.

Status Codes:

200 → Deleted

404 → Not Found

📊 Sample Data Structure
{
  "id": 1,
  "suit": "Diamonds",
  "value": "Queen"
}
🧠 RESTful Features Implemented

Stateless requests

Resource-based routing (/cards)

Proper HTTP methods (GET, POST, PUT, PATCH, DELETE)

Meaningful status codes (200, 201, 400, 404, 500)

JSON responses

🧪 Testing

The API was tested using Postman.

Tested Scenarios:

Adding a new card

Retrieving all cards

Updating a card

Deleting a card

Handling invalid ID requests

🔐 Future Improvements

Add MongoDB database integration

Implement authentication using JWT

Add pagination (page & limit query parameters)

Add input validation middleware
