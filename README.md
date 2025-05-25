# FUA-RESEARCH

## Introduction
This project investigates the spatial drivers and propagation mechanisms of urban air pollutant emissions across 619 Functional Urban Areas (FUAs) in Europe. We focus on four major pollutants—CO₂, NOx, SO₂, and PM₂.₅—and examine their relationships with 14 socioeconomic and spatial variables. The study integrates machine learning models with SHAP-based interpretability, geographically weighted regression (GWR) to capture spatial heterogeneity, and graph attention networks (GAT) to model inter-FUA influence. This multi-method approach enables a comprehensive understanding of both local emission patterns and spatial interaction effects across FUAs.

## Highlights
Multi-Model Comparison, Covering Conventional and Advanced Algorithms

Six regression models—XGBoost, CatBoost, Random Forest, Elastic Net, KNN, and Extra Trees Regressor—were developed in parallel to comprehensively evaluate the performance of different algorithms in forecasting urban emissions.

Strong Interpretability—SHAP Contribution Analysis

We use SHAP (Shapley Additive Explanations) to quantitatively interpret each model’s feature contributions. The resulting SHAP summary plots and dependence plots give policymakers an intuitive view of the marginal effects of factors such as population, industrial structure, and traffic density on emissions.

Subgroup Analysis—Accounting for Economic Disparities

Cities are grouped into high-, medium-, and low-GDP categories, with separate CatBoost + SHAP models trained for each. This reveals the key driving factors at different stages of economic development.

Spatial Heterogeneity Modeling—Geographically Weighted Regression

GWR models for PM₂.₅ and NOₓ generate local R² maps and spatial distributions of regression coefficients, uncovering how the same factor can have varying influence across regions. Residual maps and outlier detection further identify cities with abnormal emissions, providing targeted guidance for regional collaborative governance.

Cutting-Edge Application—Graph Attention Networks (GTA)

We apply the graph attention mechanism from graph neural networks to urban emissions modeling. By leveraging spatial adjacency and network “centrality” metrics, the GTA captures regional diffusion effects and structural influences among cities.

## Policy Implications
Targeted, City-Specific Policies

The SHAP and subgroup analyses help policymakers pinpoint the most sensitive emission-reduction drivers for each city type. For example:

In megacities and economically advanced regions, traffic congestion mitigation should be the top priority.

In less industrialized or energy-intensive cities, restructuring the energy mix is more urgent.

Spatially Coordinated Governance

GWR’s local R² maps clearly show where explanatory power is high or low, highlighting that cross-regional collaboration must account for differing factor effects in neighboring areas. Clusters of outliers and residuals can be used to prioritize regulatory oversight and resource deployment.

Dynamic Monitoring and Early Warning

Leveraging the graph attention model, one can construct an urban emissions network that shifts focus from individual cities to city clusters, capturing real-time “diffusion chains” of pollutants and enabling a dynamic early-warning system.

Cost-Effectiveness and Investment Guidance

Variations in factor importance rankings and magnitudes across models allow governments to conduct cost-benefit analyses within budget constraints, ensuring optimal allocation of environmental funding and technical assistance.


