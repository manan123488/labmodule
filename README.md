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
