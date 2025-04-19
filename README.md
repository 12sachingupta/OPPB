![image](https://github.com/user-attachments/assets/e42508c3-869d-4c13-9c98-7204384b025a)

![image](https://github.com/user-attachments/assets/ed0dda5b-1d55-43b4-8b53-74d8844b0791)

![image](https://github.com/user-attachments/assets/a1c1a0a6-6006-4545-a614-5a50247f70f9)

![image](https://github.com/user-attachments/assets/56d81f86-26a2-41fc-8e23-88f91f6ed512)

![image](https://github.com/user-attachments/assets/36b0f21c-008f-4b69-a379-2b71a428b29c)
![image](https://github.com/user-attachments/assets/39f53c5b-d1e8-44e6-8262-c006726316e7)


![image](https://github.com/user-attachments/assets/78d73835-cb56-4260-b94e-17a3e9dc850a)

# Offline Peer-to-Peer Payment Bridge (OPPB)

![OPPB Logo](./assets/logo.png)

OPPB is a decentralized, offline-first digital payment application engineered to ensure seamless transactions during network outages or in remote areas. By leveraging mesh networking, Bluetooth, Wi-Fi Direct, and SMS fallback mechanisms, OPPB empowers users—from urban tech-savvy individuals to rural communities—to securely perform transactions without relying on conventional internet connectivity.

## Table of Contents
- [Features](#features)
- [Dynamic UI/UX Screens](#dynamic-uiux-screens)
- [Architecture Overview](#architecture-overview)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

## Features
- **Offline Transaction Capability**  
  - **Mesh Networking & Bluetooth/Wi-Fi Direct:** Communicate directly between devices without internet access.
  - **SMS Fallback:** Securely confirm and process transactions using SMS when no data connection is available.
- **Decentralized Ledger & Deferred Synchronization**  
  - Local transaction logging with visual indicators for pending versus synced transactions.
  - Automatic deferred synchronization once network connectivity is restored.
- **Dynamic, Multilingual UI/UX**  
  - A fully responsive, component-based UI with animated transitions and interactive elements.
  - Simplified, icon-driven workflows with real-time form validations and guided transaction steps.
  - Built-in language support (e.g., English, Hindi, and one local language) and accessibility features (ARIA labels, keyboard navigation, high contrast modes).
- **Advanced Security & Dual Authentication**  
  - Dual authorization via simulated biometric (fingerprint/face) scans and OTP verification.
  - Robust encryption and offline certificate-based verification ensuring trust in every transaction.
- **Modular & Integration-Ready Design**  
  - Components are developed as modular React components to enable easy future integration with backend API services for full synchronization.
  - Flexible configuration for additional features such as digital wallets, transaction history, and settings.

## Dynamic UI/UX Screens
OPPB’s UI/UX experience is designed to be dynamic and engaging:
- **Splash & Onboarding Screen:**  
  - Animated welcome page with motion graphics and a multi-slide introduction highlighting key offline features.
- **Login/Registration:**  
  - Sleek, animated forms with real-time validation, seamless toggling between login and registration, and support for biometric sign-in.
- **Dashboard:**  
  - Intuitive dashboard displaying account balance, recent transactions (with live status updates), and animated interactive charts.
- **Payment Initiation:**  
  - A step-by-step guided form with progress indicators, dropdown selectors with auto-suggestions, and dynamic previews of digital receipts.
- **Confirmation & Security:**  
  - Animated confirmation screens featuring secure lock icons, progress spinners for transaction processing, and modal dialogs for OTP entry.
- **Transaction History:**  
  - A scrollable, filterable ledger with swipe-to-view-details functionality and status icons (pending, synced).
- **Settings & Multilingual Options:**  
  - Interactive settings page with toggles, sliders, and drop-downs that instantly preview changes (e.g., theme switching).

*Note: Screenshots and GIFs demonstrating the dynamic transitions and animations can be found in the [assets/screenshots](./assets/screenshots) folder.*

## Architecture Overview
OPPB is built with an offline-first philosophy:
- **Frontend:**  
  - Developed in React using functional components and hooks.
  - Dynamic styling managed via Tailwind CSS for rapid prototyping and responsive design.
- **Offline Local Storage:**  
  - Transactions and state information are stored locally, ensuring continuity until online connectivity is restored.
- **Deferred Synchronization:**  
  - Once network connectivity is re-established, a sync module pushes local data to a centralized backend (or directly to bank APIs) for final settlement.
- **Security:**  
  - Local authentication using dual-factor mechanisms, certificate-based validations, and encryption using industry-standard algorithms.

*Architecture diagrams and flowcharts are available in the [docs/architecture](./docs/architecture) folder.*

## Technology Stack
- **Frontend:** React, Tailwind CSS, React Router
- **Backend (Deferred Sync):** Node.js, Express (integration planned)
- **Security:** Built-in OTP module, simulated biometric authentication, and local encryption libraries
- **Utilities:** i18next for multilingual support, Axios for REST API interactions (for later synchronization)

## Installation
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YourUsername/OPPB.git
   cd OPPB







