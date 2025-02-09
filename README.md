# Flutter online Shopping(ShopSphere) App with Admin Panel

## Purpose  
This project is a Flutter-based mobile application designed to provide users with a platform to browse products, manage their accounts, and place orders. It also includes a comprehensive admin panel for managing users, products, orders, and notifications.

## Technologies and Frameworks  
- **Flutter**: For building the cross-platform mobile application.  
- **Firebase**: For authentication, notifications, and backend services.  
- **Dart**: The programming language used for Flutter development.  
- **Firebase Cloud Messaging (FCM)**: For push notifications (as seen in `fcm_service.dart` and `notification_service.dart`).  
- **RESTful APIs**: For handling backend operations like order placement and user management.  

## Project Structure  
The project is organized as follows:  

### Assets  
Contains static resources like images and icons.  
- `final-google-logo.png`  
- `splash-icon.json`  
- `whatsapp-icon.png`  

### Lib  
Contains the main application code.  

#### Controllers  
Manages application logic and state.  
- `sign-in-controller.dart`  
- `sign-up-controller.dart`  
- `forget-password-controller.dart`  
- `cart-price-controller.dart`  
- `notification_controller.dart`  
- `rating_controller.dart`  

#### Models  
Defines data structures.  
- `cart-model.dart`  
- `categories-model.dart`  
- `order-model.dart`  
- `product-model.dart`  
- `review_model.dart`  
- `user-model.dart`  

#### Screens  
Contains UI screens for the app.  

##### Admin Panel  
Admin-specific screens.  
- `admin-main-screen.dart`  

##### Auth UI  
Authentication-related screens.  
- `forget-password-screen.dart`  
- `sign-in-screen.dart`  
- `sign-up-screen.dart`  
- `splash-screen.dart`  
- `welcome-screen.dart`  

#### Services  
Handles backend services and APIs.  
- `fcm_service.dart`  
- `genrate-order-id-service.dart`  
- `get_server_key.dart`  
- `notification_service.dart`  
- `place-order-service.dart`  
- `send_notification_service.dart`  

#### Utils  
Contains utility functions and constants.  
- `app-constant.dart`  
- `manage-keyboard.dart`  

#### Widgets  
Contains reusable UI components.  

- `firebase_options.dart`  
- `main.dart`: The entry point of the application.  

### iOS  
iOS-specific configuration files.  

## Steps to Clone and Run the Project  

1. **Clone the Repository**  
   Clone the repository from GitHub.  

2. **Navigate to the Project Directory**  
   Move into the project folder.  

3. **Install Dependencies**  
   Install all required dependencies using Flutter.  

4. **Run the Application**  
   Launch the application on an emulator or physical device.  

