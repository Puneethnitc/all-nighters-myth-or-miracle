All-Nighters: Myth or Miracle?

Overview
This project analyzes the relationship between sleep patterns, academic stress, and academic performance using the Student Insomnia and Educational Outcomes Dataset.
The goal is to evaluate whether reduced sleep (commonly associated with all-nighters) can be compensated by academic effort, or whether the consequences of sleep deprivation outweigh any potential benefit.

The analysis is structured into three phases combining Exploratory Data Analysis (EDA) and regression modeling.
Dataset
Source: Student Insomnia and Educational Outcomes Dataset
Samples: 791 students
Target Variable: Academic performance (ordinal scale)
Key Variables Used
Sleep hours (sleep duration)
Sleep quality
Academic stress level
Difficulty concentrating due to lack of sleep
Impact of insufficient sleep on assignments
Class skipping due to sleep issues

Project Structure

Phase 1
  Focused on sleep hours vs academic performance
  Identified severe class imbalance in low-sleep categories
  Performed EDA using:
    Count plots
    Mean and median analysis
    Boxplots
  Conclusion:
  Sleep duration alone does not clearly separate academic outcomes, and imbalance limits direct modeling.

Phase 2
  Features:
    Sleep quality
    Academic stress level
  Methods:
    Exploratory data analysis
    Linear regression (baseline model)
    Train–test split with stratification
  Metrics:
    MAE ≈ 0.60
    R² ≈ 0.065
  Conclusion:
    Sleep quality and stress show weak but non-zero association with academic performance and are insufficient as standalone predictors.
Phase 3
  Features used together:
        Sleep hours
        Sleep quality
        Academic stress
        Concentration difficulty
        Assignment impact
        Class skipping
  Model:
    Linear Regression
  Evaluation:
    MAE ≈ 0.56
    R² ≈ 0.17
  Conclusion
  Academic consequence variables (concentration, productivity, attendance) dominate prediction, while sleep duration shows weak direct effect once these are included.

Final Conclusion

All-nighters are largely a myth rather than a miracle.
While reduced sleep may increase available study time, the resulting declines in concentration, productivity, and academic 
functioning outweigh any potential benefit. Sleep affects academic performance primarily indirectly, through its impact on cognitive and behavioral factors rather than through sleep duration alone.

Tools & Libraries
  Python
  Pandas
  Seaborn & Matplotlib
  Scikit-learn
