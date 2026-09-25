# OptiPulse: AI-Powered OEE Command Center & Predictive Maintenance Agent

## Overview
OptiPulse is an enterprise-grade agentic application built for the Snowflake CoCo CLI Hackathon. It leverages Snowflake CoCo CLI, Snowflake Cortex Agents, and Cortex Search to monitor factory machine telemetry, calculate real-time Overall Equipment Effectiveness (OEE), detect micro-anomalies, and map error codes to unstructured maintenance manuals.

## Track
Track 3: Predictive Maintenance and OEE Command Center

## Architecture & Data Flow
1. Data Storage (Snowflake): High-frequency sensor streams (vibration, temperature, pressure) and maintenance log tables.
2. Unstructured Knowledge Base: PDF manuals and technical service sheets indexed via Snowflake Cortex Search.
3. Agentic Layer (CoCo CLI): Translates plain-English prompts into optimized SQL, runs multi-step diagnostic reasoning loops, and oversees automated fixes.

## Quick Start / How to Run via CoCo CLI
1. Initialize the terminal tool:
   ```bash
   cortex
   /sql SELECT CURRENT_ROLE(), CURRENT_WAREHOUSE(), CURRENT_DATABASE();
   Analyze the telemetry data for Line-B, compute current OEE, and cross-reference error code E-402 with the maintenance manuals.
   
