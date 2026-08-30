SELECT * 
FROM churn_clean

-- Exploratory Analysis

-- Which contract type has the highest churn rate?
SELECT
	Contract ,
	COUNT(*) AS Total_Customers,
	SUM (CASE WHEN Churn = 'Yes' THEN 1 ELSE 0 END) AS Churned_Customers,
	ROUND(
				SUM(CASE WHEN Churn = 'Yes' THEN 1 ELSE 0 END) * 100.0 / COUNT(*),
                2
    ) AS Churn_Rate
	FROM churn_clean
	GROUP BY Contract
	ORDER BY Churn_Rate DESC;
	
	
-- Does internet service type influence churn?
SELECT 
	InternetService,
	COUNT(*) AS Total_Customers,
	SUM(CASE WHEN Churn = 'Yes' THEN 1 ELSE 0 END) AS Churned_Customers,
	ROUND(
		SUM(CASE WHEN Churn = 'Yes' THEN 1 ELSE 0 END) * 100.0 / COUNT(*), 
		2
	) AS Churn_Rate
	FROM churn_clean
	GROUP BY InternetService
	ORDER BY Churn_Rate DESC;

	
-- Which payment methods are associated with the highest churn?
SELECT
	PaymentMethod,
	COUNT(*) AS Total_Customers,
	SUM(CASE WHEN Churn = 'Yes' THEN 1 ELSE 0 END) AS Churned_Customers,
	ROUND(
		SUM(CASE WHEN Churn = 'Yes' THEN 1 ELSE 0 END) * 100.0 / COUNT(*), 
		2
	) AS Churn_Rate
	FROM churn_clean
	GROUP BY PaymentMethod
	ORDER BY Churn_Rate DESC

-- Are customers with higher monthly  charges more likely to churn?
SELECT
	Churn,
	ROUND(AVG(MonthlyCharges), 2) AS Avg_Monthly_Charge,
	MIN(MonthlyCharges) AS Min_Charge,
	MAX(MonthlyCharges) AS Max_Charge
FROM churn_clean
GROUP BY Churn;

-- Does customer tenure affect churn?
SELECT 
	Churn,
	ROUND(AVG(Tenure), 2) AS Average_Tenure,
	MIN(Tenure) AS Minimun_Tenure,
	MAX(Tenure) AS Maximum_Tenure
FROM churn_clean
GROUP BY Churn;



