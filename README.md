🚦 Explainable Traffic Congestion Analysis using Agentic AI
📌 Project Overview

This project presents an Agentic AI-based traffic congestion analysis system built using Langflow and IBM watsonx (Granite model).
The system analyzes historical Bangalore traffic data from a single CSV file and generates transparent, explainable insights into traffic congestion patterns and causes.

The goal is to improve trust and interpretability in AI-driven traffic analysis by clearly answering:

Is there congestion?

Is it recurring?

Why is it happening?

🎯 Key Features

Agent-based traffic analysis using Langflow

Explainable congestion detection and reasoning

CSV-driven analysis (no external APIs required)

Clear separation of analysis, causation, and explanation

Human-readable traffic insights

🧠 System Architecture (Agents Used)
1. Traffic State & Pattern Analysis Agent

Detects congestion presence and severity

Identifies whether congestion is recurring or non-recurring

2. Congestion Cause Attribution Agent

Infers data-driven causes of congestion

Uses correlations between speed, volume, time, and location

3. Explainable Traffic Insight Assistant

Converts technical analysis into simple, human-readable explanations

Improves transparency and trust

📥 Input

User provides traffic context through Chat Input:

Location

Day Type (Weekday / Weekend)

Time Window

Example:

Location: Silk Board Junction
Day Type: Weekday
Time Window: 18:00–19:00

📤 Output

Congestion status and severity

Pattern identification (recurring / non-recurring)

Clear explanation of why congestion occurs

📊 Dataset

File: Banglore_traffic_Dataset.csv

Rows: ~8000

Source: Historical Bangalore traffic data

Used as the single source of truth for all agents

🧩 Langflow Components Used

Chat Input – Accepts user traffic parameters

IBM watsonx AI Agent – Core reasoning and analysis

File Component (CSV Loader) – Loads traffic dataset

Chat Output – Displays final explainable insights

📁 Project Structure
data/
 └── Banglore_traffic_Dataset.csv

langflow/
 └── AI-traffic-explainability.json

traffic_knowledge_docs/
 └── (reserved for future extensions)

README.md
.gitignore

🚀 How to Run

Open Langflow

Import AI-traffic-explainability.json

Ensure the CSV file path is correctly linked

Configure IBM watsonx credentials

Enter traffic details in Chat Input and run the flow

🔮 Future Scope

Integration with real-time traffic data

Inclusion of weather and incident information

Predictive congestion forecasting

Expansion to multi-city traffic analysis

Deployment as a traffic decision-support system

🏁 Conclusion

This project demonstrates how agentic AI and explainable reasoning can be applied to traffic congestion analysis using a simple CSV dataset, making AI-driven decisions more transparent, interpretable, and trustworthy.
