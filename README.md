# 🩸 Haemo-Agent Network

### Offline Emergency Blood Coordination AI | Powered by Gemma 4

![Status](https://img.shields.io/badge/Status-Hackathon_Ready-red)
![Offline](https://img.shields.io/badge/Offline-100%25-brightgreen)
![Gemma](https://img.shields.io/badge/Powered%20By-Gemma%204-red)

---

## The Problem

In rural Nigeria, over 70% of health facilities experience frequent internet outages. When a trauma patient arrives and needs blood, doctors lose access to donor databases. They resort to panic phone calls, searching through paper lists, and calling hospitals one by one. Patients bleed out while they wait.

Existing solutions assume constant connectivity. In reality, emergencies rarely happen when the Wi-Fi is working.

---

## Our Solution

Haemo-Agent Network is a fully offline AI coordination system that puts the power of regional blood coordination directly into the hands of frontline healthcare workers—no internet required.

### How It Works

When a doctor types an emergency like "I need O+ blood for a trauma patient":

1. Gemma 4 extracts the blood type.
2. Agentic Search executes – Python functions search the local donor database, check 90-day eligibility, and calculate distances using offline Haversine math.
3. Regional Network Scan – The system checks nearby hospitals within 50km for available blood stock.
4. Explainable Report – A complete Emergency Dispatch Report is generated with donor names, phone numbers, distances, and reasoning for each recommendation.

All of this happens in seconds. All offline. All on a laptop.

---

## Tech Stack

- AI Model: Google Gemma 4 (via Ollama)
- Framework: Python 3.12 + Gradio UI
- Logic: Offline donor search, eligibility checks, Haversine distance math
- Data: In-memory mock data (resets on restart)

---

## Key Features

| Feature | Description |
| :--- | :--- |
| Command Center | One input triggers donors, inventory, and nearby hospitals with live Chain-of-Thought streaming. |
| Intelligence Dashboard | Ask plain English questions about hospital data. Gemma answers based on local data. |
| Compatibility Checker | Gemma explains why a donor is or isn't a match, with educational reasoning. |
| Donor Registration | Add new donors to the network. (Mock data, resets on restart). |
| Inventory Management | Update hospital blood stock levels. (Mock data, resets on restart). |
| Hospital Registration | Add new hospitals to the network. (Mock data, resets on restart). |

---

## How to Run

### Prerequisites
- Python 3.12 (3.13 is not supported)
- Ollama installed from ollama.com

### Installation & Setup

1. Clone this repository

### Installation & Setup

1.  **Clone the repository**
    ```bash
    git clone (https://github.com/Smart-Techie/Haemo_Agent_Network)
    cd HaemoAgent
