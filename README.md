# AI Chatbot - React Frontend

React TypeScript frontend for the AI-powered chatbot with Firebase authentication and modern UI components.

## 🚀 Quick Start

```bash
# Install dependencies
npm install

# Set environment variables
cp .env.example .env
# Edit .env with your Firebase configuration

# Start development server
npm run dev
```

## 🔧 Environment Variables

Create `.env` file:
```env
VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_PROJECT_ID=your_firebase_project_id  
VITE_FIREBASE_APP_ID=your_firebase_app_id
VITE_API_BASE_URL=http://localhost:8000
```

## 📁 Project Structure

```
src/
├── components/          # React components
│   ├── ui/             # shadcn/ui components
│   ├── ChatInterface.tsx
│   ├── Sidebar.tsx
│   └── AuthModal.tsx
├── pages/              # Page components
├── hooks/              # Custom React hooks
├── lib/                # Utilities and configuration
└── App.tsx            # Main application component
```

## 🎨 Features

- **Modern UI**: Built with Tailwind CSS and shadcn/ui
- **Dark Mode**: Toggle between light and dark themes
- **Responsive Design**: Mobile-first approach with WCAG compliance
- **Type Animations**: Enhanced chat experience with react-type-animation
- **Firebase Auth**: Google and GitHub OAuth integration
- **Real-time Chat**: Instant messaging with typing indicators

## 🔐 Authentication

Firebase authentication with multiple providers:
- Google OAuth
- GitHub OAuth
- Demo mode for development

## 📱 Responsive Design

- Mobile-first responsive design
- Accessible components following WCAG guidelines
- Touch-friendly interface for mobile devices
- Optimized for all screen sizes

## 🛠️ Development

```bash
# Development server
npm run dev

# Type checking
npm run type-check

# Build for production
npm run build

# Preview production build
npm run preview
```

## 🚀 Deployment

### Netlify Deployment

1. **Connect Repository**
   - Import from Git in Netlify dashboard

2. **Build Settings**
   ```yaml
   Build command: npm run build
   Publish directory: dist
   ```

3. **Environment Variables**
   - Add all VITE_ prefixed variables

### Vercel Deployment

1. **Import Project**
   - Connect GitHub repository

2. **Configure**
   ```yaml
   Framework: Vite
   Build Command: npm run build
   Output Directory: dist
   ```

## 🧪 Testing

```bash
# Run tests
npm run test

# Coverage report
npm run test:coverage
```

## 📦 Dependencies

### Core
- React 18 with TypeScript
- Vite for build tooling
- Tailwind CSS for styling

### UI Components
- shadcn/ui component library
- Radix UI primitives
- Lucide React icons

### Authentication
- Firebase SDK
- React hooks for auth state

### State Management
- TanStack Query for server state
- React hooks for local state

## 🎯 API Integration

Connects to FastAPI backend:
- Base URL: `VITE_API_BASE_URL`
- Authentication: Firebase JWT tokens
- Endpoints: `/api/chat`, `/api/chats`

## 📱 Accessibility

WCAG 2.1 AA compliant features:
- Semantic HTML structure
- Keyboard navigation support
- Screen reader compatibility
- Color contrast compliance
- Focus management

## 🔧 Configuration

### Tailwind CSS
Custom theme configuration in `tailwind.config.ts`

### TypeScript
Strict type checking enabled

### Vite
Optimized build configuration for production

This frontend provides a modern, accessible, and responsive chat interface that seamlessly integrates with the FastAPI backend.