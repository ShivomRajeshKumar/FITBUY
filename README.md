# FITBUY
FitBY: an AI shopping agent Chrome extension that analyzes products on Amazon, Flipkart and Myntra against your personal needs and gives a Fit Score, verdict and regret risk.
FitBY: Buy What Fits You
A Chrome extension with an AI agent that checks any product you browse on Amazon, Flipkart or Myntra against your needs.
Tell it once what you want (budget, use, priorities). Then just shop. FitBY gives you:
A Fit Score (0 to 100) and a clear verdict: Buy, Buy with Caution, Better Alternative, or Don't Buy
A Regret Risk estimate
Review insights that matter for your use
Better alternatives and side-by-side comparison
A chat to ask "Why?" or "Find me something cheaper"
Run it
You need Node.js 18+ and an Anthropic API key.
1. Backend (in the backend folder)
cp .env.example .env     # Windows: copy .env.example .env
# put your key in .env: ANTHROPIC_API_KEY=sk-ant-...
npm install
npm run dev
​
Keep this window open.
2. Extension (in the extension folder)
npm install
npm run build
​
3. Add to Chrome
Open chrome://extensions, turn on Developer mode, click Load unpacked, and choose extension/dist.
Notes
Works without shopping-site API keys. Demo mode uses sample products and labels them Demo Data.
Your API key stays on the backend. Never commit .env.
Built with React, TypeScript, Tailwind, Express and Claude.
