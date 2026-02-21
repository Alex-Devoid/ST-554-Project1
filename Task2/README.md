Each group member should provide feedback on the other group members’ work. Be detailed and specific where possible. The quality of this feedback can play a part in your grade.

You can provide feedback to your group members in many different ways (live in a meeting, offline, or however else you devise) but the feedback must be documented here! 

Please replace “Feedback giver #x” with a group member’s name below and add feedback as a bulleted list below. Note: There is a pencil icon on the top right of the README file (when you are viewing the README.md file) that allows you to edit.

- Emma Martinez
  - This is a very thorough and well-written EDA. The list of variables and their units was a nice touch that would help give the audience valuable context.
  - For the scatter plots, maybe using ax.scatter in favor of ax.plot would produce a cleaner visualization for the continuous relationships.
  - Under Multivariate Summaries → True C6H6 and Weather Conditions → Means and Standard Deviations of True C6H6 by Weather Condition Levels, in the cell that says "The mean C6H6 is about 2 lower for the C6H6, which is pretty small, and the standard deviation is the same.", doesn't specify which group, high or low temp, has the lower mean. A small little tweak but helpful for clarity.
  - Overall this is a very well-written notebook and satisfies all the requirements of task 2 perfectly. 


- Alex Devoid
  - I was able to follow the story of what you explored and why.
  - Your cleaning choices make sense, and I like that you checked `air_qu.isin([-200.0]).any()` first before changing anything. It shows that `-200` is actually present, before doing additional processing. 
  - I like how you explained the output of `air_qu.true_C6H6.describe()[1:].round(2)`. One improvement could be to add a sentence or two in plain language about what those numbers imply, for a non-technical reader, if possible. (for example: what the mean suggests as a typical value anything additional context about the spread).

  - In the `Scatter plots of true C6H6 vs. environmental pollutant sensor readings` section, the plots would be easier to read if the points were plotted as individual scattered points instead of being connected with lines, to more clearly show the relationship between the variables.
  - I think a short interpretation right after every plot/table is needed.
  - I don’t think the `FutureWarning: The default of observed=False is deprecated...` messages hurt the analysis, but I’d remove them for a non-technical audience. Those warnings can look like an error to the uninformed.
  - In the conclusion, you could add one sentence that explicitly names which variables look most promising for prediction, and tie it directly back to the correlation results and the scatterplot patterns.