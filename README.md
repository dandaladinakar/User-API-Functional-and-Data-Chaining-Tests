## User-API-Functional-and-Data-Chaining-Tests

### Overview:
This collection of tests checks if the API for creating, updating, retrieving, and deleting users is working properly. We use Postman to run these tests, and we create random user details (like name and email) each time to avoid using the same data repeatedly.

### Key Points:

#### 1. Connecting Tests (Data Chaining):
The tests are linked. For example, when we create a user, we save their ID and use it in the next test to update or delete that user. This makes the process smooth.

#### 2. Creating Random User Data:
Every test generates a new username and email. This helps avoid errors from using the same data and ensures fresh information.

### API Functions We Test:
- **Create**: Add a new user.
- **Get (Retrieve)**: Get details of the created user.
- **Update**: Change the user's details.
- **Delete**: Remove the user from the system.

### Checking Results:
Each test checks the API's response. We look for status codes like 200 (OK) or 201 (Created) to make sure everything works.

### Using Environment Variables:
We use variables like `username`, `useremail`, and `id` to store information. This makes it easier to run tests with different users or settings.

### Security:
All requests use a Bearer Token to ensure only authorized users can access the API.
