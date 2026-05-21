# Universal Music Learning App

An AI-powered music learning platform that allows users to learn any instrument by importing songs from Spotify.

## Features

- 🎵 **Import Songs from Spotify** - Paste a Spotify link and the app analyzes the song
- 🎸 **Multi-Instrument Support** - Learn guitar, piano, drums, trumpet, violin, and more
- 🤖 **AI-Generated Arrangements** - Automatically generates playable parts for any instrument
- 📄 **Interactive Sheet Music** - Real-time synchronized sheet music with instrument-specific guides
- 🎮 **Play Along Mode** - Practice with adjustable speed and looping
- 📊 **Progress Tracking** - Monitor your improvement across instruments
- 🎓 **Learning Modes** - Beginner, Intermediate, and Advanced difficulty levels

## Tech Stack

### Frontend
- Next.js 14+ (React)
- TailwindCSS + Shadcn/ui
- Tone.js (audio playback)
- VexFlow (sheet music rendering)
- TypeScript

### Backend
- FastAPI (Python) - Audio processing
- Node.js - API gateway
- PostgreSQL - Database
- Redis - Caching

### AI/ML
- OpenAI API - Arrangement generation
- librosa/madmom - Audio analysis
- Transformers.js - In-browser inference

## Project Structure

```
universal-music-learning-app/
├── frontend/                 # Next.js web application
├── backend/                  # FastAPI Python service
├── shared/                   # Shared types and utilities
├── docker-compose.yml        # Local development setup
└── README.md
```

## Getting Started

### Prerequisites
- Node.js 18+
- Python 3.10+
- Docker & Docker Compose
- Spotify Developer Account

### Installation

1. Clone the repository:
```bash
git clone https://github.com/carterfrancom88/universal-music-learning-app.git
cd universal-music-learning-app
```

2. Set up environment variables:
```bash
cp .env.example .env.local
```

3. Install dependencies:
```bash
cd frontend && npm install
cd ../backend && pip install -r requirements.txt
```

4. Start the development environment:
```bash
docker-compose up -d
```

5. Access the app:
- Frontend: http://localhost:3000
- Backend API: http://localhost:8000

## Roadmap

### Phase 1: MVP (Months 1-3)
- [ ] User authentication (Spotify OAuth)
- [ ] Spotify song import
- [ ] Guitar & Piano support
- [ ] Basic audio analysis
- [ ] Sheet music rendering
- [ ] Simple playalong mode

### Phase 2: Enhanced Learning (Months 4-6)
- [ ] 4+ additional instruments
- [ ] ML-based arrangement generation
- [ ] Difficulty modes
- [ ] Real-time performance feedback
- [ ] Gamification features

### Phase 3: Scale & Polish (Months 7-12)
- [ ] Mobile app (React Native)
- [ ] Advanced AI features
- [ ] Social features
- [ ] Premium monetization

## License

MIT

## Contact

For questions or suggestions, open an issue on GitHub.
