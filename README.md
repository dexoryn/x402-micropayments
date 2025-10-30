# x402 Micropayments

A movie streaming platform powered by x402 micropayments for secure, instant, and seamless payments. Users can pay and watch movies directly through the x402 payment gateway, while the backend handles API interactions for reliable transaction processing and subscription management on Base.

## Features

### Backend
 - Express.js server with x402 payment middleware
 - Paywalled endpoints for premium video content
 - Secure payment verification
 - Integrated with Base Sepolia testnet for easy testing

### Frontend
- Modern UI & Smooth Animations – Professional gradient design
- Responsive Landing Page – Hero section, feature cards, and "How It Works" guide
- Payment Processing Page – Real-time status with animated loader
- Premium Content Page – Clean video player interface with payment confirmation
- Consistent Navigation – Navbar with x402 branding and quick links
- Professional Footer – Social links, navigation, and resources
- Font Awesome Icons – Visual enhancements throughout
- SEO Optimized – Meta tags for OpenGraph & Twitter Cards
- Favicon Support – Custom branding with SVG favicon

## Prerequisites

- Node.js (v22 or higher)
- A EVM-compatible wallet with Base Sepolia USDC

## Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/dexoryn/x402-micropayments.git
   cd x402-micropayments
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3.Set environment variables: Rename .env.local to .env and update:

   ```
   WALLET_ADDRESS=your_ethereum_wallet_address
   NODE_ENV=development
   PORT=402
   ```

4. Get Base Sepolia USDC for testing:
   - Visit https://faucet.circle.com/
   - Select Base Sepolia and request test USDC
   - Request test USDC

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open your browser and navigate to `http://localhost:4021`

## How It Works

1. The server uses the `x402-express` middleware to protect the `/authenticate` endpoint
2. Users must complete a payment to access protected content.
3. Upon successful payment, users are redirected to /video-content to watch premium videos.
   
## Demo
[Demo website](https://x402-micropayments.vercel.app/)

## Customizing

- Video price: Update the `price` parameter in `api/index.js`
- Video content: Replace the video source in `public/video-content.html`
- Mainnet deployment: Update the network configuration in `api/index.js` and use proper CDP API keys
  
## 📞 Contact 

### Telegram: [dexoryn](https://t.me/dexoryn_me)

## 🍵 Tip

### If you like this project, ⭐ star or 🔗 fork it to support development!
