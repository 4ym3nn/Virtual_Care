# Guide of Installation - 2CP Project

Welcome to the 2CP Project! This guide provides comprehensive instructions for setting up and running both the backend and frontend components of the project locally, as well as accessing the deployed version online.

---

## 🚀 Live Demo

You can view the deployed version of the project here: 👉 **[2CP Project Live](https://2cp-project-silk.vercel.app)**

---

## 🛠️ Local Development Setup

### Backend Setup

1. **Navigate to the Backend Directory**  
    Ensure you are inside the `default-server/` directory:  
    ```bash
    cd default-server
    ```

2. **Install Backend Dependencies**  
    Make sure you have Node.js (v16+ recommended) and npm (v7+ or v8+) installed. Then run:  
    ```bash
    npm install
    ```

3. **Start the Backend Development Server**  
    Launch the backend server in development mode:  
    ```bash
    npm run dev
    ```

---

### Frontend Setup

1. **Clone the Repository**  
    Clone the project repository and navigate to the `client/` directory:  
    ```bash
    git clone <your-repo-url>
    cd 2CP-Project/client
    ```

2. **Install Frontend Dependencies**  
    Ensure Node.js (v16+ recommended) and npm (v7+ or v8+) are installed. Then run:  
    ```bash
    npm install --legacy-peer-deps
    ```

3. **Start the Frontend Development Server**  
    Start the development server, typically accessible at `https://localhost:3000`:  
    ```bash
    npm run dev
    ```

---

## ✅ Requirements

- **Node.js**: v16+ (recommended)  
- **npm**: v7+ or v8+  

---

## 📁 Project Structure

### Backend (`default-server/`)

```plaintext
default-server/
├── cert.pem               # SSL certificate (for HTTPS)
├── key.pem                # SSL key
├── config/                # Configuration files
├── controlers/            # Controller logic
├── middlewares/           # Express middlewares
├── models/                # Database models
├── routes/                # API route handlers
├── socket/                # Socket.io logic
├── doctori_backup.sql     # SQL backup file
├── eslint.config.mjs      # Linter configuration
├── package.json           # Project metadata and scripts
├── package-lock.json      # Dependency lock file
└── server.js              # Entry point of the backend server
```

### Frontend (`client/`)

```plaintext
client/
├── public/                 # Static assets
├── src/                    # Source files
├── components.json         # Component definitions
├── config.ts               # Configuration files
├── next.config.ts          # Next.js config
├── tailwind.config.ts      # Tailwind CSS config
├── postcss.config.mjs      # PostCSS config
├── eslint.config.mjs       # ESLint config
├── vercel.json             # Vercel deployment config
├── server.js               # Custom server (if used)
├── cert.pem, key.pem       # SSL Certificates (for dev or self-hosting)
├── package.json            # Project metadata and scripts
├── tsconfig.json           # TypeScript config
└── README.md               # Project documentation
```

---

## 📦 Scripts

### Backend Scripts

- `npm run dev` - Start the backend server in development mode  
- `npm start` - Start the backend server in production mode (if configured)  

### Frontend Scripts

- `npm run dev` - Start the frontend development server  
- `npm run build` - Build the frontend for production  
- `npm start` - Start the frontend production server (if applicable)  

---

## 🔐 Notes on HTTPS

If using SSL (`cert.pem` and `key.pem`) for either the backend or frontend, ensure the server is configured to use HTTPS in the respective `server.js` files.

---

## 📡 Deployment

The frontend of this project is deployed using **Vercel**. To deploy, connect your GitHub repository to Vercel for instant deployment.

---

## 🛠️ Troubleshooting

For any issues during setup, refer to the `README.md` in the `client/` or `default-server/` directories or contact the project maintainer.  

Feel free to reach out if you encounter any challenges during setup.  

**Happy Coding!** 🚀🎉
