# VED AI AUTO TRADER — Android starter (v0.1 demo)

This is a **starter Android Studio project**, not a finished trading product or APK.
It contains a mobile dashboard mock-up for a ₹5,000 demo account. It does not connect
to Groww, Delta Exchange, Gmail, or place any live orders.

## Open the project
1. Install Android Studio (current stable).
2. Open this folder as a project.
3. Let Gradle sync, then run on an Android device/emulator.

## Before any live trading is enabled
- Implement Gmail sign-in with Firebase Authentication and the app's own Firebase config.
- Build a secure backend. Never store broker API secrets in the Android app.
- Implement each broker using its official API and the account owner's authorized flow.
- Add broker-specific order validation, position/order reconciliation, duplicate-order
  protection, kill switch, daily loss limit, stale-feed checks, and audit logs.
- Add exchange/broker algo registration and compliance checks applicable to the strategy.
- Run extensive paper trading and failure-mode tests before considering live mode.

## Important broker notes
- Groww documents Trading APIs for market data, orders and portfolio functions; its current
  published pricing page lists ₹499 + taxes/month for the API plan. Verify current terms.
- Delta Exchange India documents authenticated order APIs and requires API-key security,
  including IP whitelisting for trading permissions.
- Broker API access and retail-algo requirements can change. Confirm directly with each broker.

## Safety defaults
- This starter has no live-order code.
- A ₹5,000 account is small; fees, taxes, slippage and API charges can materially affect results.
- Stop-loss orders cannot guarantee the exact exit price during gaps, illiquidity or outages.
