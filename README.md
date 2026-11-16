# Smart India Hackathon Workshop
# Date:
## Reference Number:
## Name:

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
1. Detailed explanation
A digital marketplace where farmers and FPOs list produce directly and consumers and bulk buyers (restaurants, hostels, retailers, institutions) order from them with no mandi middlemen. It has four parts:

A voice-first farmer app in regional languages for listing produce, setting prices and tracking orders.
A consumer and bulk-buyer app with pre-orders and subscriptions.
Built-in logistics: pickup from village collection points, shared delivery routes and partner matching.
An AI layer for demand forecasting, fair-price suggestions and route optimization. Payments go by UPI straight to the farmer’s bank account.
2. How it addresses the problem

Farmers sell directly, so the margin that went to intermediaries is shared between farmers and consumers.
Demand forecasts tell farmers what to grow and when to harvest, which cuts wastage and distress sales.
Route optimization and consolidated pickups cut transport cost per kg.
Live mandi benchmarks (eNAM, Agmarknet) keep prices transparent for both sides.
3. Innovation and uniqueness

Voice-first, vernacular interface for low-literacy and low-bandwidth users.
Demand-driven pre-orders: farmers harvest against forecast orders instead of guessing.
FPO and bulk-buyer matching, not only retail.
A price engine that shows farmers a “fair price band” next to the current mandi rate.

## Technical Approach
1. Technologies

Frontend: React Native (farmer and consumer apps, with an offline-first mode), React (admin dashboard).
Backend: Python (FastAPI) or Node.js microservices behind an API gateway, with OTP-based login.
Database: PostgreSQL for transactions, Redis for caching.
AI/ML: Python with scikit-learn, Prophet and XGBoost for demand and price forecasting, and Google OR-Tools for route optimization (a vehicle-routing problem).
Speech: Bhashini APIs for regional-language voice input and translation.
Integrations: Razorpay or the UPI/NPCI stack for payments, eNAM and Agmarknet price data, Google Maps APIs.
Hosting: cloud (AWS or Azure) with Docker.
<img width="1890" height="1242" alt="technical_approach_diagram (1)" src="https://github.com/user-attachments/assets/6d0cabfa-2a11-4e4d-b66a-ead9e3fc2a52" />
2. Methodology and process
Architecture diagram: see the one above. Implementation phases:

Pilot in one district with 2–3 FPOs and 3–4 crops.
Build the MVP: listings, ordering, UPI payments.
Train forecasting models on historical mandi data and add logistics matching.
Test with real farmers and buyers, gather feedback, then scale by district.
<img width="1890" height="1242" alt="methodology_flowchart" src="https://github.com/user-attachments/assets/7a4827cd-4246-46f0-8e1a-937b5eedb4ef" />

## Feasibility and Viability
1. Feasibility

Every component uses mature, available technology: UPI, public mandi datasets, open-source ML and routing tools.
Smartphone and UPI penetration in rural India is high enough for an app-based pilot.
FPOs give a ready aggregation channel.
2. Challenges and risks

Low digital literacy among farmers.
Perishability and last-mile delivery cost.
Quality disputes and grading.
The cold-start problem of getting both farmers and buyers on the platform.
Patchy rural connectivity.
3. Strategies

Voice-first UI, FPO-led onboarding and field agents.
Collection points and shared routes to lower delivery cost.
Photo-based quality grading plus ratings, with a clear return policy.
Starting with bulk buyers to guarantee volume, then adding retail.
Offline-first app design that syncs when connectivity returns.


## Impact and Benefits
1. Impact on the target audience

Farmers and FPOs earn a larger share of the final price and get faster, direct payment.
Consumers pay less for fresher produce.
Bulk buyers get dependable supply and transparent pricing.

2. Benefits

Economic: higher farmer income, lower consumer prices and a more efficient supply chain.
Social: digital inclusion for rural users and a stronger role for FPOs.
Environmental: less food wastage and fewer transport kilometres through optimized routes.
## Research and References
eNAM (National Agriculture Market): https://enam.gov.in
Agmarknet (mandi price data): https://agmarknet.gov.in
Price Monitoring Division, Department of Consumer Affairs: https://fcainfoweb.nic.in
ONDC (Open Network for Digital Commerce): https://ondc.org
Bhashini (Indian-language AI services): https://bhashini.gov.in
Google OR-Tools (vehicle routing): https://developers.google.com/optimization/routing
Government scheme for formation and promotion of 10,000 FPOs (Ministry of Agriculture and Farmers Welfare)

