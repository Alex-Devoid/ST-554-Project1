Each group member should provide feedback on the other group members’ work. Be detailed and specific where possible. The quality of this feedback can play a part in your grade.

You can provide feedback to your group members in many different ways (live in a meeting, offline, or however else you devise) but the feedback must be documented here! 

Please replace “Feedback giver #x” with a group member’s name below and add feedback as a bulleted list below. Note: There is a pencil icon on the top right of the README file (when you are viewing the README.md file) that allows you to edit.

- Emma Martinez
  - Your formatting and explanations in the markdown cells are very clear and thorough- I am able to follow your code pretty seemlessly. Your intrepretations for the grid search and gradient descent outputs stand out to me as particularly strong since they give context to connect the results back to sample average.
  - For the SLR gradient descent result in the "Run the line GD algorithm and compare to the usual regression solution" section, it looks like the b1 value is negative. From what I understand from the instructions, this is should be positive. I'm thinking increasing the b1 step size would help this land on the positive side and closer to Dr. Post's approximation
  - Otherwise, I think this is very well-written code and will be a strong component of our project.


- Lanette Tyler
  - In the data cleaning, values of -200 for CO(GT) are dropped. I think it should be values of -200 for  PT08.S1(CO) that are dropped. I think Dr. Post's Task 1 assignment had a typo on that step. There was a brief discussion about it in slack, and it makes more sense to do it that way since it's PT08.S1(CO) used in the rest of the code. Maybe that change would make the b1 value from the SLR gradient descent positive. (I haven't looked to see what the actual difference in dropped rows would be, if any.)
  - The negative value for b1 from the SLR gradient descent doesn't necessarily bother me. You used the same starting values he did. It is very close to zero, as is Dr. Post's positive value, so not far off even if the sign changes.
  - Copy editing:
    - Add a heading for the SLR Gradient Descent section
    - Delete the comma at the end of the first bullet point under "Evaluate RMSE across the grid and choose the best c" sub-heading
    - Drop the number six from "Grid search for SLR parameters (b0, b1)" sub-heading
  - You did a fabulous job with coding and explaning. The Gradient Descent description is particularly good - short, simple, and easy to understand.

