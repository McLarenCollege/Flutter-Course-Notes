# CRM full stack project

## Project Requirements
- MERN stack project
- Login and Register User
    - Duplicate email IDs not allowed
    - On Login handle wrong password, wrong email and successful login states
        - use `bcrypt` package to store password hash and compare supplied password
- Use cookie-session package to handle the sessions
    - send logged in user's `userID` as cookie value  
- On successful login redirect users to '/customers' by using `react-router-dom` package
- Customers endpoint (table with customers) only visible if user is logged-in
    - the get request which fetches the customer should check if user is logged in or not
    - return 403 if user is not logged in and redirect user to `/login` endpoint
- When save new customer request is sent, add owner property which is equal to `userID` to be retrieved from session info
- On customers endpoint only display the customers which belongs to logged in user
