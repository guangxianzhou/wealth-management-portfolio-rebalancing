# Executive Wealth Management & Portfolio Rebalancing Dashboard

## Project Overview
This project features an institutional-grade Wealth Management Portfolio Rebalancing & Asset Allocation Dashboard developed using Microsoft Power BI and DAX. Built from the perspective of private wealth advisors and family offices, the system monitors portfolio allocation drifts relative to strategic targets, generates automated rebalancing directives, and provides position-level visibility across diverse asset classes.
## Dashboard Preview
## Core Features & Business Architecture
### 1. Executive Portfolio Health (KPI Cards)
Total Portfolio Value (AUM): Dynamically tracks aggregated multi-asset market value.

Unrealized Gain & Unrealized Return %: Real-time measurement of unrealized performance and return metrics.

Annual Projected Income: Estimates projected forward cash flows across dividend-paying equities and fixed-income instruments.

### 2. Multi-Asset Strategic Allocation & Drift Logic
Monitors broad asset classes: US Large Cap, US Small/Mid Cap, International Equity, Fixed Income, Cash & Equivalents, and Alternatives.

Dynamic calculation of allocation drift:
Allocation Variance % = Actual Weight % - Target Weight %

Automated Action Alerts:

Trim / Sell: Triggered when an asset class exceeds strategic allocation boundaries.

Add / Buy: Highlights capital deployment opportunities for under-allocated asset classes.

In Tolerance: Signifies holdings within the target rebalancing threshold.

Conditional Formatting: Soft green and red color indicators for intuitive executive triage.

### 3. Security-Level Drill-Down Analysis
Detailed position breakdown containing: Security Name, Ticker, Quantity, Shares Price, Total Value, and Unrealized Gain/Loss.

Interactive cross-filtering allows granular inspection of underlying securities (such as VOO, BND, VGT, SGOV, GLD) when clicking on individual asset categories.

### 4. Client Slicing Capability
Integrated client-level filtering supporting multi-account portfolio governance (e.g., Miller Family Trust).

## Data Model & Technical Stack
Tool: Microsoft Power BI Desktop

Language: DAX (Data Analysis Expressions) for dynamic weighted allocation and threshold logic

Data Schema: Relational Star Schema linking client profiles (Dim_Client_Profile), strategic models (Dim_Target_Allocation), and current positions (Fact_Holdings).

Design Standards: Institutional layout, card-in-container shadow layering, Segoe UI typography, and neutral canvas background.

## Repository Contents
WM_Portfolio_Rebalancing_Dashboard.pbix: Full Power BI model, DAX measures, and interactive report.

Executive_Portfolio_Rebalancing_Report_2026.pdf: High-resolution executive presentation export.

![Dashboard Preview](Screenshot%202026-09-23%20at%2021.31.08.jpg)
