# Phanta

**AI-Powered Blockchain Portfolio Management Platform**

Phanta is a next-generation blockchain-native portfolio management platform that leverages on-chain data, Solana Program Derived Addresses (PDAs), and Google Gemini AI to provide intelligent portfolio analysis, risk assessment, and automated insights. Built entirely on blockchain infrastructure, Phanta brings the power of decentralized finance to portfolio management.

Won Badger Build Fest 2025. https://devpost.com/software/phanta?ref_content=my-projects-tab&ref_feature=my_projects

## Blockchain-First Architecture

Phanta is built entirely on blockchain infrastructure - every feature leverages the power of decentralized technology:

- **Solana Blockchain**: All portfolio data is fetched directly from on-chain sources
- **Program Derived Addresses (PDAs)**: Group functionality uses Solana PDAs for decentralized state management
- **On-Chain Data**: Real-time wallet balances, token holdings, and transaction history from the Solana blockchain
- **Smart Contract Integration**: Group deposits and membership tracked on-chain via Solana programs
- **Decentralized State**: Group accounts stored as PDAs, ensuring transparency and immutability

## Core Blockchain Features

### On-Chain Portfolio Tracking
- Real-time balance fetching from Solana RPC endpoints
- Token account analysis using Solana's Token Program
- Transaction history directly from blockchain signatures
- Multi-RPC endpoint support for reliability

### Solana Program Integration
- **Group Management**: Create and join groups with on-chain state
- **PDA Accounts**: Group data stored in Program Derived Addresses
- **Deposit Tracking**: Member deposits tracked on-chain
- **Majority Voting**: On-chain logic for group decisions

### Blockchain Data Sources
- **Helius API**: Enhanced Solana wallet indexing
- **Jupiter API**: Real-time token prices from on-chain DEX aggregators
- **Solana RPC**: Direct blockchain queries for balances and transactions
- **CoinGecko**: Market data for cryptocurrency assets

## AI-Powered Insights

Powered by Google Gemini, Phanta provides:

- **Portfolio Analysis**: AI-driven analysis of your on-chain holdings
- **Risk Assessment**: Intelligent risk scoring based on blockchain data
- **Trading Recommendations**: Data-driven suggestions for portfolio optimization
- **Group Chat AI**: Collaborative decision-making with AI assistance via `@gemini` mentions

## Technical Stack

### Blockchain Layer
- **Solana Web3.js**: Direct blockchain interaction
- **Anchor Framework**: Solana program development
- **Phantom Wallet**: Native Solana wallet integration
- **RPC Endpoints**: Multiple Solana RPC providers for redundancy

### Frontend
- **React.js**: Modern UI framework
- **Vite**: Fast build tool
- **Tailwind CSS**: Utility-first styling
- **Chart.js**: Data visualization

### Backend
- **Node.js/Express**: API server
- **SQLite**: Off-chain metadata storage
- **Google Gemini API**: AI-powered insights
- **Axios**: HTTP client for blockchain APIs

## Getting Started

### Prerequisites
- Node.js 18+ and npm
- Phantom wallet browser extension
- Google Gemini API key (for AI features)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_GITHUB_USERNAME/Phanta.git
   cd Phanta
   ```

2. **Install dependencies**
   ```bash
   # Backend
   cd backend
   npm install
   
   # Frontend
   cd ../frontend
   npm install
   ```

3. **Configure environment variables**
   
   Create `backend/.env`:
   ```env
   GEMINI_API_KEY=your_gemini_api_key_here
   HELIUS_API_KEY=your_helius_key_optional
   PORT=3001
   ```

4. **Start the servers**
   ```bash
   # Terminal 1: Backend
   cd backend
   npm start
   
   # Terminal 2: Frontend
   cd frontend
   npm run dev
   ```

5. **Connect your Phantom wallet**
   - Open http://localhost:5173
   - Click "Connect Phantom Wallet"
   - Approve the connection in Phantom

## Features

### Portfolio Dashboard
- **Real-Time Balances**: Live SOL and SPL token balances from blockchain
- **On-Chain Holdings**: All tokens tracked directly from your wallet
- **Transaction History**: Complete on-chain transaction feed
- **24h PnL**: Calculated from blockchain price data

### Group Management (On-Chain)
- **Create Groups**: Initialize Solana PDA accounts for groups
- **Join Groups**: Deposit SOL/SPL tokens to join groups
- **On-Chain State**: All group data stored in blockchain accounts
- **Majority Logic**: Blockchain-enforced group decision rules

### AI Assistant
- **Portfolio Analysis**: Gemini AI analyzes your on-chain portfolio
- **Risk Warnings**: AI identifies potential risks in holdings
- **Optimization Suggestions**: Data-driven recommendations
- **Group Chat**: AI-powered group discussions

### Market Intelligence
- **Crypto Analytics**: Market data and volatility analysis
- **Correlation Matrices**: Asset correlation from blockchain data
- **Regression Analysis**: Statistical analysis of price movements

## Security

- **Wallet Integration**: Direct connection to Phantom wallet
- **No Private Keys**: Private keys never leave your wallet
- **On-Chain Verification**: All transactions verified on Solana blockchain
- **Transparent State**: Group data publicly verifiable on-chain

## Development

### Project Structure
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

### Solana Program Development

The group functionality uses Solana programs:

```rust
// programs/phanta-groups/src/lib.rs
// GroupAccount PDA structure
pub struct GroupAccount {
    pub owner: Pubkey,
    pub members: Vec<Pubkey>,
    pub required_deposit: u64,
    pub total_deposited: u64,
    pub member_count: u8,
    pub status: bool,
}
```

### Blockchain Data Flow

1. **Wallet Connection**: Phantom wallet connects via Solana Web3.js
2. **RPC Queries**: Fetch balances, tokens, transactions from Solana RPC
3. **On-Chain State**: Read group PDAs from blockchain
4. **AI Analysis**: Gemini analyzes on-chain portfolio data
5. **User Interface**: Display blockchain data in modern UI

## Key Differentiators

- **100% Blockchain-Native**: All data sourced from on-chain sources
- **Solana-First**: Built specifically for Solana blockchain
- **PDA-Based Groups**: Decentralized group management
- **Real-Time On-Chain Data**: Live blockchain state updates
- **AI + Blockchain**: Combines AI intelligence with blockchain transparency

## License

MIT License - see LICENSE file for details

## Links

- **GitHub**: https://github.com/YOUR_GITHUB_USERNAME/Phanta
- **Solana Docs**: https://docs.solana.com
- **Phantom Wallet**: https://phantom.app
- **Google Gemini**: https://ai.google.dev

## Acknowledgments

- Solana Foundation for blockchain infrastructure
- Phantom for wallet integration
- Google for Gemini AI
- Helius and Jupiter for blockchain data APIs

1. **Wallet Connection**: Phantom wallet connects via Solana Web3.js
2. **RPC Queries**: Fetch balances, tokens, transactions from Solana RPC
3. **On-Chain State**: Read group PDAs from blockchain
4. **AI Analysis**: Gemini analyzes on-chain portfolio data
5. **User Interface**: Display blockchain data in modern UI

**Built on Solana. Powered by AI. Managed by You.**

---