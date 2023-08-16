# Module D - Interactive Guest Experience

Developers will focus on creating an interactive frontend application for guests utilizing the DineEase service. The main objective is to provide users with an easy-to-navigate platform to explore restaurants, view detailed menus, read past reviews, and place orders.

## Task Specifications:

### 1. User Login Page

Developers need to create a dedicated login page where users can enter their credentials and gain access to the platform. The login process will be facilitated by the provided backend API.

#### **Login**
- **Objective:** Allow users to log in using their registered email and password.
- **UI Elements:**
  - Email Input Field
  - Password Input Field
  - Login Button
  - Link to the Registration Page for new users
- **Functional Requirements:**
  - Input validation for correct email format.
  - Masked password input.
  - Error handling for failed login attempts.
  - On successful login, store the received JWT token for authenticating subsequent requests.

#### **Logout**
- **Objective:** Offer users a mechanism to securely log out from their session.
- **UI Elements:**
  - Logout Button
- **Functional Requirements:**
  - Clear the stored JWT token.
  - Redirect the user back to the login page.

### 2. New User Registration Page

A platform for new users to sign up and create an account. 

- **Objective:** Enable users to create a new account by providing their email, password, and name.
- **UI Elements:**
  - Name Input Field
  - Email Input Field
  - Password Input Field
  - Confirm Password Input Field
  - Registration Button
  - Back to Login Button
- **Functional Requirements:**
  - Input validation for correct email format and password matching.
  - After successful registration, store the received JWT token and direct the user to the homepage.
  - Provide feedback in case of errors, like when an email is already registered.

### 3. Browsing and Searching Restaurants Page (homepage)

Facilitate users in exploring and searching for restaurants.

- **Objective:** Display a list of restaurants and offer a search functionality.
- **UI Elements:**
  - Search Bar
  - Tile view of restaurants with name, description, average rating and "Continue" link.
  - "Show more results" link
- **Functional Requirements:**
  - Fetch and display restaurants from the backend.
  - Display 6 randomly selected restaurants at first time. If there are more restaurants and user clicks on the "Show more results" link, all the remained restaurants should appear.
  - Implement search functionality by making requests to the backend with the query string. Display the first 6 from restaurants from the search results, and use the "Show more results" as above.
  - Clicking on Continue link of a restaurant card will redirect the user to the detailed restaurant page.
  - Restaurants that the user has previously ordered from are displayed with a purple border.

### 4. Restaurant Page with Menu Card

A dedicated page showcasing all details related to a selected restaurant.

#### **Ordering**
- **Objective:** Allow users to select dishes from the menu and place an order.
- **UI Elements:**
  - List of menu items with name and price.
  - Quantity selector for each menu item.
  - Add to cart (+) button.
  - Finish Order button.
- **Functional Requirements:**
  - If users click the "Add to Cart" button next to a menu item, that item will be added to the cart with a quantity of 1.
  - The "Finish Order" button displays the total amount of the order.
  - Clicking finish order button Finish Order page should appear.
  - Orders should be retained when the browser is reloaded.

#### **Review with Rating**
- **Objective:** Users should be able to leave reviews and ratings for a restaurant.
- **UI Elements:**
  - Star Rating Selector (1-5 stars).
  - Comment Text Area.
  - Submit Review Button.
  - List of past reviews with reviewer name, rating, and comment.
- **Functional Requirements:**
  - Submitting a review sends the rating and comment to the backend.
  - Fetch and display past reviews for the restaurant from the backend.

### *Finish Order*

#### **Objective:** 
Facilitate the user in finalizing their order, making payment, and receiving a confirmation.

#### **UI Elements:**
  - **Review Cart:** A summary of all items added with their respective quantities and individual prices.
  - **Total Amount:** Displays the cumulative price of all items.
  - **Finish Order Button:** To finalize the order after verifying all details.

#### **Functional Requirements:**
  - Upon selecting items and clicking the "Finish Order" button, the user should be shown their cart's content.
  - Users should have the ability to remove items.
  - Display an estimated total.
  - Post-confirmation, the user should receive an on-screen message.
  


