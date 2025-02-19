

# 🏗️ Flutter Architecture – How It Works  

Flutter follows a layered architecture that helps in **building high-performance cross-platform apps** using a **single codebase**.  

## 🔹 1️⃣ **Flutter Framework (UI Layer)**  
This is the top layer that developers interact with. It provides:  
- **Widgets**: Everything in Flutter is a widget! (`StatelessWidget`, `StatefulWidget`)  
- **Rendering**: Paints UI elements on the screen.  
- **Animation & Gestures**: Handles user interactions smoothly.  
- **State Management**: Manages UI updates (`setState()`, Provider, Riverpod, etc.)  

## 🔹 2️⃣ **Flutter Engine (Core Layer)**  
This is the heart of Flutter, responsible for:  
- **Dart Runtime**: Executes Dart code efficiently.  
- **Skia Graphics Engine**: Renders UI elements at **60 or 120 FPS** for smooth animations.  
- **Text & Layout**: Handles fonts, text rendering, and layout calculations.  

## 🔹 3️⃣ **Platform Channels (Bridge to Native Code)**  
This allows Flutter to communicate with native Android & iOS code.  
- Uses **MethodChannels** to interact with platform-specific features like Camera, GPS, etc.  
- Enables calling **Kotlin/Java (Android)** and **Swift/Objective-C (iOS)** directly.  

## 🔹 4️⃣ **Embedder (Platform Layer)**  
- Runs Flutter inside a native app on Android, iOS, Web, macOS, Windows, and Linux.  
- Uses the device’s **native APIs** (like touch, gestures, and hardware access).  

---
### **Flutter Architecture Diagram** 🏗️

```plaintext
+-----------------------------+
|        Flutter App (UI)     |   <-- Your Dart Code (Widgets & Logic)
+-----------------------------+
             ⬇️
+-----------------------------+
|     Flutter Framework       |   <-- UI, Gestures, Animations
+-----------------------------+
             ⬇️
+-----------------------------+
|     Flutter Engine (C++)    |   <-- Uses Skia for Rendering & Dart Runtime
+-----------------------------+
             ⬇️
+-----------------------------+
|    Platform Channels        |   <-- Connects to Native Features (Camera, GPS)
+-----------------------------+
             ⬇️
+-----------------------------+
|    Native Platform (OS)     |   <-- Android (Java/Kotlin) | iOS (Swift/Obj-C)
+-----------------------------+
```

## 🚀 **How Does Flutter Run on Multiple Platforms?**  
1. **Single Dart Codebase** → Written by the developer.  
2. **Flutter Engine** → Converts it into platform-independent UI using Skia.  
3. **Platform Channels** → Communicates with native features when required.  
4. **Compiled to Native Code** → Runs directly on Android/iOS without needing a bridge (unlike React Native).  

✅ **No WebView** (Unlike React Native, Flutter does not rely on WebViews for UI rendering).  
✅ **Fast Performance** (Direct compilation to ARM machine code).  
✅ **Truly Native Look & Feel** (Uses Flutter’s own rendering engine).  


# 🎨 Everything in Flutter is a Widget!  

In Flutter, **everything on the screen is a widget**. Widgets are the **building blocks** of a Flutter app.  

## 🔹 Types of Widgets  

### 1️⃣ **StatelessWidget** – Fixed UI (Does not change)  
- Used when the UI **remains the same** after being built.  
- **Class Name**: `StatelessWidget`  
- **Main Method**: `build(BuildContext context) → Widget`

### 2️⃣ **StatefulWidget** – Dynamic UI (Can change)  
- Used when the UI **needs to change** based on user interaction or state updates.  
- **Class Name**: `StatefulWidget`  
- **Main Methods**:  
  - `createState() → State` (Creates the mutable state)  
  - `setState(() { ... })` (Updates the UI when state changes)  

## 🔹 Why Flutter Uses Widgets?  
✅ **Reusability** – Can be used multiple times.  
✅ **Fast Updates** – Only changed parts are rebuilt.  
✅ **Customization** – Easy to style and modify.  
✅ **Cross-Platform** – Works on Android, iOS, and Web.  
