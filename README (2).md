# Kenya AI Trading Command Centre

Starter project for a demo-first trading dashboard and secure Deriv OAuth backend.

## Project structure
- `dashboard.html` — responsive market dashboard prototype.
- `backend/` — Node.js/Express backend starter for Deriv demo OAuth.

## Deploy the backend on Render
1. Create a Render Web Service from this GitHub repository.
2. Set the **Root Directory** to `backend`.
3. Build command: `npm install`
4. Start command: `npm start`
5. Configure `APP_BASE_URL`, `DERIV_CLIENT_ID`, and `SESSION_SECRET` in Render's environment settings. Never commit real secrets.
6. Add the deployed callback URL to the Deriv OAuth application's allowed redirect URLs.

## Important limitations
This is a prototype. The dashboard reads public market data; the backend starter handles demo OAuth but does not place orders. Automated execution, MT5 connectivity, validated strategies, contract-aware sizing, server-side loss limits, emergency stop, and end-to-end demo testing are not implemented. Live trading must remain disabled until these controls are independently tested.
