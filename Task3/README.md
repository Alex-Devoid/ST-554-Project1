Each group member should provide feedback on the other group members’ work. Be detailed and specific where possible. The quality of this feedback can play a part in your grade.

You can provide feedback to your group members in many different ways (live in a meeting, offline, or however else you devise) but the feedback must be documented here! 

Please replace “Feedback giver #x” with a group member’s name below and add feedback as a bulleted list below. Note: There is a pencil icon on the top right of the README file (when you are viewing the README.md file) that allows you to edit.

- Lanette Tyler
  + The variable CO(GT) is used in this analysis, as Dr. Post instructed in the instructions. Using PT08.S1(CO) instead makes more sense to me.  I noticed it when I originally read the project isntructions, but it doesn't come into play in Task2. There was a short discussion related to this in the project1 channel in slack, although it was about Task 1 instead of Task 3. The conclusion seemed to be to use PT08.S1(CO). Read the discussion and see what you think. 
  + The sum of the MSE's is used to evaluate the models in this analysis. From another discussion in the project1 channel in slack it seemed that Dr. Post meant the average instead of the sum. It wouldn't change the outcome, since X_slr, X_mlr, and y are all the same length, but check out the discussion to see what you think about that, too.
  + I was initially taken aback that you found the MLR with the weather conditions to be the better predictor. The correlation coefficients between benzene and the individual weather variables were low. Then I realized it was the time series inclusion that made the difference. The correlation coefficients are of all values without regard to time. I'll take another hard look at the time series visualizations included in the Task 2 notebook.
  + The coding and outputs looked great to me. Elegant coding, professional look to everything. This is the first time I've seen a Libraries Used list with explanations of the purpose. That's a very nice touch, especially for the audience.

- Alex Devoid
  - I appreciated how you described that your observation of `temporal trends and fluctuations`confirms that traditoinal cross validation would not be approriate. 
  - You could add for quick context, how many rows were droped when you `print(f"Rows remaining after removing -200 values: {len(df_clean)}")`.
  - In `df_clean['Date'] = pd.to_datetime(df_clean['Date'])`  adding `dayfirst=` would order days for you. Or you could sort by date before `df_daily['Day'] = range(1, len(df_daily) + 1)`.  
  - It is helpful to see the row count as a result of `print(f"Number of unique dates (rows): {len(df_daily)}")` after you calcuated the daily averages to contexualize how many days we are working with. You could also add how many days were removed for additional context.
  - You refernce `df_daily['Day']` in both cross-validation functoins (`day_col = df_daily['Day']` and `final_day = df_daily['Day'].max()`). You could pass the day series as arguments instead, so as to remove the global dependicy on `df_daily`. In general removing these types of global variables will allow for easier refactoring of the code in the future, if the fuctions were ever to get moved around, for example.
  - After you `print(f"SLR Total CV MSE: {cv_mse_slr:.4f}")` and `print(f"MLR Total CV MSE: {cv_mse_mlr:.4f}")`, you could also print an “average per prediction-day MSE” just to make the scale easier to interpret.  


