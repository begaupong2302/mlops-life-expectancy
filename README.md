# Life Expectancy Prediction with MLOps

## A. Overall Goal of the Project

The goal of this project is to build a machine learning model that can predict life expectancy based on various socioeconomic, healthcare, and environmental factors. By using a dataset from the World Health Organization (WHO), the model aims to estimate life expectancy across different countries. This project also integrates MLOps practices to automate the entire machine learning lifecycle, from model development to deployment.

Key objectives include:
- Preprocessing and cleaning the data (handling missing values, scaling features).
- Exploring different machine learning models and selecting the best one.
- Deploying the model as a RESTful API to allow easy integration with external applications.
- Implementing MLOps practices for versioning, tracking experiments, and automating model deployment.

## B. Frameworks to be Used

### Machine Learning Framework:
- **scikit-learn**: For basic models like Linear Regression and Random Forest.
- **XGBoost**: For advanced regression techniques and boosting models.
- **MLflow**: To track experiments, version models, and manage the model lifecycle.

### MLOps Framework:
- **Docker**: For containerizing the project and ensuring it runs consistently across different environments.
- **Kubernetes**: For orchestrating containerized applications, allowing scalable deployment.
- **GitHub Actions** or **Kubeflow**: For automating the entire workflow, including training, testing, and deploying models.

We will include these frameworks by setting up pipelines for model training, experimentation tracking, and deployment. MLflow will be used for model versioning and experiment tracking, while Docker and Kubernetes will help automate the deployment process.

## C. Data to be Used

Initially, we will use the **"Life Expectancy (WHO)" dataset** available on Kaggle. This dataset contains various socioeconomic, healthcare, and environmental features, such as:
- **Life expectancy**
- **GDP**
- **Alcohol consumption**
- **Healthcare expenditure**
- **Population**
- **Country**
- **Year**

The data will be cleaned, transformed, and preprocessed before being used in the machine learning models. If needed, additional external datasets might be integrated in the future to improve the model’s performance.

## D. Models to be Used

We plan to experiment with several machine learning models, including:
- **XGBoost**: For advanced boosting models that can capture more complex relationships in the data.

The goal is to compare the performance of these models and choose the best-performing one for deployment.

---

5. Deploy the model:
   ```bash
   docker build -t life-expectancy-model .
   docker run -p 5000:5000 life-expectancy-model
   

