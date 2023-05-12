# Catherine-Project-2.0

Your business problem and stakeholders: 
- My business problem is determining who is more likely to suffer a stroke by seeing what sypmtoms these people have in common. My stakeholders are the drug companies that are trying to develop medicine to help prevent strokes.

The source of your data:
- the source of my data is from the kaggle website and the actual data is from numerous hospitals and studies.

A description of your data:
- My data is showing the symptoms of people who are more likely to have a stroke. It shows how having a higher BMI, hypertension, heart disease is more likely to lead to a stroke. 

2 analytical insights from your data analysis.
fig, axes = plt.subplots(ncols=2, sharey=True, figsize=(12,5))
sns.stripplot(data=stroke_df, x='hypertension', y='heart_disease',ax=axes[0],
                   hue='gender', edgecolor='white', linewidth=1);
                   
                   ax = sns.barplot(data=stroke_df, x='hypertension', y='heart_disease', hue='gender');
ax.set_title("Reasons why someone can get a stroke");

These two graphs show how it doesn't matter if it is male or female, if the person has high hypertension and heart disease then they are more likely to have a stroke. 


The metrics for your best model
- Here are the metrics for my best model: 

A description of how well your model would solve your business problem
- This model shows if we can target these specific sypmtoms than we can help develop a drug that can help prevent a stroke.

A summary with at least 2 recommendations for your stakeholders, based on your model performance AND analytical findings.
1. My first recommendation would be to develop a drug that can target both hypertension and heart disease that would decrease both, due to my analtyical insight in my first graph. 
2. My second recommendation would be to create a drug that would just target hypertension and to decrease it. Decreasing hypertension would than decrease heart disease as well, and that shows in both of my graphs. 