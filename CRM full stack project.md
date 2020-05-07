# CRM full stack project

## Project Requirements
- MERN stack project
- Login and Register User
    - Duplicate email IDs not allowed
    - On Login handle wrong password, wrong email and successful login states
        - use `bcrypt` package to store password hash and compare supplied password
- Use cookie-session package to handle the sessions
    - send logged in user's `userID` as cookie value  
- On successful login redirect users to '/customers'
- Customers endpoint (table with customers) only visible if user is logged-in
    - the get request which fetches the customer should check if user is logged in or not
    - return 403 if user is not logged in
- When save new customer request is sent, add owner property which is equal to `userID`
- On customers endpoint only display the customers which belogns to logged in user
