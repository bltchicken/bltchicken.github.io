# Crypto QR Codes Setup

## 📱 Add Your Wallet QR Codes

Place your cryptocurrency wallet QR code images in this folder with these exact filenames:

### Required Files:

1. **Bitcoin QR.png** ✅ Added
   - Your Bitcoin wallet QR code

2. **Solana QR.png** ✅ Added
   - Your Solana wallet QR code
   - From: https://i.ibb.co/RTGKHzVw/hovercode-2.png

3. **Ethereum QR.png** ✅ Added
   - Your Ethereum wallet QR code
   - From: https://i.ibb.co/gFbqwyWJ/hovercode-3.png

4. **Litecoin QR.png** (optional)
   - Your Litecoin wallet QR code
   - If not provided, Bitcoin QR will be used as fallback

## 📏 Image Requirements

- **Format**: PNG (recommended)
- **Size**: Square format (e.g., 500x500px or larger)
- **Quality**: High resolution for scanning
- **Background**: Any (will be displayed in white container)

## 🔧 How It Works

When a customer selects a payment method:
- Selects **Bitcoin** → Shows `bitcoin-qr.png`
- Selects **Solana** → Shows `solana-qr.png`
- Selects **Ethereum** → Shows `ethereum-qr.png`
- Selects **Litecoin** → Shows `litecoin-qr.png`

The correct QR code is automatically displayed based on their choice.

## ⚠️ Important

Make sure the filenames match EXACTLY (case-sensitive on GitHub):
- ✅ `Bitcoin QR.png`
- ✅ `Solana QR.png`
- ✅ `Ethereum QR.png`
- ❌ `bitcoin-qr.png` (wrong case)
- ❌ `bitcoin_qr.png` (wrong format)

