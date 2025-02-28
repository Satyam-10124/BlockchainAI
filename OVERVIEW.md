# 🎲 Aptos AI Roulette - Technical Overview

## Project Overview
Aptos AI Roulette is an innovative blockchain-based roulette game that combines the security and transparency of the Aptos blockchain with cutting-edge AI technology. The game features a unique AI virtual host powered by Google's Gemini API, providing an immersive and interactive gaming experience.

## Architecture

### 1. Smart Contract (Move)
The game's core logic is implemented in Move, Aptos's native programming language. Key features include:
- **Game State Management**: Tracks house balance, game status, and events
- **Betting System**:
  - Minimum bet: 0.01 APT
  - Numbers range: 0-36
  - Provably fair outcomes using Aptos's random number generation
- **Event System**: Records bet placements and spin results on-chain
- **Security Features**: Input validation, balance checks, and pause functionality

### 2. Frontend (React.js + Tailwind CSS)
The user interface is built with modern web technologies:
- Responsive design optimized for all devices
- Real-time game updates and animations
- Wallet integration (Petra & Martian)
- Interactive betting interface
- Real-time voice interactions

### 3. Backend Integration
- **AI Integration**: Google Gemini API for the virtual host
- **Voice Synthesis**: ElevenLabs API for realistic voice interactions
- **WebSocket**: Real-time game state updates

## Game Flow

1. **Wallet Connection**
   - Players connect using either Petra or Martian wallet
   - Account balance verification

2. **Betting Phase**
   - Player selects a number (0-36)
   - Places bet (minimum 0.01 APT)
   - Bet is recorded on-chain via smart contract

3. **Game Execution**
   - Random number generation using Aptos's secure RNG
   - Smart contract validates and processes the outcome
   - Results are recorded as blockchain events

4. **AI Host Interaction**
   - Virtual host provides real-time commentary
   - Voice synthesis for immersive experience
   - Dynamic responses based on game events

## Technical Components

### Smart Contract Functions
- `initialize_game`: Sets up initial game state
- `place_bet`: Processes player bets
- `spin_wheel`: Generates random outcome
- `payout_winners`: Handles prize distribution

### Security Measures
- Audited smart contract
- Secure random number generation
- Protected API endpoints
- Wallet security integration
- Input validation and error handling

### AI Integration
- Real-time natural language processing
- Context-aware responses
- Voice synthesis for immersive experience

## Future Enhancements
1. Multi-token support
2. Multiplayer rooms
3. Tournament mode
4. Enhanced AI interactions
5. Additional betting options

## Dependencies
- Aptos Framework
- React.js
- Tailwind CSS
- Google Gemini API
- ElevenLabs API
- Web3 wallet connectors