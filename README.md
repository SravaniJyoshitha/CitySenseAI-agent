CitySense AI Agent — Location Decision Assistant

CitySense is an AI Agent system that helps users make smarter location-based decisions—whether it’s finding apartments, PGs, gyms, or commute-friendly options. It uses real-time data, geo-analysis, scoring, and multi-agent orchestration to deliver trustworthy recommendations.

 Problem Statement

Finding the right place to live or visit often requires switching between maps, listings, reviews, commute calculators, and safety checks. The process is slow, manual, and overwhelming for students, working professionals, and newcomers to a city.

Why Agents?

Agents can reason, search, filter, verify, and combine tools—all autonomously.
Instead of manually checking 10 apps, a multi-agent system:

Collects listings

Fetches geo-coordinates

Measures distances

Evaluates safety, pricing & amenities

Summarizes insights

…without needing human micromanagement. Perfect for continuous, tool-using tasks.

 Architecture — What I Created
1. Planner Agent

Breaks user queries into subtasks and assigns them to the right agents.

2. Collector Agent

Fetches property/business data from APIs or datasets.

3. GeoAgent

Uses geocoding + distance tools (e.g., Nominatim, Haversine) to compute travel distances.

4. Scoring Agent

Ranks options based on price, distance, safety, and user preferences.

5. Summary Agent

Converts raw results into clear, user-friendly recommendations.

Architecture Pattern: Multi-Agent ORPO (Orchestrated, Role-based, Plan-based)

Demo

User inputs:
“Find apartments under ₹10,000 near IIT Hyderabad.”

Agents work:
Collector gathers options → GeoAgent computes distances → Scoring ranks results.

Output:
Top 5 options with distance, pricing, safety score, and a recommendation summary.

Planner:
Produces final action plan: “Best choice is X due to Y.”

The Build — Tech Stack

Python

Google Vertex AI / Colab environment

OpenAI or Gemini LLMs

Nominatim Geocoding API

Haversine distance calculator

Multi-agent patterns (Planner, Worker, Tool agents)

Dataset integration (open-source housing dataset)

Core Skills Demonstrated:
 Agent tool-calling
 Geo-analysis
✔ Ranking & scoring pipeline
✔ Real dataset usage
✔ Autonomous orchestration
