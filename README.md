# Influenza Surveillance Dashboard Chicago
 This project is an interactive **Power BI dashboard** built using the [City of Chicago Influenza Surveillance Dataset](https://data.cityofchicago.org/Health-Human-Services/Influenza-Surveillance-Weekly-Historical/6xmk-qk57/data_preview).  
It provides insights into influenza testing, positivity, risk levels, subtypes, and ICU admissions across multiple flu seasons.

---

## Dataset
- **Source:** [Influenza Surveillance Weekly - Historical](https://catalog.data.gov/dataset/influenza-surveillance-weekly)
- **Frequency:** Weekly historical influenza surveillance data  
- **Time range:** 2015–2016 through 2023–2024 (9 flu seasons)
- **Metrics include:**  
  - Flu tests and positive cases 
  - Influenza A & B totals  
  - Influenza A subtypes (H1N1, H3N2, Not Subtyped)  
  - Risk level categories (Low, Increasing, Decreasing, High)  
  - ICU admissions and pediatric deaths
- For detailed descriptions of each column, see the [official data dictionary](https://data.cityofchicago.org/Health-Human-Services/Influenza-Surveillance-Weekly-Historical/6xmk-qk57/about_data).

---

## How to Open the Power BI File  

To view the interactive dashboard:  
1. Download the `.pbix` file from this repository.  
2. Install **[Power BI Desktop](https://powerbi.microsoft.com/desktop/)** (free from Microsoft).  
3. Open Power BI Desktop, go to **File > Open**, and select the `.pbix` file.  
4. The full dashboard with all pages and filters will load for exploration.  

**Note**: The dataset is already included in the `.pbix` file. You do not need to reconnect or refresh the data unless you want the most recent records.  

### Alternative View (Static PDF)  
If you do not have Power BI Desktop, a **PDF version** of the dashboard is also provided in this repository.  
- The PDF allows you to view all pages of the dashboard.  
- However, it is **not interactive**, so filtering and drill-down features available in Power BI will not work.  

---

## Power BI Dashboard
### Page 1 – Flu Surveillance Chicago Overview
Big-picture trends across flu seasons:
- Sum of Lab Flu test by Season and Risk Level 
- Sum of Positive Lab Flu Test by Season
- Influenza A vs B comparison
- Sum of ICU admissions and Risk Level
  
<img width="1433" height="851" alt="image" src="https://github.com/user-attachments/assets/7393daa2-cb76-4920-ae3f-9a01fab71dc5" />

#### Insights – Plot 1: Lab Flu Tests by Season and Risk Level
- The number of lab flu tests increased significantly from 26k in 2015–2016 to 217k in 2023–2024.
- Across seasons, test results were classified into varying flu risk levels (low, increasing, decreasing, high).
- Notably, during 2020–2021 and 2021–2022, almost all lab tests were classified as low risk despite large testing volumes (43k and 198k).
- This pattern may suggest effective influenza control measures in those seasons, possibly due to broader vaccination coverage or reduced flu severity, where positive cases represented only minor illnesses rather than severe outbreaks.
#### Insights - Plot 2: Positive Lab Flu Test by Season
- In 2015–2016, the positive lab flu tests started at 1.6k out of 26k total tests, rising to 11.3k out of 217k in 2023–2024.
- The highest point in this line chart is 12.8k positive tests out of 198k total in 2022–2023.
- The lowest point is 15 positive tests out of 43k total in 2020–2021.
#### Insights - Plot 3: Flu A and B by Season
- This plot shows how influenza A and B were distributed across seasons, from 2015–2016 to 2023–2024.  
- Influenza A consistently dominates over influenza B, suggesting that Flu A subtypes are more common and that more people were infected with Flu A than Flu B in Chicago.  
- Similar to Plot 2, about 12.4k people tested positive for Flu A in 2022–2023, making it the highest data point and showing that most positive lab tests that season were driven by Flu A.  
#### Insights - Plot 4: ICU Admissions by Season and Risk Level
- The plot illustrates the number of ICU admissions from 2015–2016 through 2023–2024.  
- The highest number of ICU admissions occurred in 2017–2018 with 583 admissions, while the lowest occurred in 2020–2021 with only 2 admissions.  
- 2020–2021 stands out as an exceptional year: there were 43k low-risk lab tests, only 15 positive cases out of those 43k, and just 2 ICU admissions.  
- Similarly, 2021–2022 also shows favorable results, with 198k low-risk lab tests and only 52 ICU admissions classified as low risk.  
- More importantly, we need to focus on the two critical flu seasons: 2017–2018 and 2019–2020.  
  - 2017–2018 had the highest ICU admissions across all nine seasons (583 admissions), with 362 classified as high-risk.  
  - 2019–2020 recorded the highest number of high-risk ICU admissions, with 414 out of 480 admissions classified as high-risk.  
- These patterns suggest that it is important to examine what happened during these two seasons and identify precautionary measures that could help reduce the number of ICU admissions, especially those classified as high-risk.  

### Page 2 - Flu Risk Level by Season
Detailed look at flu risk level across seasons.
- Decreasing and High Risk Level 
- Decreasing and Increasing Risk Level
- High and Increasing Risk level
- Low Risk Level
  
<img width="1427" height="855" alt="image" src="https://github.com/user-attachments/assets/9cf219fb-84c2-4a1f-bea7-db09ea45c941" />

#### Insights - Plot 5: Decreasing and High Risk Level by Season
- In this plot, we are comparing decreasing and high flu risk levels.  
- The line for decreasing flu risk level increased steadily from 5k in 2015-2016 to 77k in 2023-2024, which is a positive sign.  
- The line for high flu risk level started at 2k in 2015-2016, rose sharply to 50k in 2022-2023, but then dropped dramatically to 13k in 2023-2024. This indicates that there might have been effective practices or interventions that helped reduce high-risk flu cases in 2023-2024.  
#### Insights - Plot 6: Decreasing and Increasing Risk Level by Season
- This plot compares decreasing and increasing flu risk levels.  
- The line for increasing flu risk level started at 8k in 2015-2016 and rose to 43k in 2023-2024.  
- However, it remains lower than the decreasing flu risk level in 2023-2024, which reached 77k.  
- This suggests that while increasing risk cases are growing, efforts to manage flu risk may be successfully shifting more cases into the decreasing category.
#### Insights - Plot 7: High and Increasing Risk Level by Season
- This plot compares high and increasing flu risk levels.  
- Although increasing flu risk levels rose to 43k in 2023-2024, high flu risk levels dropped sharply to 13k in the same season.
#### Insights - Plot 8: Low Risk Level by Season
- This plot illustrates low flu risk levels.  
- The line starts at 11k in 2015-2016, peaked at 198k in 2021-2022, and then decreased to 84k in 2023-2024.  
- However, the number of low risk cases in 2023-2024 still remained higher than increasing risk (43k) and high risk (13k) in the same season.  
- When combined with decreasing risk levels (77k) in 2023-2024, this suggests a positive sign of effective precautionary practices against flu during that season.

### Page 3 - Flu Subtype by Season
Detailed look at Flu B and Flu A with its subtypes.
- Flu A Subtypes and Not Subtype
- Flu B
- Flu H3N2 (Subtype A)
- Flu H1N1 (Subtype A)
- Not Subtype (Flu A)
  
<img width="1425" height="852" alt="image" src="https://github.com/user-attachments/assets/0bf0b460-6f89-43ee-9d1d-006a70eb50a7" />

#### Insights - Plot 9: Flu A Subtypes and Not Subtypes by Flu Season
- This plot illustrates the distribution of Flu A subtypes (H1N1, H3N2) and not subtyped cases from 2015-2016 to 2023-2024.  
- In 2015-2016, the bar chart is dominated by Flu A H1N1, which accounted for 79.19% of reported cases.  
- From 2017-2018 to 2023-2024, the majority of the bar is dominated by Not Subtyped A, increasing from 66.53% in 2017-2018 to 83.77% in 2023-2024.  
- This indicates that in recent flu seasons, most Flu A cases could not be classified into a specific subtype, suggesting challenges in identifying or recording exact Flu A subtypes.

#### Insights - Plot 10: Flu B by Flu Season
- This line plot shows the number of positive Flu B cases by season, from 2015-2016 to 2023-2024.  
- The number of positive Flu B cases started at 162 in 2015-2016 and rose to 3.2k in 2023-2024.  
- Notable spikes occurred in 2019-2020 (2.6k cases) and again in 2023-2024 (3.2k cases), indicating peak Flu B activity in these seasons.  
- The lowest number of Flu B cases was recorded in 2020-2021, with only 2 cases across the entire season.  

#### Insights - Plot 11: Flu H3N2 (Subtype A) by Season
- This plot shows the number of positive Flu H3N2 (Subtype A) cases across flu seasons from 2015-2016 to 2023-2024.  
- The number of cases started at 55 in 2015-2016, peaked at 1.98k in 2022-2023, and then dropped to 521 in 2023-2024.  
- The lowest point was recorded in 2020-2021 with only 3 cases.  
- After very low activity in 2020-2021 and 2021-2022, Flu H3N2 increased sharply again in 2022-2023.  

#### Insights - Plot 12: Flu H1N1 (Subtype A) by Season
- This plot shows the number of positive Flu H1N1 (Subtype A) cases across flu seasons from 2015-2016 to 2023-2024.  
- The number of cases started at 1.1k in 2015-2016, dropped sharply to 23 in 2016-2017, and then surged to its highest point of 1.3k in 2019-2020.  
- The lowest point occurred in 2020-2021, with only 5 cases, followed by a gradual rebound reaching 793 in 2023-2024.  

#### Insights - Plot 13: Not Subtype (Flu A) by Season
- This plot shows the number of positive Flu A cases that were not subtyped across flu seasons from 2015-2016 to 2023-2024.  
- The number of cases started at 242 in 2015-2016, rose to 2.9k in 2017-2018, and dropped to the lowest point in 2020-2021 with only 5 cases.  
- The highest point occurred in 2022-2023 with 10.1k cases, followed by a decline to 6.8k in 2023-2024. This indicates that a substantial number of Flu A cases remain unclassified into specific subtypes.  
- The counts of non-subtyped Flu A are consistently higher than those of Flu B, H3N2, and H1N1 (Subtype A), highlighting a major gap in subtype identification.

### Page 4 - ICU Admissions for Influenza
Detailed look at ICU admissions for Influenza
- ICU Admissions and Positive Lab Flu Test
- ICU Admissions Low Risk Level
- ICU Admissions High and Increasing Risk Level
- ICU Admissions Decreasing and High Risk Level
  
<img width="1428" height="855" alt="image" src="https://github.com/user-attachments/assets/b471a80a-6192-4861-b2fb-a2afc1109b7a" />

#### Insights - Plot 14: Sum of ICU Admissions vs Positive Lab Flu Test by Season
- This plot shows a comparison between ICU admissions and positive lab flu tests across seasons, from 2015-2016 to 2023-2024.  
- Compared to the positive lab flu tests across seasons, the number of ICU admissions remains relatively low, which is a positive sign.
  
#### Insights - Plot 15: ICU Admission Low Risk Level
- This line plot shows ICU admissions for low risk levels from 2015-2016 to 2023-2024.  
- The line started at 15 in 2015-2016, dropped to 8 in 2016-2017, and then rose to 20 in 2018-2019.
- It then declined to 2 in 2020-2021, peaked sharply at 52 in 2021-2022, and decreased again to 13 in both 2022-2023 and 2023-2024.

#### Insights - Plot 16: ICU Admissions - High vs Increasing Risk Level
- This plot shows a comparison between ICU admissions with high and increasing risk levels, from 2015-2016 to 2023-2024.  
- The line for high-risk ICU admissions started at 58 in 2015-2016, rose to 362 in 2017-2018, dropped to 219 in 2018-2019, peaked at 414 in 2019-2020, and then fell to 60 in 2023-2024 — a positive sign for influenza control.  
- The line for increasing-risk ICU admissions began at 162 in 2015-2016, dropped to 45 in 2017-2018, slightly rose to 75 in 2018-2019, declined again to 14 in 2022-2023, and increased slightly to 92 in 2023-2024.  
- Overall, high-risk ICU admissions showed sharper fluctuations compared to increasing-risk ICU admissions, suggesting that high-risk cases tend to surge more dramatically during severe flu seasons.

#### Insights - Plot 17: ICU Admissions – Decreasing vs High Risk Level
- This plot compares ICU admissions between decreasing and high-risk levels, from 2015-2016 to 2023-2024.  
- The line for decreasing-risk ICU admissions started at 45 in 2015-2016, slightly declined to 25 in 2016-2017, then rose sharply to 162 in 2017-2018. It later dropped to 9 in 2022-2023 before increasing again to 137 in 2023-2024.  
- In contrast, high-risk ICU admissions consistently remained higher across the seasons, highlighting the stronger burden of severe flu cases compared to decreasing-risk admissions.  

---

### Conclusion
From 2015–2016 to 2023–2024, flu testing in Chicago rose sharply, from **26k** tests to over **217k**. Positive flu cases peaked at **12.8k** in 2022–2023, though severity has recently declined. High-risk ICU admissions were highest in 2017–2018 (**583 cases**) and 2019–2020 (**414 high-risk out of 480**), but dropped to just **60** in 2023–2024, while low- and decreasing-risk cases became more common. Influenza A consistently dominated over Flu B, with subtype spikes in H1N1 and H3N2, though most Flu A cases in recent years were left unclassified.

### Final Takeaway
Chicago’s flu trends show progress: more testing, fewer severe cases, and better outcomes in recent years. Still, high unclassified rates for Flu A highlight the need for continued monitoring and stronger diagnostic precision.
