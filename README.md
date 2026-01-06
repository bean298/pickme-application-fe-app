# 📱 PickMe – Frontend App

Frontend mobile application for **PickMe – Pre-orde

PickMe is a food pre-ordering platform that allows users to order food in advance and pick it up directly at restaurants, helping users save time and avoid delivery delays.

This Flutter application communicates with the **PickMe Backend API** to provide authentication, ordering, and location-based features.

---

## 🚀 Tech Stack

### 📱 Frontend Framework
- Flutter (Dart SDK)
- Material Design
- Cupertino Icons (iOS-style UI components)

### 🌐 Networking & API
- `http` – RESTful API communication
- JWT-based authentication (handled by backend)

### 🔐 Local Storage & Config
- `shared_preferences` – Local data & token storage
- `flutter_dotenv` – Environment variable management

### 🧭 Navigation
- `go_router` – Declarative routing and navig

### 🖼 Media & Assets
- `image_picker` – Pick images from camera or gallery
- `flutter_svg` – Render SVG assets

### 🗺 Map & Location (OpenStreetMap)
- `flutter_map` – OpenStreetMap rendering
- `geolocator` – Current location detection
- `geocoding` – Address ↔ coordinate conversion
- `latlong2` – Latitude/longitude utilities
- `flutter_map_location_marker` – Live location marker
- `flutter_polyline_points` – Route & direction polylines

### 📊 Data Visualization
- `fl_chart` – Charts and analytics visualization

### 📝 Utilities
- `intl` – Date, time, and number formatting
- `multi_select_flutter` – Multi-select UI components

---

## 🧩 Main Features

### 👤 Customer
- Register and login
- Browse restaurants and menus
- Pre-order food and select pickup time
- View restaurant locations on the map
- Get route directions to restaurants
- Manage pickup addresses
- Submit feedback after order completion

### 🧑‍🍳 Restaurant Owner
- Manage restaurant profile and location
- Manage menus and food items
- View all revenue and all orders status

### 🧑‍💼 Admin
- View system statistics
- Monitor users and restaurants
- Manage system data via backend APIs

---

## ⚙️ Environment Configuration

1. Create a `.env` file at the root of the project:

```env
# API URL FOR REAL DEVICE
API_URL=http://192.168.1.5:8080/api

# API URL FOR ANDROID EMULATOR
# API_URL=http://10.0.2.2:8080/api
```

---

⚙️ Installation & Run

Clone the repository and run the frontend:

```bash
git clone <frontend-repo-url>
flutter pub get
flutter run
```

Run on Android Emulator, make sure .env uses:

```
API_URL=http://10.0.2.2:8080/api
```

Run on Real Device, ensure your phone and backend server are on the same network

```
API_URL=http://YOUR_LOCAL_IP:8080/api
```

---

## 🔄 System Flow

This section describes how the **PickMe Frontend App** interacts with users and the backend system from authentication to order completion.

### 👤 User (Customer)

Register → Login  →  Browse restaurants (Home / Map)  → Select restaurant → View menu  → Add items to cart  → Select pickup time  
→ Place order → Payment  → Track order status  → Pick up food at restaurant  → Submit rating & feedback

### 🧑‍🍳 Restaurant Owner
Register → Login → Create restaurant profile  → Submit restaurant for approval  → Wait for Admin approval  → Add and manage menu items  
→ Receive customer pre-orders  → Update order status (Preparing → Ready)  → View orders & revenue  & feedback

---

Video demo:

```
https://drive.google.com/file/d/1PeEM6wOXhGfFAIvdIqtM6rW5LF746Wi3/view?usp=sharing 
```






































