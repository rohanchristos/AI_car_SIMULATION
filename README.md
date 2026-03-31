# 🚗 Self-Driving Car Simulation

A self-driving car simulation built from scratch using **vanilla JavaScript** — no external libraries. This project implements a complete autonomous driving system featuring neural networks, artificial sensors, collision detection, and real-time traffic simulation, all rendered on HTML5 Canvas.

## ✨ Features

- **Car Driving Mechanics** — Realistic acceleration, braking, steering, and friction physics
- **Dynamic Road System** — Procedurally defined multi-lane roads with lane markings
- **Artificial Sensors** — Ray-casting sensor system that detects road boundaries and nearby vehicles
- **Collision Detection** — Polygon-based collision detection for accurate crash handling
- **Traffic Simulation** — AI-controlled traffic vehicles with varying speeds and lane positions
- **Neural Network** — Custom-built neural network that controls the car's driving decisions
- **Network Visualization** — Real-time visualization of neural network activations and weights
- **Network Optimization** — Mutation-based optimization to evolve better driving behavior
- **Fine-Tuning** — Parameter adjustments for improved performance and stability

## 🛠️ Tech Stack

- **JavaScript** (ES6+) — Core logic, physics, and neural network implementation
- **HTML5 Canvas** — Rendering and visualization
- **CSS** — UI styling
- **LocalStorage** — Saving and loading trained neural network weights

## 📂 Project Structure

```
self-driving-car/
├── 1. Car driving mechanics/     # Core vehicle physics & controls
├── 2. Road definition/           # Road generation & lane system
├── 3. Artificial sensors/        # Ray-casting sensor implementation
├── 4. Collision detection/       # Polygon intersection algorithms
├── 5. Traffic simulation/        # NPC traffic vehicle logic
├── 6. Neural network/            # Neural network from scratch
├── 7. Visualizing neural networks/ # Real-time network visualizer
├── 8. Optimizing neural networks/  # Mutation & evolution strategies
├── 9. Fine-tuning/               # Performance tuning & parameter optimization
└── 10. Live stream variant/      # Extended variant with additional features
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/rohanchristos/AI_car_SIMULATION.git
cd AI_car_SIMULATION
```

### 2. Run the Simulation

This is a pure HTML/JS project — no `npm install` or build step required. Just serve the files using any of these methods:

#### Option A: VS Code Live Server (Recommended)
1. Install the **Live Server** extension in VS Code
2. Open any phase folder (e.g. `9. Fine-tuning/`)
3. Right-click `index.html` → **"Open with Live Server"**

#### Option B: Python HTTP Server
```bash
cd "9. Fine-tuning"
python -m http.server 8080
```
Then open [http://localhost:8080](http://localhost:8080) in your browser.

#### Option C: npx serve
```bash
npx -y serve "9. Fine-tuning"
```
Then open [http://localhost:3000](http://localhost:3000) in your browser.

> **💡 Tip:** Start with the **`9. Fine-tuning`** folder — it's the most complete version with the full self-driving AI and neural network visualization.

### 3. Train the Car

- Click 💾 **Save** to store a good-performing brain to `localStorage`
- Click 🗑️ **Discard** to clear the saved brain
- **Refresh** the page to generate new mutations from the saved brain
- Repeat the save → refresh cycle to evolve smarter driving over time

## 🧠 How It Works

1. **Sensors** cast rays from the car to detect obstacles and road boundaries
2. The sensor readings are fed as inputs into a **feedforward neural network**
3. The network outputs control signals (forward, left, right, reverse)
4. Multiple cars run in parallel with **mutated** neural networks
5. The best-performing car's brain can be **saved** and used as a base for further evolution

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
