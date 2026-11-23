# Machine Learning based Buyer Segmentation and Investment Profiling for Real Estate Market Intelligence

Internship project with **Unified Mentor** and **Parcl Co. Limited**.

## Objective

Group real estate buyers into clear segments, understand how each group invests and spends, and turn the findings into business actions.

## Data

| File | Description |
|---|---|
| `clients.csv` | 2,000 clients |
| `properties.csv` | 10,000 units (7,305 sold) |

## Workflow

1. **Cleaning and preparation (Python):** merged sold units to clients, converted text prices to numbers, parsed mixed date formats, calculated age.
2. **Feature engineering:** 0/1 flags for company, investment purpose, loan use and international buyer; log transform of total spend; standard scaling.
3. **Model selection:** compared KMeans, Hierarchical (Ward) and Gaussian Mixture for k = 2 to 8 using silhouette score and the elbow method.
4. **Final model:** Hierarchical clustering with 4 clusters on 8 features.
5. **Dashboard:** Power BI, 5 pages, 4 slicers (country, region, acquisition purpose, client type).
6. **Research paper:** findings, limitations and recommendations.


## Key Findings

- Total spend is about $2.52B, an average of $1.26M per customer.
- Segments differ in **who the buyers are**, not in how much they spend (average spend varies by about 4%).
- 31% of buyers invest, 37% use loans, and 77% of customers are in the USA (California is the top region).
- Average satisfaction is 3.03 out of 5, and about 39% of buyers rate it 1 or 2.
- Referral channels: website 55%, agency 35%, client referral 10%.

## Recommendations

- Improve loan support and after-sales service for home buyers.
- Build rental-yield offers for domestic investors.
- Run remote-buying support and country-focused marketing for international buyers.
- Offer bulk packages and a dedicated account manager for corporate buyers.
- Start a client referral reward programme.

## Power BI Dashboard Pages

1. Buyer Segmentation Overview
2. Customer Profile
3. Investor Behavior and Financing
4. Geographic Buyer Analysis
5. Segment Insights

## Limitations

- Silhouette score is about 0.19, so the segments overlap.
- There is no income column, so affordability could not be profiled.
- The date format in the property data is ambiguous, so no time trends were built.
- Power BI was used instead of Streamlit.

## Tech Stack

Python (pandas, scikit-learn), Power BI (DAX)



