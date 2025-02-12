# FaceShare - Android App for Easy Photo Sharing

## Overview
FaceShare is an Android application designed to revolutionize the way you share group photos. By combining facial recognition technology with seamless integration with WhatsApp, FaceShare makes it easy to identify and connect people in your photos, ensuring that everyone in the image gets a high-quality version of it. 

### Key Features
- **User Registration**: Users can register within the app, capturing their facial features for future identification.
- **Facial Recognition**: Utilizing FaceApi, the app analyzes the facial features of individuals in the photo to recognize and match registered users.
- **High-Quality Image Storage**: Photos are uploaded to an Express server, stored with high resolution, and linked to the identified users.
- **Efficient Sharing**: Once the app identifies the people in the image, it sends a WhatsApp message to those individuals with a link to the high-quality image, allowing them to download it instantly.
- **Fast Image Sharing**: Share images effortlessly and at the highest quality, without compression or loss of detail when sending via WhatsApp.

## How It Works
1. **Register Users**: Users take a picture of themselves to store their facial features in the database.
2. **Take Group Photos**: Users can take group photos where the app identifies all faces within the image.
3. **Upload & Identify**: The image is uploaded to the server where facial recognition algorithms identify the people in the photo by matching their features to those stored in the database.
4. **Sharing via WhatsApp**: Once the identities are matched, a WhatsApp message is sent to each identified person with a link to download the high-quality image.

## Technologies Used
- **Android (Java/Kotlin)**: For the mobile application development.
- **Express.js**: A fast, minimalist web framework for handling backend requests.
- **FaceApi**: Used for detecting and analyzing facial features.
- **MongoDB**: A NoSQL database used to store user data and facial features.
- **WhatsApp API**: For sending messages with download links to identified users.
- **AWS S3/Server Storage**: To store images in high quality.

## Setup & Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/FaceShare.git
    ```
2. **Backend Setup**:
    - Navigate to the backend directory:
        ```bash
        cd backend
        ```
    - Install dependencies:
        ```bash
        npm install
        ```
    - Set up environment variables such as database credentials and API keys for WhatsApp and FaceApi.
    - Start the Express server:
        ```bash
        npm start
        ```
3. **Frontend (Android App) Setup**:
    - Open the project in Android Studio.
    - Configure the app with your server details (API endpoint, etc.).
    - Build and run the app on your Android device or emulator.

## How to Use
- **Register**: Create an account by uploading a photo of yourself.
- **Take a Group Photo**: Use the app to take a photo of a group, and it will automatically detect faces.
- **Receive a Link**: If the faces are identified, you’ll receive a WhatsApp message with a link to download the high-quality image.
- **Download the Photo**: Click the link in the WhatsApp message to download the image without losing quality.

## Why FaceShare?
- **Efficient Sharing**: Instantly share high-quality images with people who appear in the photos, without worrying about compression and resolution loss.
- **Easy Registration**: Simple user registration that lets you easily identify and share photos with people.
- **Fast & Secure**: With robust facial recognition and secure cloud storage, FaceShare guarantees a smooth and safe user experience.

## Contributing
We welcome contributions! If you'd like to help improve FaceShare, feel free to fork the repository, create an issue, or submit a pull request.

1. Fork the repository.
2. Create a new branch for your feature.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Create a pull request.

## Acknowledgements
- [FaceApi](https://www.face-api.js.org/) for facial recognition.
- [WhatsApp API](https://www.twilio.com/whatsapp) for sending messages.
- [Express.js](https://expressjs.com/) for the backend server.
- [MongoDB](https://www.mongodb.com/) for the database storage.

---

Feel free to reach out if you have any questions or suggestions!
