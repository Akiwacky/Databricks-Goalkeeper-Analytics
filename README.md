# Discovering Europe's Top Goalkeeper: A Data-Driven Analysis

In the world of football, the debate over who reigns supreme in any position is a favorite pastime among fans. Recently, a discussion with a friend prompted an intriguing question: who is the best goalkeeper in European football at the moment? As someone who values objectivity over bias, I realized that relying solely on personal observations wouldn't suffice due to the vast number of matches across European leagues. Thus, I turned to data analysis to find an answer.

## Setting the Criteria

The first step was to establish the metrics or statistics that best evaluate a goalkeeper's performance. After careful consideration, I identified the top five metrics as follows:

1. **Save Percentage**: This metric indicates the goalkeeper's effectiveness in stopping shots on target, a fundamental skill for any goalkeeper.
2. **Clean Sheet Percentage**: Reflecting not just the team's defensive strength but also the goalkeeper's contribution, this metric shows how often a goalkeeper maintains a clean sheet.
3. **Goals Against per 90 Minutes**: This measures the average goals a goalkeeper concedes in a full match, offering insight into their reliability.
4. **Crosses Stopped**: A goalkeeper's command of the box is crucial, and this metric highlights their ability to prevent opportunities from crosses.
5. **Post-Shot Expected Goals minus Goals Allowed per 90 Minutes (PSxG-GA)**: As an advanced metric, PSxG-GA estimates the quality of shots faced and the expected goals conceded, subtracted by the actual goals conceded per 90 minutes, showcasing a goalkeeper's skill in preventing goals above expectation.

## Data Collection

With the criteria set, the next phase was data collection. For robust and reliable football statistics, Fbref stands out as a premier source. Utilizing Python, I extracted relevant data from Fbref and saved it to a CSV file, ready for analysis in Databricks. The process of extracting this data is detailed in a [repository](XXX).

## Cleaning and Preparing Data

Upon acquiring the data, the necessary steps of cleaning, transforming, and preparing it were undertaken. Understanding the importance of each metric, we assigned weights according to their perceived significance, which, admittedly, introduces a subjective element that could be adjusted:

- Save Percentage (30%)
- Clean Sheet Percentage (25%)
- Goals Against per 90 Minutes (20%)
- Crosses Stopped (10%)
- PSxG-GA per 90 Minutes (15%)

## The Analysis

After applying the weights and calculating the overall scores, we ranked the goalkeepers based on their cumulative scores. The analysis revealed that Yann Sommer stood out among his peers, topping the list as the best goalkeeper in European football according to our metrics.

## Conclusion

This analysis, while straightforward, was an insightful exercise in utilizing Databricks and PySpark for data analysis within the realm of football. It's important to note that the metrics chosen and their weights reflect one way to evaluate goalkeepers, and other factors such as the quality of opposition, defensive strategies of the team, and variances in league styles can significantly affect these metrics. For a more nuanced evaluation, these additional factors should be considered. However, for the purpose of gaining experience and learning with Databricks, this simplified analysis served its goal well, highlighting Yann Sommer as a standout goalkeeper through a data-driven lens.

### Note

This analysis is intended as a learning exercise in the field of data analysis with Databricks and PySpark. It highlights the potential and importance of data in understanding football performance and opens the door to more comprehensive and detailed analyses in the future.
