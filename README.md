## 🚀 Project Overview: AtmoSync (Micro-Climate Arbitrage Analytics)

### 📌 Problem Statement
Traditional supply chain analytics rely heavily on standard transit times and macro-weather forecasts. However, they fail to track how real-time, hyper-local micro-climate shifts—such as sudden humidity or temperature spikes inside a specific shipping container—degrade agricultural commodities long before they reach the market.

### 💡 Use Case & Business Value
Designed for commodities traders at Infotact, AtmoSync continuously monitors live container telemetry. If the streaming pipeline detects an internal temperature drift that increases the spoilage rate of perishable goods (like avocados), the dashboard instantly calculates **"Spoilage Arbitrage"**. This alerts the trader to reroute the shipment to a closer, secondary market, securing a premium price before the goods degrade below quality thresholds.

### 🛠️ Tech Stack & Architecture
The project utilizes the Modern Data Stack (MDS) and cloud-native architecture:
* **Streaming Ingestion:** **Apache Kafka** for high-throughput event streaming of continuous mock lot sensor data (temperature, humidity, vibration).
* **Cloud Data Warehouse:** **Snowflake** for highly scalable storage of raw IoT streams and historical commodity pricing data.
* **Data Transformation:** **dbt (Data Build Tool)** for ELT modeling to clean raw JSON payloads and calculate complex arbitrage margins and spoilage degradation curves using SQL.
* **Visualization Layer:** **Apache Superset** for a real-time BI dashboard rendering live container health and financial arbitrage opportunities.
