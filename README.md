# Instagram Clone - Frontend

A modern, high-performance Instagram clone frontend built with Next.js 15, React 19, and TypeScript. This application demonstrates advanced frontend development practices including server-side rendering, real-time communication, state management, and performance optimization.

## 🚀 Key Features

- **Next.js 15 App Router**: Leveraging the latest Next.js features with server components and streaming
- **React 19**: Using the latest React features and concurrent rendering
- **Real-time Communication**: Socket.io integration for instant messaging and notifications
- **Video Calls**: Peer-to-peer video calling with PeerJS
- **Performance Optimized**: Virtual scrolling, lazy loading, code splitting, and image optimization
- **TypeScript**: Full type safety throughout the application
- **Modern UI/UX**: Responsive design with TailwindCSS, Framer Motion animations, and intuitive user interface
- **State Management**: Redux Toolkit for global state and Zustand for local state
- **Server-Side Rendering**: Optimized SSR and SSG for better SEO and performance

## 🛠 Technology Stack

### Core Framework
- **Next.js 15.3.1** - React framework with App Router
- **React 19.0.0** - Latest React with concurrent features
- **TypeScript 5** - Type-safe development

### State Management
- **Redux Toolkit 2.8.2** - Predictable state container
- **Zustand 5.0.5** - Lightweight state management
- **SWR 2.3.3** - Data fetching and caching

### Styling & UI
- **TailwindCSS 4** - Utility-first CSS framework
- **SCSS** - Enhanced CSS with variables and mixins
- **Framer Motion 12.16.0** - Production-ready motion library
- **Lucide React** - Beautiful icon library
- **React Icons** - Popular icon library

### Real-time & Communication
- **Socket.io Client 4.8.1** - Real-time bidirectional communication
- **PeerJS 1.5.4** - WebRTC peer-to-peer connections

### Performance & Optimization
- **React Window 1.8.11** - Virtual scrolling for large lists
- **React Window Infinite Loader** - Infinite scrolling optimization
- **Next.js Bundle Analyzer** - Bundle size optimization
- **NProgress** - Loading progress indicator

### Media Handling
- **CropperJS** - Image cropping functionality
- **React Cropper** - React wrapper for CropperJS
- **React Easy Crop** - Image cropping component
- **Swiper 11.2.8** - Modern touch slider

### Utilities
- **Day.js** - Lightweight date library
- **React OAuth Google** - Google authentication

## 📁 Project Structure

```
front-end/
├── src/
│   ├── app/                    # Next.js App Router pages
│   │   ├── (CheckAuth)/       # Authentication routes
│   │   ├── (Layout)/          # Main application layout
│   │   ├── hooks/             # Custom React hooks
│   │   ├── ui/                # UI components and pages
│   │   └── globals.css        # Global styles
│   ├── components/            # Reusable React components
│   │   ├── Messenger/         # Real-time messaging components
│   │   ├── Modal/             # Modal components
│   │   ├── Story/             # Story features
│   │   └── ...                # Other feature components
│   ├── contexts/              # React Context providers
│   │   ├── CallContext.tsx    # Video call context
│   │   ├── GlobalContext.tsx  # Global app context
│   │   ├── PostContext.tsx    # Post management context
│   │   └── UserContext.tsx    # User context
│   ├── store/                 # Redux store configuration
│   │   ├── index.tsx          # Store setup
│   │   ├── messengerSlice.ts  # Messenger state
│   │   └── post.ts            # Post state
│   ├── server/                # Server-side utilities
│   │   ├── auth.tsx           # Authentication utilities
│   │   ├── socket.tsx         # Socket.io client setup
│   │   └── ...                # API utilities
│   ├── types/                 # TypeScript type definitions
│   ├── utils/                 # Utility functions
│   └── styles/                # SCSS variables and mixins
└── public/                    # Static assets
```

## 🏗 Architecture & Design Patterns

