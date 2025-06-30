🛒 BaskNOW – Smart Delivery Fallback System
BaskNOW is a smart delivery simulation app that demonstrates how a real-world quick commerce platform handles inventory shortages using a dark store + kirana fallback model. If an item is unavailable in the dark store, it automatically finds nearby kirana stores to fulfill the order, simulates the rider route with animated map tracking, and gives a complete final order summary with ETA.

🚀 Features
✅ Fulfillment from a central Dark Store

✅ Automatic fallback to nearby Kirana Stores

🧠 Smart matching of missing items using inventory logic

🗺️ Animated rider route simulation on Leaflet maps

⏱ ETA calculation using Haversine distance

🧾 Final merged order summary and price breakdown

⚡ Modern UI with basic animations and clean layout

🗺️ Flow Overview
mermaid
Copy
Edit
graph TD
A[User Places Order] --> B[Dark Store Checks Inventory]
B -->|Items Available| C[Fulfilled by Dark Store]
B -->|Items Missing| D[Kirana Fallback Matching]
D --> E[Rider Route Simulation on Map]
E --> F[Final Order Summary + ETA]

🧩 Tech Stack
Tech	Usage
React	Component-based architecture
React-Leaflet	Map and rider animation
OpenStreetMap	Base map tiles
JavaScript	Fallback logic + ETA calculations
CSS3	UI styling & animations
Mock Data	Simulated inventories and orders

📁 Project Structure
css
Copy
Edit
📦src
 ┣ 📂components
 ┃ ┣ 📜DarkStoreSummary.jsx
 ┃ ┣ 📜FallbackItemMatcher.jsx
 ┃ ┣ 📜MapRouteSimulator.jsx
 ┃ ┣ 📜FinalOrderSummary.jsx
 ┃ ┣ 📜OrderSummary.jsx
 ┣ 📜App.jsx
 ┣ 📜main.jsx
🧠 How It Works
Simulates a user order (e.g., Milk, Bread, Eggs)

Checks dark store inventory

If items are missing → finds kirana stores in the same pincode

Animates the complete delivery route:
Dark store → Kiranas → Customer

Calculates delivery ETA based on total distance

Merges and displays final item summary + price

📦 Installation
bash
Copy
Edit
git clone https://github.com/yourusername/basknow.git
cd basknow
npm install
npm run dev
App will run locally at: http://localhost:5173/ (Vite default)

🔮 Future Improvements
🧾 Backend for real-time inventory updates

🧭 Distance-based kirana selection (not just pincode)

🛑 Quality score/reliability of kirana stores

📱 Mobile-first responsive UI

📦 User-auth & cart persistence

✨ Learnings & Highlights
How fallback systems work in real-world commerce
React architecture + component state management
Geo-based distance calculation with the Haversine formula
Simulating delivery logic visually with maps
UI design for modern ordering systems

📄 License
This project is licensed under the MIT License.

👤 Author
Rajan Kumar Das
💼 Building creative tech solutions | ⚙️ Robotics & Product Thinking

⭐ Star This Repo
If you like this project, give it a ⭐ — it really helps!

