# Forecasting Live Bird Prices in India: A Novel Explainable Approach

## Problem Statement
This work addresses the challenges of forecasting live bird prices in India, focusing on improving prediction stability, accuracy, and interpretability. Traditional regression models such as LSTM and LSTM+TCN exhibited high variability, with prediction errors exceeding 10%, making them unreliable for practical use. To address this, the research reframes the forecasting problem as a classification task and introduces innovative techniques for transparent and actionable insights.

## Proposed Approach
The research introduces the novel ‘gram-K-G’ model, which combines **n-grams**, **K-nearest neighbors**, and **Gower’s distance** to predict sales rate categories instead of continuous sales prices. This classification-based approach reduces volatility and improves forecast accuracy. Additionally, the study incorporates **counterfactual explanations** and **Large Language Model (LLM)-generated justifications** to enhance model interpretability and user trust.

### Key Contributions:
1. **Problem Reframing**: Transforming sales price prediction into a classification task by categorizing sales rates into bins.
2. **gram-K-G Model**: A hybrid model combining n-grams, KNN, and Gower’s distance for accurate category prediction.
3. **Counterfactual Explanations**: Generating actionable alternative scenarios for predicted sales categories, enabling decision-makers to explore minimal feature changes.
4. **LLM-Generated Explanations**: Providing natural language justifications for predictions, enhancing user understanding and trust.

## Methodology
### 1. Data Preparation
- **Features Considered**: Bird quantity, average weight, zone, bird quality, day of the week, holiday indicators, and seasonality.
- **Labeling**: Sales rates were categorized into bins to reframe the regression problem as a classification task.

### 2. Models Evaluated
- **Initial Regression Models**: LSTM and LSTM+TCN, which showed high variability in predictions.
- **Proposed Model (gram-K-G)**: Utilized n-grams for feature engineering, KNN for local pattern recognition, and Gower’s distance for handling mixed data types.
![image](https://github.com/user-attachments/assets/d49633e3-2603-438a-9654-37d471dd6fff)

![image](https://github.com/user-attachments/assets/d89cd065-8e2a-4e99-a80a-90eebc402154)

![image](https://github.com/user-attachments/assets/6feef464-f56d-4a45-b742-89b25c2e5d47)


### 3. Explainability
- **Counterfactual Explanations**: Developed using optimization-based methods to suggest actionable changes (e.g., altering bird quantity or weight) while maintaining realistic bounds.
- **Evaluation Metrics**: Counterfactuals were assessed for validity, diversity, and proximity to user inputs.
- **LLM-Generated Justifications**: Integrated to explain model predictions in clear, contextually relevant terms.

![image](https://github.com/user-attachments/assets/f03566cd-a69a-46f3-bc91-46957566ab21)


## Proof of Concept (PoC)
A PoC application was built using **Streamlit**, allowing users to:
- Input parameters such as bird quantity, weight, and other features.
- Receive predicted sales rate categories.
- Explore counterfactual explanations to understand alternative pricing scenarios.
- View LLM-generated justifications for the model’s predictions.

![image](https://github.com/user-attachments/assets/14136572-e1cd-4fb8-b19b-50901272f04a)

### User Feedback:
Feedback was collected from seven employees involved in pricing decisions. On a five-point Likert scale:
- **Clarity**: Rated highly for clear and comprehensible explanations.
- **Relevance**: Justifications were considered contextually appropriate and actionable.
- **Trust**: Users reported increased confidence in model predictions and decision-making.

## Results and Evaluation
- **Improved Stability**: Classification approach reduced prediction variability, ensuring more reliable forecasts.
- **Enhanced Interpretability**: Counterfactuals and LLM explanations provided actionable insights, increasing user trust.
- **User Acceptance**: High ratings from domain experts validate the practical applicability of the prototype.


## Conclusion
This research presents a robust and explainable framework for live bird price forecasting, addressing price volatility and the need for transparent decision-making. The integration of advanced machine learning techniques, counterfactual explanations, and LLM-generated justifications ensures reliable, actionable, and interpretable predictions.

### Key Contributions:
- Enhanced forecast stability and accuracy by reframing the problem as a classification task.
- Provided actionable insights through counterfactual scenarios and natural language justifications.
- Delivered a user-friendly PoC to demonstrate real-world applicability, increasing trust and confidence among domain experts.


## Future Work
- Extend the approach to other agricultural commodities and volatile markets.
- Explore additional deep learning architectures for further accuracy improvements.
- Enhance the PoC with real-time data integration and advanced visualization features.

This research offers a scalable and transparent solution for live bird price forecasting, providing significant value to decision-makers in the poultry industry and beyond.

## 🌍 Explore More Projects  
For more exciting machine learning and AI projects, visit **[The iVision](https://theivision.wordpress.com/)** and stay updated with the latest innovations and research! 🚀  

---