## Repository Link  
[Flutter E-commerce App with Admin Panel](https://github.com/manan123488/flutter-ecommerce-app-with-admin-panel)  

## Steps to Commit Project Structure and Initial Files  

1. **Initialize a Git Repository**  
   Set up a new Git repository in the project directory.  

2. **Add All Files to the Staging Area**  
   Stage all project files for the initial commit.  

3. **Commit the Files with a Message**  
   Create the initial commit with a descriptive message.  

4. **Link the Local Repository to the Remote GitHub Repository**  
   Connect the local repository to the remote GitHub repository.  

5. **Push the Files to the Remote Repository**  
   Upload the initial commit to the remote repository.  

This document provides a comprehensive guide to understanding, setting up, and contributing to the Flutter E-commerce App with Admin Panel project.


The image appears to depict a MongoDB Compass interface, showing the structure of a database named `online-Shopping` with a collection named `users`. Below is a breakdown of the database structure based on the provided content:

---

### **Database Structure**

#### **Database Name**: `online-Shopping`

#### **Collections**:
1. **`users`**  
   - This collection stores user-related data.
   - Each document in the `users` collection contains the following fields:

| Field Name   | Data Type               | Example Value                                      |
|--------------|-------------------------|---------------------------------------------------|
| `_id`        | ObjectId                | `ObjectId('9?a4fbe3766fab768b88ee3')`             |
| `name`       | String                  | `"admin"`                                         |
| `email`      | String                  | `"admin@gmail.com"`                               |
| `password`   | String                  | `"5255-1950X19j10e9FnddNNUlgLcOcpmA1fZnIVnvEubB8HNK74fa7311cc1"` |
| `phone`      | String                  | `"09875553211"`                                   |
| `address`    | String                  | `"Libror"`                                        |
| `answer`     | String                  | `"football"`                                      |
| `role`       | Integer                 | `0`                                               |
| `createAt`   | ISODate (Timestamp)     | `2025-02-06T18:13:55.683+00:00`                   |
| `updateAt`   | ISODate (Timestamp)     | `2025-02-06T18:14:49.879+00:00`                   |
| `__v`        | Integer                 | `0`                                               |

---

#### **Other Collections in `online-Shopping` Database**:
- **`categories`**: Likely stores product categories.
- **`online-users`**: Possibly tracks currently active or logged-in users.
- **`orders`**: Likely stores order-related data.
- **`products`**: Likely stores product-related data.

---

### **Key Observations**:
1. **User Roles**:
   - The `role` field in the `users` collection is an integer (`0` in the example). This likely represents user roles (e.g., `0` for admin, `1` for regular users).

2. **Timestamps**:
   - `createAt` and `updateAt` fields track when the user was created and last updated, respectively.

3. **Security**:
   - Passwords are stored as hashed strings (likely using a secure hashing algorithm).

4. **Database Management**:
   - MongoDB Compass is used to manage and query the database.
   - The interface allows for adding, updating, and deleting data.

---

### **Example Document in `users` Collection**:
```json
{
  "_id": ObjectId("9?a4fbe3766fab768b88ee3"),
  "name": "admin",
  "email": "admin@gmail.com",
  "password": "5255-1950X19j10e9FnddNNUlgLcOcpmA1fZnIVnvEubB8HNK74fa7311cc1",
  "phone": "09875553211",
  "address": "Libror",
  "answer": "football",
  "role": 0,
  "createAt": ISODate("2025-02-06T18:13:55.683Z"),
  "updateAt": ISODate("2025-02-06T18:14:49.879Z"),
  "__v": 0
}
```

---

This structurer , where user management, product categorization, and order tracking are essential components. Let me know if you need further clarification or assistance! 😊


The provided content outlines a set of API endpoints for a web application, likely related to user authentication, category management, and product management. Here's a description of each API endpoint:

1. **POST auth Register**: This endpoint is used to register a new user. It typically requires user details such as username, email, and password.

2. **POST auth Login**: This endpoint allows a registered user to log in. It usually requires credentials like email and password and returns an authentication token upon successful login.

3. **GET test**: This might be a test endpoint to check if the authentication is working correctly. It could return a simple message or status.

4. **POST create category**: This endpoint is used to create a new category. It likely requires details such as the category name and description.

5. **PUT update category**: This endpoint allows updating an existing category. It might require the category ID and the new details to be updated.

6. **GET get category**: This endpoint retrieves a list of all categories.

7. **GET get single category**: This endpoint fetches details of a specific category, usually by its ID.

8. **DEL delete category**: This endpoint deletes a specific category, typically requiring the category ID.

9. **POST create-product**: This endpoint is used to create a new product. It likely requires product details such as name, description, price, and category.

10. **GET get product**: This endpoint retrieves a list of all products.

11. **GET get single product**: This endpoint fetches details of a specific product, usually by its ID.

12. **GET get product picture**: This endpoint retrieves the image associated with a specific product.

13. **DEL delete product**: This endpoint deletes a specific product, typically requiring the product ID.

14. **PUT update product**: This endpoint allows updating an existing product. It might require the product ID and the new details to be updated.

The **Parameters** section indicates that these APIs might require an authorization token in the headers for secure access. The **Response** section suggests that there might be a history of API calls or responses, but it's not detailed in the provided content.

These APIs collectively form the backbone of a system that manages user authentication, categories, and products, which could be part of an e-commerce platform or a content management system.
