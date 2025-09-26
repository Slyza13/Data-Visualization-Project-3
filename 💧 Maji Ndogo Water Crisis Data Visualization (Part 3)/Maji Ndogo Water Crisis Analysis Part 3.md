### **Project Summary: Designing a User-Centric Dashboard for Maji Ndogo's Water Crisis**

**Objective:** To transition from exploratory data analysis to building a focused, actionable Power BI report tailored to the specific needs of decision-makers, namely the national president and provincial leaders.

---

#### **1. Adopting a User-First Design Philosophy**

The project shifted focus from technical data exploration to addressing the explicit needs of the end-users. This was achieved by developing **user stories** to guide the design.

*   **President Aziza's Needs (National Level):**
    1.  Understand the overall status of water access in Maji Ndogo.
    2.  Know the number of people affected by water challenges and the nature of those challenges.
    3.  Determine the total budget required for upgrades and how it will be allocated.
    4.  View all data at both national and provincial levels.

*   **Provincial Leaders' Needs:**
    1.  See data relevant only to their specific province.
    2.  Understand the scope of work and associated costs for their region.

#### **2. Structuring the National Dashboard for Clarity and Impact**

The national dashboard was organized into three logical sections to tell a compelling data story:

1.  **The Audience & Location:** This section visualizes the population of Maji Ndogo, split by urban and rural areas, and identifies their geographic distribution across provinces. The goal is to answer "Who are we helping and where are they?"
2.  **The Problem & Solution:** This section details the current state of water sources, showing the types of sources used and the specific improvements required (e.g., installing public taps, repairing infrastructure). It answers "What needs to be done and where?"
3.  **The Investment:** This section calculates and presents the total project budget, with breakdowns by province and improvement type. It answers "What is the cost?"

#### **3. Enriching Data for Deeper Insights**

To provide actionable metrics, significant data enrichment was performed using DAX formulas in Power BI:

*   **Budget Calculations:** A new `infrastructure_cost` table was integrated. A `Rural_adjusted_cost` column was added, applying a 50% cost increase for rural projects to account for higher logistical expenses.
*   **Key Performance Indicator (KPI) - Basic Water Access:** A crucial metric was created to measure project success based on UN standards. This involved a multi-step process:
    1.  Calculating the average queue time for each shared tap.
    2.  Creating a `Basic_water_access` column that classifies each water source as "Basic" or "Below Basic" based on criteria like water quality (for wells) and queue times (for shared taps).
    3.  Building a measure to calculate the percentage of the population with basic water access, providing a clear, overarching goal for the project.

#### **4. Enhancing Interactivity and User Experience**

To manage information density, advanced Power BI features were implemented:

*   **Interactive Budget Toggle:** Buttons were created to allow users to switch between two views within the budget section: one showing a breakdown by **Province** and another by **Improvement Type**. This was achieved using Power BI's **bookmark** functionality to show/hide specific visuals, creating a dynamic and uncluttered interface.
*   **Drill-Through Pages:** Provincial-level pages were created. Users can right-click on a province in the national report and "drill through" to a detailed page customized for that province's leader, enabling localized decision-making.

#### **5. Focusing on Actionable Metrics**

The report header was designed to display high-impact summary statistics (like large-number "KPI cards") that answer the most critical questions at a glance:
*   Total estimated budget required.
*   Current percentage of the population with basic water access.
*   The projected improvement in access after project completion.

#### **6. Conclusion: An Iterative Approach to Data Storytelling**

The final design prioritizes delivering a functional and understandable tool to the users quickly. The philosophy is that it is more effective to get a usable report into the stakeholders' hands and iterate based on their feedback than to strive for perfection in isolation. The dashboard is now poised to become the central tool for planning and executing the water infrastructure upgrades in Maji Ndogo, directly supporting data-driven governance.

***

**Disclaimer:** This summary is an original synthesis of the data visualization and dashboard design concepts described in the source material. It demonstrates an understanding of user-centric design, data modeling, and interactive reporting principles without reproducing the specific content.