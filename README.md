Currency Converter Pro
A high-precision, real-time currency exchange platform with 24-hour market trend analysis.

📌 The "Why"
In a globalized economy, knowing the exchange rate is not enough—users need to know how the market is moving. Currency Converter Pro was built to provide not just conversions, but a mini-financial dashboard. It bridges the gap between a simple calculator and a professional trading tool.

🚀 Key Features
Global Currency Support: Over 150+ fiat currencies and 2,500+ exchange pairs.

Live API Integration: Fetches accurate, real-time rates directly from a live financial data provider.

24-Hour Trend Indicators: Automated "snapshots" compare current rates with the previous 24 hours, displaying visual arrows and percentage shifts.

Optimized Performance: Uses an intelligent caching/snapshotting system to minimize API calls and maximize speed.

User-First UI: Responsive design with interactive animations and intuitive currency selection.

🛠️ Tech Stack
Runtime: Node.js (utilizing native fetch for high-speed API communication)

Database: PostgreSQL with Drizzle ORM (custom schema for rateSnapshotsand currency logs).

Language: TypeScript (Strictly typed for financial accuracy).

Deployment: Integrated for cloud-based persistence.

🌍 Real-Life Application
E-commerce: Essential for businesses calculating global shipping and multi-currency pricing.

Travel: A reliable companion for travelers to track their spending power against shifting markets.

Finance Education: A practical tool for learning how currency pairs fluctuate in response to global events.

⚙️ How It Works (The Logic)
The system runs an automated script ( update-rates-fast.mjs) that:

Validates the current currency list.

Creates a snapshot of existing rates in the database.

Fetches new data from the API.

Calculates the delta(change) between the new rate and the snapshot.

Updates the UI with color-coded indicators (Green for growth, Red for decline).

💡 What's Next?
I'm planning to implement a Cron Job for automatic hourly updates and a History Graph feature.
