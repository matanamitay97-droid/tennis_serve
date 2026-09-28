**🎾 ATP 2024 Serve Analytics: Does 1st serve percent actually makes you win?**
Welcome to the data-driven side of tennis! This project dives into the 2024 ATP tennis season data to answer a classic question: what separates the winners from the losers when it comes to serving?

Using R, we clean, wrangle, visualize, and statistically test match metrics to find out just how much a solid first serve impacts victory.


**🚀 What's Inside the Pipeline?**
Data Engineering: Slices and dices raw match stats (atp_matches_2024_no_RET.csv) to calculate key performance indicators:

First & second serve success rates (1sv_percent, 2sv_percent)

First & second serve win percentages (1sv_w_percent, 2sv_w_percent)

Ace and double fault rates

Tidy Data Magic: Restructures the data into a clean, long-format dataset (long_data) tagged by player_type ("Winner" vs. "Loser").


**Visualizations (ggplot2):**
Boxplots + jittered points comparing winner vs. loser serving stats at a glance.

High-resolution histograms to check data distributions (because normality checks are important!).

Saves clean publication-ready charts (like 1sv.pdf).

Stats & Effect Sizes:

Runs Welch's t-tests to check for statistical significance.

Calculates Cohen's d using the effsize package to see just how massive the performance gap is.


**📦 Prerequisites & Libraries**
Make sure you have R installed along with these packages:
install.packages(c("tidyverse", "effsize"))


**🎯 How to Run**
Drop your atp_matches_2024_no_RET.csv file into the project directory.

Fire up RStudio, open the R Markdown script, and hit Knit or run the chunks to let the code do its magic!
