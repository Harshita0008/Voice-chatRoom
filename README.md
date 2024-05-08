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

1. Challenge: When dealing with multiple voices concurrently, ensuring synchronization poses a significant challenge. This is especially true in real-time applications where delays or mismatches can lead to confusion or disruption.

Solution: Refining the server architecture was key to addressing this challenge. This involved optimizing the server to efficiently handle concurrent voice streams, ensuring that each voice is processed and synchronized in real-time. Techniques such as load balancing, efficient resource allocation, and prioritization of voice streams were implemented to ensure smooth synchronization.
Recording Conversations:

2. Challenge: Recording conversations introduces complexities in terms of data storage, security, and accessibility. Ensuring that voice data is captured accurately, securely stored, and readily accessible when needed presents significant hurdles.

Solution: Integration of specialized tools tailored for voice data capture and storage was crucial in overcoming this challenge. These tools provide robust mechanisms for capturing voice data with high fidelity, encrypting it for security, and storing it in secure, scalable storage systems. Additionally, implementing access controls and auditing mechanisms ensures that voice data is only accessible to authorized personnel, thereby addressing privacy and security concerns.

3. Challenge: Deploying a complex voice application can be challenging, especially when considering factors such as scalability, reliability, and accessibility across different platforms and devices.

Solution: Streamlining the deployment process using platforms like Vercel can greatly simplify the deployment of voice applications. Vercel provides tools and services for seamless deployment, automatic scaling, and continuous integration/continuous deployment (CI/CD), reducing the overhead associated with managing infrastructure. By leveraging Vercel's platform, deployment becomes more efficient, ensuring uninterrupted accessibility for users while also enabling easy scaling to accommodate growing demand. Additionally, Vercel's support for serverless functions can be utilized to handle backend tasks, further simplifying the deployment architecture.
