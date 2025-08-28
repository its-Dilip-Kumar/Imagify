
### 1. Clone the Repository
```bash
git clone https://github.com/singh04ayush/imagify.git
cd imagify
```

### 2. Backend Setup
```bash
# Navigate to server directory
cd server

# Install dependencies
npm install

# Create .env file in the server directory
touch .env

# Add the following environment variables to .env:
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLIPDROP_API=your_clipdrop_api_key

# Start the server
npm run server
```

#### Backend Environment Variables Explanation
| Variable | Description | Example |
|----------|-------------|---------|
| `PORT` | Server port number | `5000` |
| `MONGODB_URI` | MongoDB connection string | `mongodb+srv://username:password@cluster.mongodb.net/imagify` |
| `JWT_SECRET` | Secret key for JWT authentication | `your-secret-key-here` |
| `CLIPDROP_API` | API key for ClipDrop image generation | `your-clipdrop-api-key` |

### 3. Frontend Setup
```bash
# Open a new terminal
# Navigate to client directory
cd client

# Install dependencies
npm install

# If vite not installed
npm install vite@latest

# Create .env file in the client directory
touch .env

# Add the following environment variable to .env:
VITE_BACKEND_URL=http://localhost:5000

# Start the development server
npm run dev
```

#### Frontend Environment Variables Explanation
| Variable | Description | Example |
|----------|-------------|---------|
| `VITE_BACKEND_URL` | Backend API URL | `http://localhost:5000` |

### 4. Access the Application
- Frontend: `http://localhost:5173`
- Backend API: `http://localhost:5000`

> **Important Notes**: 
> - Never commit your `.env` files to version control
> - Make sure to replace the example values with your actual configuration
> - The CLIPDROP_API key can be obtained from [ClipDrop API](https://clipdrop.co/apis)
> - Keep your JWT_SECRET secure and use a strong random string

<div align="center">

### Development Scripts

| Command | Description |
|---------|-------------|
| `npm run server` | Starts backend |
| `npm run dev` | Starts frontend |

### Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `PORT` | Server port | 5000 |
| `MONGODB_URI` | MongoDB connection string | - |
| `JWT_SECRET` | JWT secret key | - |



