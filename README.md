# probarber-architecture
Technical showcase and architecture overview of ProBarber, a full-stack SaaS platform built with Laravel, Angular, and PHP. Focused on scalability and clean code.

# ProBarber - Architecture Showcase ⚙️

This repository serves as a **technical documentation and architectural overview** of the ProBarber SaaS platform. The project was built from the ground up **(Green Field)** to solve complex management challenges in the beauty industry. White-labelling and modularization have been top priorities from the start.

## 🛠 Tech Stack
* **Backend:** **Laravel (PHP)** **-** robust data validation via **FormRequests** and business rules enforcement through **Actions.**
* **Frontend:** **Angular** **-** **TanStack Query** for efficient state management and server-state synchronization.
* **Database:** **MySQL** **-** lightweight relational data integrity.
* **Testing:** **PHPUnit** **-** automated backend testing to ensure reliability.
* **Messaging:** **FireBase FCM** for real-time push-notifications.
* **Logging:** **AWS DynamoDB NoSQL** **-** decouple audit logs from the primary transactional database.
* **Multi-Tenancy:** Logical Data Isolation using **Global Query Scopes** to ensure secure tenant-level data partitioning.
* **Dashboard:** All dashboard operations run from **cache.** No server load and instant feedback for a seamless user experience.
* **Mobile:** Custom HTML and SCSS rules for **mobile devices.**
* **SMTP:** Brevo integration for reliable e-mailing, currently used for password recoveries and onboarding.

## 📊 Core Features & Business Logic
* **Appointment Management:** A highly interactive interface for scheduling and managing barbers' availability.
* **Zero-Friction Workflow:** No client-owner interaction required to confirm a slot; the system handles the handshake.
* **Instant Notifications:** As soon as a booking is confirmed, Firebase FCM triggers a notification to the user instantly.
* **Dashboard & CRM:** Detailed customer profiles with service history, preferences, and automated retention tools.
* **Real-time Analytics:** Instant insights into revenue, peak hours, and occupancy rates directly on the main dashboard.
* **Mobile Experience:** Tailored UI/UX designed for the specific high-mobility needs of beauty professionals.

## 🏗 Key Engineering Pillars
My goal with this architecture was to implement the core concepts of high-performance systems:
* **Reliability:** High test coverage and error handling.
* **Scalability:** Database modeling designed to support high-load multi-tenant growth.
* **Maintainability:** Clean code principles and modular architecture for easy evolution.
* **White-Label Architecture:** Designed with a decoupled core, making the platform ready for rapid rebranding and niche adaptation (e.g., ProBeauty, ProPet) without code duplication.

## 🗺️ Roadmap & Future Enhancements
While the core SaaS engine is functional, the following features are planned to further improve scalability and developer experience:
* **Infrastructure:** Containerization using **Docker** for consistent environment orchestration.
* **Messaging Integration:** **Meta API (WhatsApp)** integration for promotional messaging and automated reminders with official business verification.
* **SaaS Monetization:** Stripe/Asaas integration for automated subscription billing, ensuring seamless tenant access management.

## 🎯 Product-Minded Approach
This project was designed with **User Experience** in mind, ensuring that technical complexity never hinders operational efficiency.

## 📸 Project Preview

The ProBarber platform emphasizes operational efficiency and a seamless user experience.

| Management Interface & General Styling |
| :---: |
| <img src="https://github.com/user-attachments/assets/6df31d4f-87af-4ced-862f-56afb21f745d" width="100%" /> |
| *Main dashboard showcasing the intuitive scheduling system.* |

| Mobile Specific Interfaces |
| :---: |
| <img width="1080" height="741" alt="image" src="https://github.com/user-attachments/assets/fd55722a-52a5-4ce3-b783-a54c3eec212a" /> |
| *UX planned around barber's high-mobility day-to-day scenarios.* |

| Project Organization | Automated Testing |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/8dea8aba-8a75-410e-bc39-3bcd0cdc046d" width="359" /> | <img src="https://github.com/user-attachments/assets/492f8637-d56e-4f02-9086-6396be129c2f" width="359" /> |
| *Complex structures organized for high maintainability.* | *Fully operational automated testing.* |



