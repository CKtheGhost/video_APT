# DeFi Headquarters (HQ)

![DeFi Headquarters Logo](https://raw.githubusercontent.com/CKtheGhost/logosvg/main/Prospera%20(1).svg)

## AI-Powered DeFi Aggregator and Yield Optimizer for Aptos

DeFi Headquarters is a comprehensive platform for Aptos blockchain users that combines real-time market data, portfolio analysis, and AI-driven recommendations to optimize DeFi investments. The platform offers automatic portfolio rebalancing and one-click execution of complex investment strategies.

## 🚀 Features

### Core Functionality
- **Protocol Aggregation**: Integrated with major Aptos DeFi protocols including Amnis, Thala, Tortuga, Ditto, Pancakeswap, and more
- **AI-Powered Recommendations**: Claude 3.5 Sonnet integration for personalized investment strategies
- **Portfolio Analysis**: Real-time tracking of APT holdings, staked tokens, and liquidity positions
- **One-Click Strategy Execution**: Execute complex multi-protocol strategies with a single click
- **Auto-Portfolio Balancer**: Set and forget with 24-hour automatic portfolio rebalancing

### Additional Features
- **Real-time Market Data**: Latest APR rates, token prices, and protocol comparisons
- **Risk Profile Customization**: Choose from conservative, balanced, or aggressive investment approaches
- **Visual Portfolio Analytics**: Interactive charts for asset allocation and performance tracking
- **Crypto News Integration**: Latest updates from the Aptos ecosystem
- **Matrix Animation UI**: Sleek, cyberpunk-inspired interface

## 📊 Dashboard Sections

- **Market Overview**: General market data, trends, and sentiment analysis
- **Protocol Comparison**: Side-by-side comparison of APRs across different protocols
- **Portfolio Analysis**: Detailed breakdown of wallet holdings with visualization
- **AI Recommendations**: Personalized investment strategies tailored to your portfolio and risk profile
- **News Feed**: Latest updates from the Aptos ecosystem

## 🔧 Technical Architecture

### Frontend
- Node.js with Express server
- EJS templates with Tailwind CSS
- Chart.js for data visualization
- Custom matrix animation effects

### Backend
- Aptos Blockchain integration via `@aptos-labs/ts-sdk`
- AI models: Claude 3.5 Sonnet (Anthropic) with OpenAI fallback
- Move Agent Kit for transaction execution
- In-memory caching for performance optimization

### Key Modules
- **staking_optimizer.js**: Protocol rate tracking and recommendation generation
- **portfolio_tracker.js**: Wallet analysis and performance monitoring
- **defi-transaction-manager.js**: Handles all blockchain transactions
- **chart-utilities.js**: Data visualization components
- **defi-auto-rebalancer.js**: Automated portfolio adjustment

## 🔍 How It Works

1. **Data Aggregation**: The platform continuously fetches current APR rates, token prices, and market data from multiple Aptos protocols.

2. **Portfolio Analysis**: When a user connects their wallet, DeFi HQ analyzes their holdings, staking positions, and liquidity pools.

3. **AI Strategy Generation**: Based on the user's risk profile and current market conditions, the AI generates personalized investment strategies optimized for maximum yield.

4. **Strategy Execution**: Users can execute recommended strategies with a single click. The transaction manager handles all the complex operations (unstaking, swapping, providing liquidity, etc.).

5. **Auto-Optimization**: When enabled, the platform automatically rebalances the user's portfolio every 24 hours to adapt to changing market conditions.

## 🔌 Supported Protocols

### Liquid Staking
- Amnis (stAPT)
- Thala (sthAPT)
- Tortuga (tAPT)
- Ditto (dAPT)

### Lending/Borrowing
- Aries
- Echo
- Echelon
- Abel
- Joule

### DEXes and AMMs
- Pancakeswap
- Liquidswap
- Cetus
- Sushi
- Aux
- Pontem

### Yield Optimizers
- Merkle
- Fetch

### Stablecoin and Minting
- Thala Stablecoin
- Momento

## 🛠️ Installation and Setup

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Aptos CLI (optional)

### Environment Variables
Create a `.env` file with the following variables:
```
PORT=3000
APTOS_NETWORK=MAINNET
APTOS_PRIVATE_KEY=your_private_key
ANTHROPIC_API_KEY=your_anthropic_key
OPENAI_API_KEY=your_openai_key_as_fallback
```

### Installation Steps
1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/defi-headquarters.git
   cd defi-headquarters
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Start the development server
   ```bash
   npm run dev
   ```

4. For production
   ```bash
   npm run build
   npm start
   ```

## 🔐 Security Notes

- Private keys are only used server-side and never exposed to the client
- All sensitive operations use rate limiting and error handling
- For production use, implement proper key management and wallet connection security
- Consider adding 2FA for high-value operations

## 📝 License

[MIT License](LICENSE)

## 🙏 Acknowledgements

- Aptos Labs for the blockchain infrastructure
- Anthropic for Claude AI integration
- Move Agent Kit contributors
- All the Aptos DeFi protocols supported in this platform

---

Developed with ♥ for the Aptos ecosystem
