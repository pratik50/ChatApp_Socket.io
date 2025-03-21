# ChatApp

A real-time chat application built with **Android (Kotlin)** for the client and **Node.js (Socket.IO)** for the server.

---

## Features

1. **Real-Time Messaging**:
   - Send and receive messages in real-time using **Socket.IO**.
   - Messages are displayed in a **RecyclerView**.

2. **MVVM Architecture**:
   - The app follows the **Model-View-ViewModel (MVVM)** architecture for clean separation of concerns.
   - **ViewModel** manages UI-related data and communicates with the **Repository**.

3. **Room Database**:
   - Messages are stored locally using **Room Database** for offline persistence.
   - Previous chats are loaded when the app is reopened.

### Server
- **Real-Time Communication**: Handles real-time messaging with Socket.IO.

---

## How to Run

### Prerequisites
- **Node.js** (for server)
- **Android Studio** (for client)
- **JDK** (for Android development)

### Running the Server
1. Navigate to the `server` directory:
   ```bash
   cd server
2. Install dependencies:
   ```bash
   npm install
3. Start the server:
   ```bash
    node server.js 
4. The server will run on http://localhost:3000.

### Running the Android Client
1. Open the `android_app` folder in **Android Studio**.
2. Sync the project with Gradle files.
3. **For Emulator**:
   - Start an Android emulator from the AVD Manager.
   - The server URL in the app is set to `http://10.0.2.2:3000` (for localhost on the emulator).
   - Change the localhost value if requried from uils/constants.kt file
4. **For Physical Device**:
   - Connect your Android device via USB and enable **USB debugging**.
   - Replace the server URL in the app with your machine's **local IP address** (e.g., `http://192.168.x.x:3000`).
   - Ensure both the device and the server are on the **same network**.
5. Build and run the app.
  
