Flutter E-commerce App with Admin Panel
Purpose
This project is a Flutter-based mobile application designed to provide users with a platform to browse products, manage their accounts, and place orders. It also includes a comprehensive admin panel for managing users, products, orders, and notifications.

Technologies and Frameworks
Flutter: For building the cross-platform mobile application.

Firebase: For authentication, notifications, and backend services.

Dart: The programming language used for Flutter development.

Firebase Cloud Messaging (FCM): For push notifications (as seen in fcm_service.dart and notification_service.dart).

RESTful APIs: For handling backend operations like order placement and user management.

Project Structure
The project is organized as follows:

assets
Contains static resources like images and icons.

final-google-logo.png

splash-icon.json

whatsapp-icon.png

lib
Contains the main application code.

controllers
Manages application logic and state.

sign-in-controller.dart

sign-up-controller.dart

forget-password-controller.dart

cart-price-controller.dart

notification_controller.dart

rating_controller.dart

models
Defines data structures.

cart-model.dart

categories-model.dart

order-model.dart

product-model.dart

review_model.dart

user-model.dart

screens
Contains UI screens for the app.

admin-panel
Admin-specific screens.

admin-main-screen.dart

auth-ui
Authentication-related screens.

forget-password-screen.dart

sign-in-screen.dart

sign-up-screen.dart

splash-screen.dart

welcome-screen.dart

services
Handles backend services and APIs.

fcm_service.dart

genrate-order-id-service.dart

get_server_key.dart

notification_service.dart

place-order-service.dart

send_notification_service.dart

utils
Contains utility functions and constants.

app-constant.dart

manage-keyboard.dart

widgets
Contains reusable UI components.

firebase_options.dart

main.dart: The entry point of the application.

ios
iOS-specific configuration files.

Steps to Clone and Run the Project
Clone the repository:
