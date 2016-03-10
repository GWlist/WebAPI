# WebAPI
WebAPI design document


Services:

Create a user: POST /api/v1/profiles
Update user profile: PUT /api/v1/profiles/{profileID}
Create a new item to sell:  POST /api/v1/items
Edit an item that you are selling:  PUT /api/v1/items/{itemID}
Buy an item:  PUT /api/v1/items/{itemID}?sold=Y
Give a grade to user after buying item: PUT /api/v1/items/{itemID}?rating={score}
Search for items to buy: GET /api/v1/items
Search for items from specific seller: GET /api/v1/items?pid={profileID}

Calculation:
Find another users’ average rating: GET /api/v1/profiles/{id}
Find top 5 best sellers: GET /api/v1/service/top5
