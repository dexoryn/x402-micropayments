# x402 Micropayments

This project is a movie streaming platform integrated with x402 for secure and seamless payments. Users can pay and watch movies directly through the x402 payment gateway. The backend handles x402 API interactions, ensuring reliable transaction processing and subscription management using x402 services.

## Features

### Backend
- Simple Express.js server with x402 payment middleware
- Paywalled endpoint for accessing premium video content
- Secure payment processing and verification
- Base Sepolia testnet integration for easy testing

### Frontend
- **Modern, Professional UI** - Beautiful gradient design with smooth animations
- **Responsive Landing Page** - Hero section with feature cards and "How It Works" guide
- **Payment Processing Page** - Real-time status indicators with animated loader
- **Premium Content Page** - Clean video player interface with payment confirmation
- **Consistent Navigation** - Navbar with x402 branding and quick links across all pages
- **Professional Footer** - Social links, quick navigation, and resource links
- **Font Awesome Icons** - Enhanced visual design throughout the interface
- **SEO Optimized** - Complete meta tags for social sharing (OpenGraph, Twitter Cards)
- **Favicon Support** - Custom branding with SVG favicon

## Prerequisites

- Node.js (v22 or higher)
- A EVM-compatible wallet with Base Sepolia USDC

## Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/enlomy/x402-micropayments.git
   cd x402-micropayments
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Rename `.env.local` to `.env` and add the following variables (remember to replace `WALLET_ADDRESS` with your actual wallet address you want to receive payments for)

   ```
   WALLET_ADDRESS=your_ethereum_wallet_address
   NODE_ENV=development
   PORT=402
   ```

4. Get Base Sepolia USDC for testing:
   - Visit https://faucet.circle.com/
   - Select Base Sepolia in the network dropdown
   - Request test USDC

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open your browser and navigate to `http://localhost:402`

## How It Works

1. The server uses the `x402-express` middleware to protect the `/authenticate` endpoint
2. When a user tries to access the protected endpoint, they are required to make a payment
3. After successful payment, the user is redirected to `/video-content`, where the premium video content is served

## Demo
[Demo website](https://x402.enlomy.xyz/)

## Customizing

- To change the price of the video, modify the `price` parameter in `api/index.js`
- To use a different video, update the video source in `public/video-content.html`
- To deploy on Base mainnet, update the network configuration in `api/index.js` (you will need also need CDP API Keys and need to use a different Facilitator)

## 📞 Contact Info

### Telegram: [enlomy](https://t.me/enlomy)

## 🍵 Tip

### If you are interested in my projects, please 🔗fork or give me ⭐star
