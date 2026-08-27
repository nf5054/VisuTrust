# 🛡️ VisuTrust — Decentralized Smart Contract Vision Verification

<div align="center">
  <p><strong>Bridging Blockchain Smart Contracts with Real-World Physical Verification via Zero-Shot Edge AI Vision (YOLO-World)</strong></p>
</div>

---

## 📸 UI Showcase & Screenshots


### 🖥️ Main Dashboard & Smart Contract Hub
![Dashboard Overview](./screenshots/dashboard.png)
*Overview of active automated safety contracts, financial escrow pools, and real-time verification milestones.*

### 👁️ Live Edge Vision Verification Feed
![Live Vision Feed](./screenshots/vision_monitoring.png)
*Real-time object detection and safety gear verification powered by zero-shot open-vocabulary AI.*

### ⚙️ Python Edge Manager Software (Standalone Node)
![Python Edge Manager](./screenshots/edge_manager.png)
*The desktop Edge Node interface controlling local USB/IP cameras, GPU inference, and uplink telemetry.*

### 📜 Automated Milestone Execution Log
![Execution Logs](./screenshots/contract_logs.png)
*Immutable audit trail showing verified physical events automatically triggering contract releases.*

---

## 🌟 Overview

**VisuTrust** creates an automated, trustless bridge between digital contracts and physical real-world actions. Traditional contracts require human inspectors to manually verify if work has been completed, safety gear is being worn, or objects have arrived before releasing funds. 

VisuTrust eliminates this manual bottleneck by deploying local **AI Edge Nodes** equipped with real-time computer vision that feed cryptographic verification signals directly into automated monitoring pipelines.

---

## 🧠 How It Works

VisuTrust operates on a hybrid **Cloud Application + Local Edge Node** architecture:

```
+---------------------------+        REST / Uplink Sync       +----------------------------+
|   VisuTrust Web Dashboard | <=============================> |  Python Edge Vision Node   |
|   (Smart Contracts & UI)  |      Targets & Telemetry        |  (YOLO-World + Camera Hub) |
+---------------------------+                                 +----------------------------+
             |                                                               |
             v                                                               v
 1. Define verification goals                                    2. Zero-Shot Vision Analysis
 2. Monitor execution milestones                                 3. Real-world physical verification
```

### 1️⃣ Contract Definition & Milestone Goals
Users create automated contracts inside the VisuTrust UI. Each contract defines specific physical milestones linked to natural language object queries (e.g., *"worker wearing yellow safety helmet"*, *"forklift in loading bay"*, or *"inspected shipping container"*).

### 2️⃣ Edge Node Uplink
Physical monitoring locations run the **VisuTrust Edge Node Software** connected to local cameras. The web application establishes a secure uplink to the node (e.g., `http://localhost:8080` or an intranet IP).

### 3️⃣ Zero-Shot Computer Vision (YOLO-World)
Instead of training custom AI models for months, the Edge Node leverages **YOLO-World open-vocabulary object detection**. The target text defined in the contract is synced directly to the edge camera, which immediately begins scanning the live video stream for matching physical items.

### 4️⃣ Automated Verification & Release
When the Edge Node detects the requested target with high confidence continuously over a required verification window:
1. The Edge Node logs the detection event and marks the target as **Verified**.
2. The Web Dashboard receives the verification handshake.
3. The contract milestone switches to **Completed**, automatically logging the transaction or releasing escrowed funds.

---

## ✨ Key Features

- **⚡ Zero-Shot Open Vocabulary AI:** Detect almost any physical object or safety equipment simply by typing its name into the contract goal—no machine learning dataset training required.
- **🔗 Seamless Edge-to-Cloud Sync:** Automated synchronization between online contract dashboards and offline/local monitoring cameras.
- **🛡️ Manual & Automated Fallbacks:** Includes manual override triggers and custom threshold sliders inside the Edge Manager for high-security environments.
- **📊 Real-Time Telemetry & Auditing:** Continuous frame rate monitoring, confidence tracking, and historical execution logs.

---

## 🚀 Quick Start Guide (Pre-Built Binaries)

This distribution comes pre-packaged with executable files ready to run without requiring a code compilation or build environment setup.

### 1. Launch the Web Application
- Open the provided pre-built **VisuTrust Web App** executable or double-click `index.html` (if distributed as a bundled package).

### 2. Launch the Edge Vision Node
- Double-click the standalone **`ManagerSoftware`** executable on the computer connected to your physical camera.
- The manager will initialize the camera feed and open its local API server on port `8080` by default.

### 3. Establish Uplink
1. Inside the Web Application dashboard, navigate to the **Contracts** or **Active Monitoring** section.
2. Click **Establish Uplink** and enter your Edge Node address (use `http://localhost:8080` if running on the same PC).
3. Select a contract target to start real-time vision verification!
---
 *its still a concept we didnt finish the system YET.
