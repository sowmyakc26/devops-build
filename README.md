# React App Deployment & Monitoring Project

This project demonstrates the containerization of a React application using **Docker**, deployment on **AWS EC2**, and professional monitoring using **Uptime Kuma** with **Discord** notification alerts.

---

##  Tech Stack
- **Frontend:** React.js
- **Platform:** AWS EC2 (Ubuntu)
- **Containerization:** Docker
- **Monitoring:** Uptime Kuma (Open Source)
- **Notifications:** Discord via Webhooks

---

##  Deployment Steps

### 1. Dockerization
The application is containerized using a multi-stage Dockerfile. To run the app:
```bash
# Build the image
docker build -t react-app-prod .

# Run the container
docker run -d -p 80:80 --name react-container react-app-prod
```

### 2. Monitoring Setup
**Uptime Kuma** is used to monitor the application's heartbeat. It is configured to:
- Check the application status every **60 seconds**.
- Send instant alerts if the service is unreachable.

### 3. Notification Integration
Integrated **Discord Webhooks** to receive real-time updates:
- **[DOWN] Alert:** Sent immediately when the React app stops.
- **[UP] Alert:** Sent when the service recovers.

---


---

## 🔗 Project Links
- **Deployed URL:** [http://54.211.29.37](http://54.211.29.37)

---
**screenshots**

<img width="2496" height="1179" alt="screenshot1" src="https://github.com/user-attachments/assets/f2f30d67-ff36-4f96-8e2f-17b50e4d13cb" />

<img width="2449" height="1257" alt="screenshot3 jenkins ready" src="https://github.com/user-attachments/assets/671c38c6-3c40-46f6-92b3-3708c4b0c3a4" />

<img width="2550" height="887" alt="screenshot 4 dockerhub" src="https://github.com/user-attachments/assets/a970ef35-6147-4bb6-aba4-8993a03203e0" />

<img width="2489" height="1238" alt="screenshot5 pipeline view" src="https://github.com/user-attachments/assets/75a89bcb-9116-44aa-8ea6-0b7880d25b60" />

<img width="2504" height="1238" alt="screenshot6 console output" src="https://github.com/user-attachments/assets/3fcbaacb-a999-45fa-8c3b-18908a94259d" />

<img width="2538" height="1235" alt="screenshot7" src="https://github.com/user-attachments/assets/72afa1c1-26f6-4648-a91b-af9c90e4a801" />

<img width="2499" height="1077" alt="screenshot8 prod image" src="https://github.com/user-attachments/assets/83929a31-f93a-413a-a5da-a61ae1852b46" />

<img width="2542" height="1226" alt="screenshot9 consoleoutput for pod" src="https://github.com/user-attachments/assets/f529ff66-c21e-4326-8f66-5b840965d550" />

<img width="2525" height="1259" alt="screenshot2 live app" src="https://github.com/user-attachments/assets/a6348a90-9013-41d6-bc5f-2c5f4af37ed4" />


<img width="2549" height="1141" alt="monitoring testing op" src="https://github.com/user-attachments/assets/9acfd199-95a2-43fc-a43e-6a466a5e8ed5" />

<img width="2539" height="1269" alt="uptime is down" src="https://github.com/user-attachments/assets/3c42fc5a-97f8-47de-a969-a91597c6d6a3" />
