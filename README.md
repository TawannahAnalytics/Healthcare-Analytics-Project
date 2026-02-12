# Healthcare-Analytics-Project
<div align = "justify" >This analysis examines a healthcare dataset of 349 patient records to identify disease patterns, symptom prevalence, and outcome predictors. The analysis was conducted using Excel functions (COUNTIF, AVERAGEIF, COUNTIFS) with PivotTable validation to ensure accuracy.
### Key Questions Addressed
1. Most frequent disease and its prevalence
2. Age patterns across diseases
3. Most common symptoms
4. Gender distribution
5. Blood pressure distribution
6. Relationship between difficulty breathing and patient outcomes.

**Tools Used:** Microsoft Excel (functions, PivotTables, data visualization).

**1.Which disease occurs most frequently in the dataset, and what percentage of patients does it represent?**
**Approach:** The dataset contained 349 patient records with diseases repeated across multiple rows. To identify the most common disease, I first extracted unique disease names using Excel's Remove Duplicates feature. Then I used the COUNTIF function to count how many times each disease appeared in the dataset.
**Validation (PivotTable Cross Check):** To validate the accuracy of the excel function results, i created a PivotTable with diseases in the rows area and count of diseases in the values area. The PivotTable confirmed that **Asthma** had the highest frequency, matching the countif result and ensuring no records were missed.  
**Result:** Asthma was the most frequent disease, affecting 23 patients. To calculate the percentage, I divided 23 by the total patient count (349), which equals 6.59% of patients.  
**Insight:** Asthma represents the most common condition in this patient population. This information could help healthcare providers allocate resources for asthma management programs or screening initiatives.

  <img width="538" height="350" alt="image" src="https://github.com/user-attachments/assets/133ba71a-29db-4bc7-9aee-a75a5da756c9" />  


**2. What is the average age of patients for each disease, and which disease affects the oldest group on average?**  
**Approach:** I calculated the average patient age for each disease using the AVERAGEIF function after extracting unique disease-values. This approach enabled disease-level age analysis using formula-based logic.  
**Validation (PivotTable Cross-Check):** To ensure completeness and accuracy, I created a PivotTable with Disease in Rows and Average of Age in Values. The PivotTable confirmed the calculated averages and revealed additional diseases with the same highest mean age that were not immediately apparent in the formula-based output.  
**Result:** Seven diseases share the highest mean age of 70 years:  Cholecystitis, Gout, Prostate Cancer, Schizophrenia, Testicular Cancer, Tonsillitis, William Syndrome.  
**Insight:** No single disease exclusively affects the oldest patient demographic. Instead, multiple conditions across different medical categories (urological, psychiatric, inflammatory, and genetic) exhibit similar age patterns. This suggests that healthcare screening and care strategies for patients around age 70 should be holistic rather than disease specific.

  <img width="488" height="313" alt="image" src="https://github.com/user-attachments/assets/6278e99d-4061-4f65-a16b-db2bd99a8a2f" />



**3. Which symptom (Fever, cough, fatigue, or difficulty in breathing) is the most common overall?**  
**Approach:** The dataset included binary Yes/No values for each symptom across all patient records. I used the COUNTIF function to count the number of "Yes" responses for each symptom column (Fever, Cough, Fatigue, Difficulty Breathing). Percentages were calculated by dividing each symptom count by the total number of patients (349)  
**Validation (PivotTable Cross-Check):** To validate the results, I created a PivotTable that aggregated symptom responses and confirmed the frequency counts for each symptom. The PivotTable output matched the COUNTIF results, verifying the accuracy of the calculations.  
**Result:** Fatigue was the most common symptom, reported by 242 out of 349 patients (69.3%).  
**Insight:** Since fatigue is the most prevalent symptom across all conditions, healthcare providers should prioritize fatigue assessment during patient intake. This finding suggests that screening protocols should include detailed questions about fatigue severity, duration, and impact on daily activities. Additionally, treatment plans may need to address fatigue management as a primary concern for patient quality of life.

  <img width="459" height="308" alt="image" src="https://github.com/user-attachments/assets/77ee5157-8247-44a9-982d-67063c17d438" />


