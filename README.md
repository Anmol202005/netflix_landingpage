# CaveVerse

A real-time multiplayer 2D virtual world where users can explore, interact, and communicate with others in a shared digital space.

## Features

- **Real-time Multiplayer**: Walk around and interact with other players in real-time
- **Voice & Video Chat**: Peer-to-peer audio/video communication and screen sharing
- **Interactive Chat System**: Text-based messaging with other users
- **2D Game World**: Smooth character movement and exploration
- **Modern UI**: Clean, responsive interface with smooth animations
- **Cross-platform**: Works on desktop and mobile browsers

## Technology Stack

### Frontend
- **React 18** - Modern UI framework
- **TypeScript** - Type-safe development
- **Vite** - Fast build tool and development server
- **Phaser 3** - 2D game engine for character movement and world rendering
- **TailwindCSS** - Utility-first CSS framework
- **ShadCN/UI** - High-quality component library
- **Motion** - Smooth animations and transitions
- **Redux Toolkit** - State management

### Backend
- **Node.js** - JavaScript runtime
- **Colyseus** - Multiplayer game server framework
- **Express** - Web application framework
- **TypeScript** - Type-safe server development

### Real-time Communication
- **Colyseus** - Server-side multiplayer state synchronization
- **PeerJS** - Client-side peer-to-peer video/audio communication

## Project Structure

```
├── client/          # React frontend application
│   ├── src/         # Source code
│   ├── public/      # Static assets
│   └── package.json # Frontend dependencies
├── server/          # Colyseus game server
│   ├── src/         # Server source code
│   ├── build/       # Compiled server code
│   └── package.json # Server dependencies
└── README.md        # Project documentation
```

## Getting Started

### Prerequisites
- Node.js 16.13.0 or higher
- npm or yarn package manager

### Installation

1. Clone the repository
```bash
git clone <repository-url>
cd CaveVerse
```

2. Install server dependencies
```bash
cd server
npm install
```

3. Install client dependencies
```bash
cd ../client
npm install
```

### Development

1. Start the game server
```bash
cd server
npm run dev
```
The server will start on `http://localhost:2567`

2. Start the client development server
```bash
cd client
npm run dev
```
The client will start on `http://localhost:5173`

3. Open your browser and navigate to the client URL to start playing

### Building for Production

#### Server
```bash
cd server
npm run build
npm start
```

#### Client
```bash
cd client
npm run build
```

The built files will be in the `client/dist` directory, ready for deployment to any static hosting service.

## Deployment

### Recommended Hosting Options

**Frontend (Static Site)**
- Vercel
- Netlify
- GitHub Pages
- Cloudflare Pages

**Backend (Node.js Server)**
- Railway
- Render
- Heroku
- DigitalOcean App Platform

### Environment Configuration

Ensure your client connects to the correct server URL in production by updating the Colyseus connection configuration.

## Development Features

- Hot reload for both client and server during development
- TypeScript support with full type checking
- ESLint configuration for code quality
- Optimized build process with Vite

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the UNLICENSED license.

## Support

For issues and questions, please open an issue in the repository's issue tracker.