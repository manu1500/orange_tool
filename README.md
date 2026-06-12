## 🧠 Predictive Modeling Pipeline (Orange)

Before applications enter the live automation routing, risk evaluation thresholds are validated using a predictive machine learning pipeline designed in **Orange Data Mining**. This layer tests classification stability to ensure decision logic boundaries are mathematically sound.

### Data Science Canvas
<img src="./WhatsApp Image 2026-06-12 at 10.25.50 AM.jpeg" alt="Orange Data Mining Predictive Workflow" width="100%"/>

### Model Components
* **File Node**: Ingests historical credit application training profiles.
* **Select Columns**: Sets the target classification variable (e.g., `System_Initial_Decision`) and isolates key predictive features like credit score and DTI ratios.
* **Logistic Regression**: Trains a generalized linear classification model to calculate risk probabilities.
* **Test and Score**: Evaluates model accuracy, AUC-ROC statistics, and confusion matrices prior to production logic deployment.
