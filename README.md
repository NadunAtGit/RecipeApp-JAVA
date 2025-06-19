📱 The Chef App (Java Android)
A fully featured recipe-sharing mobile app built with Java, Android, and Firebase. This app allows users to register, log in, view, upload, and manage recipes with support for both images and videos via Firebase Authentication and Firebase Storage.

🚀 Features
🔐 User Authentication (Email & Password)

📤 Upload recipes (text, image, video)

📂 Firebase Storage (with folders: recipes/, recipes_videos/)

📄 View and manage your own recipes

🔎 Browse categories like snacks, drinks, desserts, etc.

📱 Built using Android SDK (Java)

🛠️ Getting Started
Follow these steps to set up and run the project locally.

🔁 1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/NadunAtGit/RecipeApp-JAVA.git
cd RecipeApp-JAVA
📦 2. Open in Android Studio
Open Android Studio

Choose "Open an Existing Project"

Select the cloned folder (RecipeApp-JAVA)

Let Gradle sync automatically

📥 3. Install Dependencies
Gradle will automatically download all required dependencies.
If it doesn't:

Go to File → Sync Project with Gradle Files

Or run ./gradlew build from the terminal

🔐 4. Firebase Setup
Step 1: Create a Firebase project
Go to Firebase Console → Add Project

Step 2: Add Android App
Use your app’s package name: com.example.thechef

Step 3: Download google-services.json
Place it inside:
app/google-services.json

Step 4: Enable Firebase services:
Authentication → Enable Email/Password sign-in

Storage → Go to Build → Storage

Create two folders inside Firebase Storage:

Copy
Edit
recipes/
recipes_videos/
You can do this by uploading a dummy file to each folder in the Firebase console.

🔧 5. Run the App
Connect your emulator or physical device

Click ▶️ Run in Android Studio

📁 Project Structure Overview
pgsql
Copy
Edit
app/
├── java/com/example/thechef/
│   └── [All activity and feature classes]
├── res/
│   └── layout, drawable, values, etc.
├── google-services.json  ← must add manually
📸 Firebase Storage Usage
recipes/ — stores recipe images

recipes_videos/ — stores recipe videos

You can retrieve, display, and manage these using Firebase Storage SDK.

🧪 Tech Stack
Java (Android)

Firebase Authentication

Firebase Realtime Database

Firebase Storage

Glide (Image loading)

ExoPlayer (Video playing)

Material UI

🙋‍♂️ Contribution
Pull requests are welcome. For major changes, open an issue first to discuss what you'd like to change.