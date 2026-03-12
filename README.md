# LLM Trading Experiment Dashboard

Live dashboard for monitoring the autonomous trading research agents.

## Access

Open `index.html` in your browser. The dashboard will connect to the API server.

**Note:** The API server must be accessible from your network. If using remotely, update the `API_URL` variable in `index.html`.

## What It Shows

- 🎯 **Production Strategy** - Current live trading parameters
- 💰 **Live Paper Trading** - Alpaca account status, positions, trades
- 🤖 **Research Agents** - Experiment counts, best Sharpe, recent results

## API Endpoint

The dashboard fetches data from:
```
http://<your-server>:5000/api/status
```

## Setup

1. Ensure the API server is running:
   ```bash
   cd /home/ubuntu/.openclaw/workspace/projects/llm-trading-experiment/src
   python3 web_dashboard.py
   ```

2. Open port 5000 in your firewall/security group (AWS, GCP, etc.)

3. Update `API_URL` in `index.html` to point to your server

4. Open `index.html` in a browser
