 EU Logistics Expansion Screen

Independent portfolio project by Nusrat Jaman

## Business Question

Which EU markets should a Danish third-party logistics (3PL) provider take forward for deeper expansion assessment when current road-freight activity and logistics performance are considered together?

This project is designed as a first-stage market-screening exercise. It does not attempt to forecast revenue, profitability, market share or return on investment.

## Method

The analysis covers the 27 EU Member States and combines two indicators:

| Indicator |                       Source |               Period |                     Weight |

| Logistics Performance Index (LPI) | World Bank           | 2023                       | 40% |
| Road freight activity             | Eurostat             | 2024                       | 40% |

The two indicators are normalised and combined in Power BI to produce an **Expansion Score**.

The current model explicitly weights these two components at 40% each. The remaining 20% is not assigned to an additional variable, so the Expansion Score is a screening index rather than a percentage measure of market attractiveness.

## Key Results

| Rank    | Market    | LPI 2023 |      2024 Road Freight (MIO_TKM)        | Expansion Score |

| 1 |      Germany     | 4.10 |         127,006                             | **67.08** |
| 2 |      Poland      | 3.60 |         57,992                              | **39.18** |
| 3 |      France      | 3.90 |         32,249                              | **35.26** |
| 4 |      Sweden      | 4.00 |         21,789                              | **33.37** |
| 5 |      Austria     | 4.00 |         20,997                              | **33.13** |

## Recommendation

Germany is the primary market identified by the screening model, with Poland as the secondary market for further commercial assessment.

The result follows from the combination of the selected logistics-performance and road-freight indicators. It should not be interpreted as evidence that either market will necessarily generate higher revenue or profitability.

## Data Preparation

The project was developed in Power BI using Power Query for data preparation.

The Eurostat road-freight data was cleaned, annual fields were standardised, non-numeric markers were handled, and the 2024 `MIO_TKM` measure was selected for the scoring model.

The World Bank LPI dataset was reduced to country, country code and the latest usable project year, 2023.

Because the two datasets use different country-code formats, a country-code mapping was created in Power BI to establish the relationship between the datasets.

The final analysis was restricted to the 27 EU Member States.

## Tools

- Power BI
- Power Query
- DAX
- Microsoft Excel

## Dashboard

The Power BI dashboard contains:

- 2024 freight-market analysis
- World Bank LPI country ranking
- EU Expansion Score model
- Top-10 market ranking
- Recommendation page

## Limitations

The model is a first-stage screening tool and does not include several commercial variables that would be required for a market-entry decision.

These include:

- Competitive intensity
- Customer demand and concentration
- Labour costs
- Warehouse and operating costs
- Pricing and margins
- Regulatory requirements
- Market-entry investment
- Local commercial conditions

The freight and LPI indicators also refer to different reporting periods: 2024 and 2023 respectively.

Further commercial due diligence would therefore be required before making an actual expansion decision.

## Data Sources

- Eurostat — Road freight transport
- World Bank — Logistics Performance Index
- European Commission — TEN-T and European transport infrastructure
- dashboard_1_scoring.png
dashboard_2_recommendation.png



## Project Files

- `EU_Logistics_Dashboard.pbix` — Power BI dashboard and data model
- `EU_Logistics_Expansion_Business_Paper.docx` — Business research paper and analysis
- `README.md` — Project documentation