**4.What is the gender distribution in the dataset?**  
**Approach:** The dataset included binary gender values (Male/Female). I used the COUNTIF function to count the occurrences of each gender and calculated their respective percentages based on the total patient count.  
**Validation (PivotTable Cross-Check):** To validate the gender distribution, I created a PivotTable with Gender in the Rows area and Count of Gender in the Values area. The PivotTable confirmed the gender counts and percentages, ensuring the distribution was accurately represented.  
**Result:** The dataset contained 176 female patients (50.4%) and 173 male patients (49.6%), showing a nearly equal gender distribution.  
**Insight:** The balanced gender distribution ensures that findings from this analysis are not skewed by gender bias. This makes the dataset suitable for identifying patterns that apply broadly across both male and female patient populations. If future analysis reveals gender-specific trends (such as certain diseases affecting one gender more than another), those findings would be statistically meaningful given this balanced baseline.

<img width="470" height="315" alt="image" src="https://github.com/user-attachments/assets/0f1cbff1-d07a-4521-af64-dbcbdb0df95d" />  


**5. What is the distribution of blood pressure levels (Low, Normal, High) among patients in the dataset?**  
**Approach:** The dataset included categorical blood pressure values (Low, Normal, High) for each patient. I used the COUNTIF function to count the number of patients in each blood pressure category and calculated percentages based on the total patient count.  
**Validation (PivotTable Cross-Check):** To validate the distribution, I created a PivotTable with diseases in the rows, blood pressure categories in the columns, and count of blood pressure in the Values area, which summarized the number of patient records classified as low, normal, or high blood pressure for each disease.  
**Result:**
**Low BP:** 18 patients (5.2%)  
**Normal BP:** 164 patients (47.0%)  
**High BP:** 167 patients (47.8%)  
Most patients had either normal or elevated blood pressure, with only a small percentage presenting with low blood pressure.  
**Insight:** The near-equal split between normal and high blood pressure patients (47% vs 48%) suggests that hypertension is a significant concern in this patient population. Healthcare providers should prioritize blood pressure monitoring and management protocols, as nearly half of all patients show elevated levels. The low percentage of patients with low blood pressure (5.2%) indicates that hypotension is relatively rare in this cohort, allowing providers to focus resources on hypertension management and cardiovascular risk reduction. 

<img width="452" height="311" alt="image" src="https://github.com/user-attachments/assets/39a56c64-0127-4ec6-ad5f-f0a82e132bed" />


**6. Are patients with difficulty breathing more likely to have a positive outcome compared to those without it?**  
**Approach:** The dataset included a binary indicator for difficulty breathing (Yes/No) and binary outcome values (Positive/Negative). I used Excel COUNTIFS logic to calculate the number of positive outcomes within each difficulty-breathing group. Percentages were calculated by dividing the number of positive outcomes by the total number of patients in each group.  
**Validation (PivotTable Cross-Check):** To validate the Excel calculations, I created a PivotTable with difficulty breathing status in the rows, outcome variable in the columns, and count of outcome Variable in the Values area. The PivotTable confirmed the distribution of positive and negative outcomes for patients with and without difficulty breathing and verified the calculated percentages.  
**Result:** Patients with difficulty breathing: 54/88 (61%) positive outcomes Patients without difficulty breathing: 132/261 (51%) positive outcomes. This represents a 10 percentage-point difference in positive outcome rates.  
**Insight:** Patients reporting difficulty breathing showed a higher rate of positive outcomes compared to those without difficulty breathing. This suggests that patients presenting with respiratory distress may receive more immediate or intensive clinical intervention, which could contribute to improved outcomes. However, further analysis would be required to control for disease severity and other confounding factors before drawing causal conclusions.  

<img width="401" height="304" alt="image" src="https://github.com/user-attachments/assets/162a2da7-189f-4338-bafc-ca726ecf3233" />


**Key Findings Summary**
This analysis revealed several important patterns:
1.Asthma is the most common disease (6.59% of patients)
2.Multiple diseases affect patients around age 70, suggesting the need for comprehensive geriatric screening
3.Fatigue is the most prevalent symptom (69.3%), indicating it should be a screening priority
4.The dataset contained 176 female patients (50.4%) and 173 male patients (49.6%), showing a **nearly equal** gender distribution.
5.Hypertension affects nearly half of patients (47.8%)
6.Patients with difficulty breathing showed higher positive outcome rates (61% vs 51%), possibly due to more aggressive intervention  
**Methodology Note:** _All analyses were cross-validated using PivotTables to ensure accuracy and completeness. This dual-method approach helped identify and correct initial calculation errors, demonstrating the importance of verification in data analysis._
</div>
