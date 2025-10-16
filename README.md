# DumpClub - Digital Products Marketplace

A modern, responsive e-commerce platform for digital products with cryptocurrency payment integration.

## 📁 File Structure

```
Dumpclub/
├── Home.html              # Main shop page
├── payment.html           # Payment/checkout page
├── Crypto QR/            # QR code images for crypto payments
│   ├── bitcoin-qr.png    # Bitcoin wallet QR code
│   ├── ethereum-qr.png   # Ethereum wallet QR code
│   ├── solana-qr.png     # Solana wallet QR code
│   └── litecoin-qr.png   # Litecoin wallet QR code (optional)
└── README.md             # This file
```

## 🚀 Setup Instructions

### 1. Add Your QR Codes

Place your cryptocurrency wallet QR code images in the `Crypto QR/` folder with these exact names:

- `bitcoin-qr.png` - Your Bitcoin wallet QR code
- `solana-qr.png` - Your Solana wallet QR code (from https://i.ibb.co/RTGKHzVw/hovercode-2.png)
- `ethereum-qr.png` - Your Ethereum wallet QR code (from https://i.ibb.co/gFbqwyWJ/hovercode-3.png)
- `litecoin-qr.png` - Your Litecoin wallet QR code (optional)

### 2. Update Telegram Link

In `Home.html`, find this line and update with your actual Telegram channel:

```html
<a href="https://t.me/yourtelegramchannel" target="_blank">
```

### 3. Update Crypto Addresses

In `payment.html`, update the wallet addresses (around line 1987):

```javascript
const cryptoData = {
    btc: {
        address: 'YOUR_BITCOIN_ADDRESS',
        // ...
    },
    eth: {
        address: 'YOUR_ETHEREUM_ADDRESS',
        // ...
    },
    sol: {
        address: 'YOUR_SOLANA_ADDRESS',
        // ...
    },
    ltc: {
        address: 'YOUR_LITECOIN_ADDRESS',
        // ...
    }
};
```

### 4. Customize Crypto Conversion Rates

Update the conversion rates in `payment.html` (around line 1972) to match current market prices:

```javascript
const cryptoRates = {
    btc: 96000,  // $96,000 per BTC
    eth: 3500,   // $3,500 per ETH
    sol: 220,    // $220 per SOL
    ltc: 107     // $107 per LTC
};
```

## 🌐 GitHub Pages Deployment

### Option 1: GitHub Pages (Recommended)

1. Create a new GitHub repository
2. Upload all files maintaining the folder structure
3. Go to Settings → Pages
4. Select main branch as source
5. Your site will be live at: `https://yourusername.github.io/repository-name/Home.html`

### Option 2: Direct Hosting

Simply upload the `Dumpclub` folder to any web hosting service while maintaining the file structure.

## 🎨 Features

- **Modern UI**: Glass-morphism design with animated backgrounds
- **Responsive**: Works on desktop, tablet, and mobile
- **Multi-language**: Support for 10 languages
- **Live Search**: Real-time product filtering
- **Category Filter**: Filter by Cards/Accounts
- **Stock Indicators**: Shows availability on each product
- **Crypto Payment**: Bitcoin, Ethereum, Solana, Litecoin support
- **Auto QR Codes**: Different QR code for each cryptocurrency
- **Order Tracking**: Unique order ID for each transaction
- **Secure**: SSL, PCI compliant badges

## 📦 Products

The shop currently features:
- **Visa Pre-paid** - $30-$300
- **MasterCard Pre-paid** - $30-$300
- **Stake FA** - $40-$55
- **CashApp FA** - $50-$70
- **Best Buy w/ CC** - $9-$10
- **PayPal FA** - $5
- **Walmart w/ CC** - $5-$8

## 🔧 Customization

### Add New Products

Edit `Home.html` and add to the `productData` object (around line 1288):

```javascript
'Your Product Name': {
    description: '<p>Product description with feature badges...</p>',
    options: [
        { value: 'option1', name: 'Option 1', price: 10.00, stock: 5 },
        { value: 'option2', name: 'Option 2', price: 20.00, stock: 3 }
    ]
}
```

Then add the product card in the HTML (around line 891).

## 📝 Notes

- Files use `sessionStorage` to pass order data between pages
- QR codes are loaded dynamically based on selected cryptocurrency
- All images are hosted externally (except QR codes)
- Custom cursor effects on payment page
- Countdown timer for payment expiration (1 hour)

## 🛠️ Browser Support

- Chrome/Edge (recommended)
- Firefox
- Safari
- Mobile browsers

## 📄 License

Copyright © 2025 DumpClub. All rights reserved.

---

For support or questions, contact via Telegram or Instagram (@punchogs).

