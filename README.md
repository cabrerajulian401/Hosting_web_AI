# Web-AI Frontend

A React-based frontend for the Web-AI research application.

## 🚀 Vercel Deployment

### Frontend (Vercel)
1. Connect your GitHub repository to Vercel
2. Set the following environment variables in Vercel:
   - `VITE_API_URL`: Your backend API URL (e.g., `https://web-ai-v4vh.onrender.com`)
3. Deploy - Vercel will automatically build and deploy your frontend

**Important**: Make sure your backend is deployed and accessible before deploying the frontend!

### Backend (Render/Railway/Railway)
1. Deploy the `python_backend` folder separately
2. Set environment variables for your backend:
   - `OPENAI_API_KEY`
   - `TAVILY_API_KEY`
   - `PEXELS_API_KEY`
   - `EVENT_REGISTRY_API_KEY`

## 🛠️ Local Development

### Frontend
```bash
npm install
npm run dev
```

### Backend
```bash
cd python_backend
pip install -r requirements.txt
python main.py
```

## 📁 Project Structure

```
├── client/                 # Frontend React app
│   ├── src/
│   └── public/
├── python_backend/         # Backend FastAPI app
│   ├── main.py
│   └── requirements.txt
├── server/                 # Node.js server files (legacy)
├── shared/                 # Shared schemas
└── attached_assets/        # Static assets
```

## 🔧 Environment Variables

### Frontend (.env)
```
VITE_API_URL=https://your-backend-url.com
```

### Backend (.env)
```
OPENAI_API_KEY=your_openai_key
TAVILY_API_KEY=your_tavily_key
PEXELS_API_KEY=your_pexels_key
EVENT_REGISTRY_API_KEY=your_event_registry_key
```

## 🚀 Build Commands

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Preview production build

## 📦 Dependencies

### Frontend
- React 18
- Vite
- TypeScript
- Tailwind CSS
- Radix UI Components
- TanStack Query

### Backend
- FastAPI
- LangChain
- OpenAI
- Tavily
- BeautifulSoup4 