### Component Architecture
- **Component Composition**: Reusable, composable components
- **Custom Hooks**: Encapsulated business logic in custom hooks
- **Context API**: Shared state management for related components
- **Server Components**: Leveraging Next.js server components for optimal performance

### State Management Strategy
- **Redux Toolkit**: Global application state (posts, user data, messenger)
- **Zustand**: Local component state and UI state
- **SWR**: Server state management with automatic caching and revalidation
- **React Context**: Shared state for related component trees

### Performance Optimization
- **Virtual Scrolling**: Using react-window for large lists (posts, messages)
- **Code Splitting**: Automatic code splitting with Next.js
- **Image Optimization**: Next.js Image component with lazy loading
- **Bundle Optimization**: Tree shaking and bundle analysis
- **Memoization**: React.memo and useMemo for expensive computations

### Real-time Features
- **Socket.io Integration**: Real-time messaging, notifications, and updates
- **WebRTC**: Peer-to-peer video calls with PeerJS
- **Optimistic Updates**: Immediate UI updates with server sync

## 🚀 Getting Started

### Prerequisites

- Node.js 18.x or higher
- npm, yarn, or pnpm
- Git

### Installation

```bash
# Clone the repository
git clone git@github.com:vanloc19/InstagramClone_Front-End.git
cd InstagramClone_Front-End

# Install dependencies
npm install

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Environment Variables

Create a `.env.local` file in the root directory:

```env
NEXT_PUBLIC_API_URL=http://localhost:5000
NEXT_PUBLIC_SOCKET_URL=http://localhost:5000
NEXT_PUBLIC_GOOGLE_CLIENT_ID=your_google_client_id
NEXT_PUBLIC_PEER_HOST=your_peer_host
NEXT_PUBLIC_PEER_PORT=443
```

## 📜 Available Scripts

```bash
# Development server with Turbopack
npm run dev

# Production build
npm run build

# Start production server
npm start

# Lint code
npm run lint
```

## 🎨 Key Features Implementation

### Real-time Messaging
- Socket.io integration for instant messaging
- Message threading and replies
- File and media sharing
- Online/offline status indicators
- Read receipts and typing indicators

### Video Calls
- Peer-to-peer video calls using WebRTC
- Call management and UI
- Screen sharing capabilities
- Call history and management

### Posts & Stories
- Create, edit, and delete posts
- Image and video uploads
- Story creation with music
- Interactive comments and likes
- Post virtualization for performance

### User Experience
- Responsive design for all devices
- Smooth animations with Framer Motion
- Loading states and skeletons
- Error handling and user feedback
- Accessibility considerations

## 🔒 Security Features

- JWT token authentication
- Protected routes with middleware
- Secure cookie handling
- XSS prevention
- CSRF protection
- Input validation and sanitization

## 📈 Performance Metrics

- **Lighthouse Score**: Optimized for 90+ performance score
- **First Contentful Paint**: < 1.5s
- **Time to Interactive**: < 3s
- **Bundle Size**: Optimized with code splitting
- **Image Optimization**: Automatic image optimization with Next.js

## 🧪 Best Practices

- **TypeScript**: Full type safety
- **ESLint**: Code quality and consistency
- **Component Testing**: Reusable and testable components
- **Error Boundaries**: Graceful error handling
- **Loading States**: Proper loading and error states
- **Accessibility**: WCAG compliance considerations

## 📦 Build & Deployment

### Production Build

```bash
npm run build
npm start
```

### Deployment Options

- **Vercel**: Recommended for Next.js applications
- **Netlify**: Alternative deployment platform
- **Docker**: Containerized deployment
- **Self-hosted**: Custom server deployment

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Copyright © 2025 vanloc19. All rights reserved.

## 👤 Author

**vanloc19**

- 📧 Email: [tovanloc19@gmail.com](mailto:tovanloc19@gmail.com)
- 📘 Facebook: [vanloc1963](https://www.facebook.com/vanloc1963/)
- 💻 GitHub: [@vanloc19](https://github.com/vanloc19)

---

Built with ❤️ using Next.js, React, and TypeScript
