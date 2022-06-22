1. Implement/test your evaluation metric
Don't fly blind! Make sure you understand what "good" looks like.
It's also a good time to probe it and understand the flaws -- for instance,
AUC can be misleading on imbalanced datasets. Complicated metrics will require more testing.


2. Get a baseline
Start by guessing the mean, yesterday's value for time series, etc.
I like to start by knowing what accuracy I can get with a totally naive prediction.
Also, if you can estimate irreducible error at this stage, do it.


3. Start small
Start with a model that:
• Can give quick feedback (<10 minutes)
• Can beat my baseline
The most important thing at this stage with rapid iteration.
The best models are created by the data scientists that tried the most things.


4. Analyze your predictions
Now that you've done a bit of tweaking to beat your baseline, it's time to see what your model is
missing.
Save out your validation predictions and start slicing your data every way you can think
to see which subsets your model struggles with.


5. Tweak your model and iterate
Error analysis should surface some new improvements, so go try them!
At this stage, repeat steps 3-4 until you run out of things to try.


6. Find what scales
Finally, it's time to scale up.
This may mean including more data or grabbing the "large" variant of whatever model you're training.
You also can toy around with ensembling at this stage.
