# Smart India Hackathon Workshop
# Date:25/11/2026
## Reference Number:26007418
## Name:Vishva.S

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
1.1 Detailed explanation
FarmLink is a mobile-first web and app platform that connects farmers and Farmer Producer Organizations (FPOs) directly with consumers, retailers, restaurants and bulk buyers.

How it works:

The farmer or FPO registers using a phone number and OTP, in their own language, and lists produce with crop name, quantity, quality grade, expected price, harvest date and photos.
Buyers (households, hotels, supermarkets, hostels, caterers) browse by location, place an order, or post a bulk demand request.
The platform suggests a fair price using mandi price data, matches the order with nearby farmers, and arranges pickup and delivery.
Payment is made through UPI and released to the farmer's bank account after delivery is confirmed.
Both sides rate each other to build trust.
Main modules:

Farmer/FPO portal (listing, orders, earnings dashboard)
Consumer and bulk-buyer portal (search, cart, subscriptions, bulk bidding)
Logistics module (pickup scheduling, delivery tracking, pooled transport)
AI engine (demand forecasting, price suggestion, route optimization)
Admin dashboard (monitoring, dispute handling, analytics)
1.2 How it addresses the problem
Problem today	How FarmLink helps
Produce passes through many middlemen, each taking a margin	Direct farmer-to-buyer connection, so fewer hands in between
Farmers don't know market prices and accept low rates	Live mandi price display and AI-based fair price suggestion
Farmers don't know how much to grow or sell	Demand forecasting shows what buyers need
Vegetables and fruits spoil in a long supply chain	Shorter chain and optimized routes reduce delivery time and wastage
Small farmers can't reach bulk buyers	FPO pooling lets small farmers combine produce for large orders
Late or uncertain payment	Transparent UPI payment tracked in the app
1.3 Innovation and uniqueness
Demand-driven selling: AI forecasts what will sell, so farmers can plan instead of just reacting to the market.
Pooled logistics: orders from nearby farmers are combined into one vehicle to cut transport cost for small farmers.
Fair Price Indicator: shows the farmer price, mandi price and consumer price side by side, so everyone can see where the money goes.
Voice-based and regional-language support (Tamil, Hindi, Telugu, etc.) for farmers with low digital literacy.
Subscription baskets: weekly vegetable boxes directly from local farms give farmers a predictable income.
Low-bandwidth design that works on basic smartphones and weak networks.

## Technical Approach
2.1 Technologies to be used
Layer	Technology
Frontend (web)	React.js, Tailwind CSS
Mobile app	React Native / Flutter (or a Progressive Web App)
Backend	Python (FastAPI or Django)
Database	PostgreSQL (main data), Firebase (notifications)
AI / ML	Python, scikit-learn, Prophet / ARIMA (forecasting), Pandas, NumPy
Route optimization	Google OR-Tools, Google Maps / OpenStreetMap API
Payments	UPI / Razorpay (sandbox for the prototype)
Authentication	OTP-based login (Firebase Auth)
Language support	i18n libraries, speech-to-text and text-to-speech APIs
Hosting	AWS / Render / Vercel
Data sources	Agmarknet / data.gov.in (mandi prices), weather API
2.2 Methodology and process
System flow (flowchart):


System flow (steps):

Farmer lists produce
AI suggests a fair price (using mandi data and demand forecast)
Buyer searches or places an order
Matching engine pairs the order with nearby farmer(s)
Route optimization groups pickups and plans delivery
Delivery and buyer confirmation
UPI payment released to the farmer
Ratings and data feed back into the AI models
Implementation phases:

Phase 1 – Research and design: farmer and buyer interviews, wireframes, database design.
Phase 2 – Core platform: registration, listings, search, orders, payment (sandbox).
Phase 3 – AI modules: price suggestion and demand forecasting using historical mandi data; route optimization for delivery.
Phase 4 – Logistics and tracking: pickup scheduling and delivery status.
Phase 5 – Pilot: test with one FPO in one district, collect feedback and improve.
Working prototype / images: (add your wireframes, screenshots and demo video link here)

## Feasibility and Viability
3.1 Feasibility analysis
Technical: all the tools listed are open-source or have free tiers, and mandi price data is publicly available.
Economic: revenue comes from a small commission per order (around 2-5%), delivery fees and subscription plans. Since the platform removes multiple middleman margins, farmers can still earn more even after the commission.
Operational: we can start with FPOs, which already aggregate farmers, in one district and expand step by step.
Policy: the idea fits with existing government initiatives such as FPO promotion, e-NAM, ONDC and Digital India.
3.2 Challenges and risks, with strategies to overcome them
Challenge / Risk	Strategy
Low digital literacy among farmers	Voice and regional-language interface, simple screens, onboarding through FPOs and local volunteers
Poor internet in villages	Lightweight app, SMS/WhatsApp fallback, offline listing that syncs later
Quality and grading disputes	Photo-based listing, standard grading rules, ratings and a dispute resolution process
High last-mile logistics cost	Pooled deliveries, collection hubs and partnerships with local transport providers
Trust and payment fraud	Verified profiles and escrow-style payment released only after delivery
Perishable produce and price swings	Demand forecasting, short delivery windows and cold-chain partners later
Buyers' habit of using traditional markets	Competitive prices, freshness guarantee and subscription offers
Limited data for AI accuracy at the start	Begin with public mandi data and improve the models as platform data grows

## Impact and Benefits
4.1 Potential impact on the target audience
Farmers / FPOs: higher share of the final price, quicker payments, better planning and access to bulk buyers.
Consumers: fresher produce at lower prices and transparency about where their food comes from.
Bulk buyers (hotels, retailers, caterers): reliable supply, quality assurance and easy ordering.
Government: better visibility into supply and demand, which helps with price stabilization and policy decisions.
4.2 Benefits of the solution
Economic: better farmer income, lower consumer prices and new livelihood opportunities for local delivery partners.
Social: reduced dependence on middlemen, empowerment of small and women farmers, and digital inclusion in rural areas.
Environmental: less food wastage, shorter transport distances and fewer vehicle trips through route optimization.
## Research and References
Agmarknet (mandi prices): https://agmarknet.gov.in
e-NAM, National Agriculture Market: https://enam.gov.in
Ministry of Agriculture & Farmers Welfare (FPO scheme): https://agricoop.gov.in
SFAC, Small Farmers' Agribusiness Consortium: https://sfacindia.com
Google OR-Tools (vehicle routing): https://developers.google.com/optimization
Existing platforms studied: e-NAM, DeHaat, Ninjacart, AgroStar Roy, R., Gupta, S., Wardhan, H., Sarkar, S., Tewari, S., Bansal, R., Bhatia, S. and Gulati, A. (2024). Vegetables Inflation in India: A Study of Tomato, Onion and Potato (TOP). RBI Working Paper Series No. 08/2024: https://rbi.org.in/scripts/PublicationsView.aspx?id=22723
Scroll.in (2024). Farmers get only a third of what consumers spend on vegetables, fruits: Reserve Bank study: https://scroll.in/latest/1074172/scroll_in
