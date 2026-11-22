# 💰 WealthAdvisor

A **macOS portfolio tracker** built with SwiftUI that helps you manage your Indian stock market investments — with live price updates, SIP management, and an AI-powered financial advisor.

---

## ✨ Features

- 📊 **Portfolio Dashboard** — View your total net worth, profit/loss, and an interactive donut chart showing asset allocation
- 📈 **Live Stock Prices** — Fetches real-time market prices for NSE/BSE listed stocks using ticker symbols (e.g. `RELIANCE.NS`, `TCS.NS`)
- 🔍 **Ticker Search** — Search and auto-complete stock tickers when adding a new asset
- ➕ **Add / Edit / Delete Assets** — Track stocks, mutual funds, and cash with quantity and average purchase price
- 📉 **Asset Performance View** — See individual stock performance with historical charts
- 🔁 **SIP Manager** — Set up and track your Systematic Investment Plans with monthly deduction dates
- 🤖 **AI Advisor (Gemini 2.5 Flash)** — Ask questions about your portfolio and get personalized, AI-powered financial advice
- 📸 **Portfolio Snapshots** — Save and compare your portfolio at different points in time

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| **SwiftUI** | UI framework |
| **SwiftData** | Local data persistence |
| **Swift Charts** | Native donut & performance charts |
| **Google Generative AI SDK** | Gemini 2.5 Flash for AI advice |
| **Yahoo Finance API** | Live stock price fetching |

---

## 🚀 Getting Started

### Prerequisites
- macOS 14 (Sonoma) or later
- Xcode 15 or later

### Setup

1. **Clone the repo**
   ```bash
   git clone git@github.com:Zenoop90/Wealth-Advisor.git
   cd Wealth-Advisor
   ```

2. **Add your Gemini API Key**

   Open `WealthAdvisor/AIAdvisorService.swift` and replace the placeholder with your key:
   ```swift
   static let apiKey = "YOUR_GEMINI_API_KEY_HERE"
   ```
   Get a free API key at [aistudio.google.com](https://aistudio.google.com)

3. **Open in Xcode**
   ```bash
   open WealthAdvisor.xcodeproj
   ```

4. **Build & Run** — Select your Mac as the target and hit `Cmd + R`

---

## 📂 Project Structure

```
WealthAdvisor/
├── WealthAdvisorApp.swift       # App entry point
├── ContentView.swift            # Root navigation view
├── DashboardView.swift          # Net worth & allocation chart
├── AdvisorView.swift            # AI chat interface
├── SIPManagerView.swift         # SIP setup & tracking
├── AssetPerformanceView.swift   # Individual stock charts
├── PerformanceChartView.swift   # Reusable chart component
├── AddAssetView.swift           # Add new asset form
├── EditAssetView.swift          # Edit existing asset
├── Asset.swift                  # Asset SwiftData model
├── SIP.swift                    # SIP SwiftData model
├── PortfolioSnapshot.swift      # Snapshot model
├── AIAdvisorService.swift       # Gemini AI integration
├── StockPriceService.swift      # Live price fetching
└── TickerSearchService.swift    # Stock ticker search
```

---

## ⚠️ Disclaimer

This app is for **personal tracking and educational purposes only**. It is not financial advice. Always consult a certified financial advisor before making investment decisions.

---

## 📄 License

MIT License — feel free to use, modify, and distribute.
