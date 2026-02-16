# Phanta

**AI-Powered Blockchain Portfolio Management Platform**

Phanta is a next-generation portfolio management platform that leverages on-chain data, Solana Program Derived Addresses (PDAs), and Google Gemini AI to provide intelligent portfolio analysis, risk assessment, and automated insights. Built entirely on blockchain infrastructure, Phanta brings the power of decentralized finance to portfolio management.

Won Badger Build Fest 2025
Dev Post : https://devpost.com/software/phanta

## Features

-   **On-Chain Portfolio Tracking**: Real-time balances and transaction history directly from Solana.
-   **Decentralized Groups**: Create and join groups using Solana PDAs with on-chain state management.
-   **AI Insights**: Google Gemini-powered portfolio analysis, risk assessment, and trading recommendations.
-   **Market Intelligence**: Real-time token prices and volatility analysis via Jupiter and Helius APIs.

## Tech Stack

-   **Frontend**: React, Vite, Tailwind CSS
-   **Backend**: Node.js, Express, SQLite
-   **Blockchain**: Solana Web3.js, Anchor Framework
-   **AI**: Google Gemini API

## Project Structure

```
Phanta/
├── backend/
│   ├── routes/          # API routes
│   ├── services/        # Blockchain & AI services
│   ├── programs/        # Solana programs (Anchor)
│   └── database.js      # SQLite setup
├── frontend/
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── services/    # API clients
│   │   └── hooks/       # Custom React hooks
└── README.md
```

## Getting Started

### Prerequisites

-   Node.js 18+
-   Phantom Wallet
-   Google Gemini API Key

### Installation

1.  **Clone & Install**

    ```bash
    git clone https://github.com/YOUR_GITHUB_USERNAME/Phanta.git
    cd Phanta
    
    # Install Backend
    cd backend && npm install
    
    # Install Frontend
    cd ../frontend && npm install
    ```

2.  **Setup Environment**

    Create `backend/.env`:
    ```env
    GEMINI_API_KEY=your_key
    HELIUS_API_KEY=optional_key
    PORT=3001
    ```

3.  **Run**

    ```bash
    # Backend (Terminal 1)
    cd backend && npm start
    
    # Frontend (Terminal 2)
    cd frontend && npm run dev
    ```

    Open: http://localhost:5173

## License

MIT License
