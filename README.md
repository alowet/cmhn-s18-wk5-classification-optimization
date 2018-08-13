# cmhn-s18-wk4-dimensionality-reduction
Perform hyper-parameter optimization and other pipeline analysis procedures

Read through and perform the analyses described in the notebook. Complete all of the **Exercises** described in the text. **Self-study** indicates an optional tangent that can help you to flesh out your knowledge of the content covered in this course.

When you are satisfied, commit your changes to this repo. It will automatically be submitted tomorrow at noon.


*Instructor's corner*

Feedback:
Ex 2: Your cost parameter is set inappropriately which is why the values are in such a low range.  
Ex 4: that is one possible solution but as you say you might miss the global optima if the parameters are not independent. Instead the idea is to 'follow the gradient' of good results: if changing the parameter in one direction produces better results then we keep moving in that direction until the results no longer improve.  
Ex 6: Good answer.   
Ex 7: With small datasets like this we want to stratify our training/test splits to ensure that the classifiers are as balanced as possible and that your training/test sizes are sufficiently large. Hence using KFold for your nested loop can result in issues (as manifested in your low classification results).  By looping over both the inner and outer cv 10 times, you are doing this analysis more than 10 times (since each fold of the outer loop counts as 1 time of doing it). However I admit the language in the question here was vague.  
Ex 8: Great answer.  
Ex 10: In param_grid you can list the different parameter values in the same list. You do PCA in all of your pipelines rather than doing a grid search over it.

5/5
