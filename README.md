# Real-Time-Chat-App

## ✅ 1. Project Structure

🔧 Backend (/server)
* Node.js + Express

* Socket.IO for WebSockets

* PostgreSQL (via Drizzle ORM)

* Redis for status tracking

* JWT Authentication

🌐 Frontend (/client)
* Next.js with TypeScript

* REST API calls for login/register

* WebSocket (Socket.IO client) for chat

* UI: Tailwind CSS

## ✅ 2. Backend Setup (server/)
>🔹 Install dependencies
npm init -y
npm install express socket.io jsonwebtoken bcryptjs drizzle-orm pg cors redis dotenv
npm install -D typescript ts-node @types/express @types/node @types/jsonwebtoken @types/bcryptjs

>🔹 File Structure
** server/
    ├── src/
    │   ├── index.ts
    │   ├── config/
    │   │   └── db.ts
    │   ├── routes/
    │   │   └── auth.ts
    │   ├── controllers/
    │   │   └── authController.ts
    │   ├── middleware/
    │   │   └── authMiddleware.ts
    │   ├── sockets/
    │   │   └── chat.ts
    │   ├── utils/
    │   │   └── redis.ts
    │   └── drizzle/
    │       └── schema.ts
    ├── .env
    └── tsconfig.json

## Drizzle + PostgreSQL Setup
>> npx drizzle-kit init

## Frontend Setup (client/)
>> 🔹 Dependencies
  ** npx create-next-app@latest chat-client --typescript
    cd chat-client
    npm install socket.io-client axios jwt-decode
