Customer Booking Behaviour & Revenue Drivers Analysis
An end-to-end exploratory data analysis of 119,390 hotel booking records, examining cancellation drivers, pricing patterns, and demand seasonality across City Hotel and Resort Hotel segments.

Project Objective
The hotel industry suffers significant revenue leakage from last-minute cancellations, under-priced rooms, and poorly targeted marketing. This project answers three core questions:

Why do guests cancel — and which segments cancel most?
How does Average Daily Rate (ADR) vary across hotel types and seasons?
Which markets and countries drive the most demand and cancellation risk?


Dataset
PropertyDetailFilehotel_bookings.csvRecords119,390 bookingsFeatures32 variablesPeriod2015 – 2017Hotel TypesCity Hotel, Resort Hotel
Key variable groups: booking logistics, guest demographics, room/rate details, and reservation outcomes (is_canceled as the primary target).
Data quality: company (94% missing) and agent (14% missing) were dropped. Remaining nulls removed via listwise deletion. One ADR outlier (> 5,000) removed. Final working dataset: ~118,898 records.

Methodology

Data Loading & Inspection — shape, dtypes, null counts, descriptive statistics
Data Cleaning — datetime conversion, column drops, null removal, outlier filtering, feature engineering (month column)
Univariate & Bivariate Analysis — cancellation distribution, hotel-type comparison, market segment breakdown
Time-Series Visualisation — ADR trends over time for both hotel types; cancelled vs. not-cancelled ADR overlay
Geographic & Segmentation Analysis — top 10 cancelling countries (pie chart), market segment share comparison


Key Findings

~37% of bookings are cancelled — a major revenue risk
City Hotel cancels at nearly 2× the Resort Hotel rate — driven by transient corporate and OTA bookings
ADR peaks mid-year (July–August), especially for Resort Hotel; cancelled bookings cluster at higher ADR values
Portugal (PRT) accounts for the largest share of cancellations by country
Online Travel Agencies drive ~74% of cancellations despite being one of multiple booking channels
August is the peak month for both bookings and cancellations — the most operationally complex period


Managerial Implications
RecommendationRationaleEnforce deposit requirements on OTA bookingsOTAs drive ~74% of cancellations; deposits reduce speculative bookingsApply dynamic overbooking at City HotelNear-2× cancellation rate means rooms regularly go empty post-cancellationRaise prices in July–August (especially Resort)ADR analysis reveals under-pricing during peak demand periodsInvestigate Portuguese guest behaviourOutsized domestic cancellation share warrants targeted retention effortsIncentivise direct bookingsDirect channel has the lowest cancellation rate (4%) and no OTA commissionMonitor ADR vs. cancellation correlationHigher-ADR bookings cancel more — rate parity management is essential
