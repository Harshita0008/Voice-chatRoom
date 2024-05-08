# Voice RoomChat

### Demo video: https://www.loom.com/share/e546634a763f401cbf6e80adf2fd9434?sid=5b3f02fd-19f6-4993-8ae7-b756a16bc9d5

## Setup and Running Instructions

This README provides guidance on setting up and running the website and voice server, along with insights into design choices, challenges faced, and their solutions.

### Installation
Website:

- Install Node.js.
- Navigate to the root folder (voice chat) in your terminal.
- Run npm install to set up dependencies.

Voice Server:

- Install Go.
- Navigate to the backend folder in your terminal.
- Run go mod tidy to manage dependencies.

### Running the Project

Website:

- Navigate to the frontend folder in your terminal.
- Run npm run dev to start the website at http://localhost:3000.

Voice Server:

- Navigate to the api folder in your terminal.
- Run go run server.go to initiate the voice server.


### Design Choices


Design Choices

Simplicity and user-friendliness remain the cornerstone of our design philosophy. We've ensured not just easy navigation but an intuitive user experience, marked by clearly labeled buttons and a cohesive layout. Real-time communication capabilities have been integrated to facilitate seamless voice exchange, 
thereby enhancing the fluidity and immediacy of conversations. Furthermore, the user management feature offers transparency into the chat room's occupants, fostering a vibrant sense of community and connection among users.

### Challenges and Solutions

##### Synchronizing Voices:
Challenges arose in synchronizing voices, especially in managing multiple voices concurrently. These were addressed by refining the server to adeptly handle concurrent voice streams.

##### Recording Conversations:
The task of recording conversations presented hurdles. These were surmounted by integrating specialized tools tailored for capturing and securely storing voice data.

##### Deployment:
The deployment process was streamlined using Vercel, simplifying deployment and ensuring uninterrupted accessibility for users.
