# 🔫 FBI NICS Firearm Background Check Data 📊

The data in this repository comes from the [FBI's National Instant Criminal Background Check System (NICS)](https://www.fbi.gov/about-us/cjis/nics). 🔍

---

### 📜 Background

> 🏛️ **Mandated by the Brady Handgun Violence Prevention Act of 1993**, the NICS was launched by the FBI on **November 30, 1998**. It helps **Federal Firearms Licensees (FFLs)** instantly determine whether a prospective buyer is eligible to purchase firearms or explosives. 🛒🔍 Before completing a sale, cashiers must check with the FBI or designated agencies to ensure the customer **does not have a criminal record or other disqualifying factors**. 🚫⚖️

📌 **Fast Facts:**
✅ Over **100 million** background checks conducted in the last decade  
🚫 More than **700,000** denials issued  

---

### 📊 About the Data

The FBI provides firearm check data by **month, state, and type**—but unfortunately, it's only available as a **PDF**. 😖📄 The code in this repository **downloads, parses, and converts** that PDF into a more usable **spreadsheet/CSV format**. 💾📈

🔗 **[Click here to download the data](data/nics-firearm-background-checks.csv?raw=true)** *(November 1998 – January 2025)*

---

### 📌 Important Notes & Caveats ⚠️

The original FBI report includes **important disclaimers** you should review. One of the most crucial is:

> ❗ These statistics represent the number of **firearm background checks initiated** through the NICS. They **do not** represent the **number of firearms sold**. A one-to-one correlation **cannot** be made between a background check and a firearm sale. 🔄🔫

### 📰 Additional Context

📢 A 2015 article from *The Trace* highlighted that **not all background checks are tied to gun sales**:

> 🔄 Many checks are for **concealed carry permits**, not actual firearm purchases.  
> 🔁 Kentucky, for example, **reruns checks monthly** for all concealed carry license holders.  
> 📋 **Private gun sales** often **do not require background checks**, affecting total numbers.  

📑 A **2017 study** published in the *Annals of Internal Medicine* surveyed 1,613 gun owners and found that **22%** of recent firearm acquisitions were made **without a background check**. 📊

---

### 🔎 Methodology & Sales Estimation 🛠️

Not all categories of background checks provide a **clear picture** of gun sales. When *The New York Times* analyzed NICS data in **Dec. 2015**, they noted:

> 📌 **Sales estimates** are based on **handgun, long gun, and multiple-gun background checks**.  
> 🏛️ **Permit checks** and other categories are **excluded**.  
> ⚖️ Due to differing **state laws**, sales figures **cannot be directly compared** across states.  

📊 **NYT’s Calculation Method:**

- 🏹 Each **long gun & handgun check** = **1.1 sales**  
- 🔫 Each **multiple-gun check** = **2 sales**  
- 🚫 **Permit checks & other categories omitted**  

*(Methodology adapted from the **[Small Arms Survey](http://www.smallarmssurvey.org/fileadmin/docs/F-Working-papers/SAS-WP14-US-Firearms-Industry.pdf)** by Jurgen Brauer, Georgia Regents University.)*

---

### 📚 Additional Resources 🔗

📘 **[NICS Federal Firearms Licensee Manual](https://www.fbi.gov/file-repository/nics-firearms-licensee-manual-111811.pdf/view)** – Comprehensive guide to NICS background checks.  

🗺️ **[NICS Participation Map](https://www.fbi.gov/file-repository/nics-participation-map.pdf/view)** – Visual representation of each state's participation level with the NICS.  

# Some Example Visualizations From the Data

### Other Guns Checks by State with Tooltip by Year  

This first visualization presents the total number of background checks for firearms categorized as "Other" across different U.S. states. The data is aggregated by state, showing trends over time.  

- **Y-Axis:** Sum of "Other" category firearm background checks  
- **X-Axis:** States  
- **Tooltip:** Displays the total number of "Other" gun background checks for each specific year based on the date of acquisition.  

This allows for both a high-level comparison between states and a more detailed year-over-year trend when hovering over data points.

![Other Guns with By Year Tooltip](image.png)


### United States Map Distribution of Total Gun-Related Check Activities  

This next visualization displays the total number of firearm-related background check activities across U.S. states using a shape map.  

- **Visualization Type:** Shape map of the United States  
- **Data Representation:** States are color-coded based on the total number of firearm-related background checks.  
- **Metric:** Sum of all gun-related check activities per state.  

This provides a geographic overview, allowing for quick identification of states with higher or lower firearm background check activity.

![Gun Activity Shapemap](image-1.png)


### COVID-19 Cases Summed by Month  

This visualization presents the total number of COVID-19 cases reported in the United States, aggregated by month.  

- **X-Axis:** Months  
- **Y-Axis:** Total number of COVID-19 cases  
- **Visualization Type:** Line chart showing the trend of COVID-19 cases over time  

This data helps illustrate the rise and fall of COVID-19 cases across different months. Additionally, it provides context for analyzing potential connections between the onset of the pandemic and changes in firearm-related background check activities, particularly in early 2020 when uncertainty and public concerns may have influenced gun purchases.

![Gun Activity Connection to Covid Pandemic](image-2.png)


### Permit Data by State and Year  

This visualization displays the total number of firearm permit background checks across U.S. states, broken down by year.  

- **Visualization Type:** Sparkline chart with independent Y-axes for each state  
- **X-Axis:** Years  
- **Y-Axis:** Sum of permit-related background checks  
- **Nested Data:** Yearly trends of permit background checks per state  

The visualization highlights fluctuations in firearm permit checks over time. Many of the larger spikes in the data can be attributed to legislative changes, as new laws or policy shifts often lead to surges in permit applications. This provides insight into how regulatory changes impact firearm-related background check activity across different states.

![Permit Data by State and Year](image-3.png)


### Disparity of Handguns and Long Guns by State  

This visualization presents the difference in firearm-related background check activities between handguns and long guns across different U.S. states.  

- **Visualization Type:** Bar chart  
- **X-Axis:** States  
- **Y-Axis:** Sum of the difference between handgun and long gun background checks  
- **Metric:** Positive values indicate more handgun-related activity, while negative values suggest higher long gun-related activity  

This chart highlights the disparity in firearm preferences across states, showing whether a state has a stronger association with handgun or long gun background checks. The differences may be influenced by factors such as hunting culture, self-defense trends, or state-specific regulations.

![Disparity of Long and Hand Gun Spread](image-4.png)

