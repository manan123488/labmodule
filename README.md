# Flutter E-commerce App with Admin Panel

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
