<img width="963" height="420" alt="image" src="https://github.com/user-attachments/assets/33f9742c-f134-445f-83a3-8e888f597f95" />
Let say the target of model is 85%, 1. they try one model RF, with one kind of cv input got 67%, like it goes on with variety of change in input format, cleanup, features, platform (windows, linux) change, model chanes, paameter changes.
what if i find my 3rd round of experiment results are good. then how can i go back and use same combinaton?
Every experiment round 
            1. we change parameters that need to save
            2. code version - model or algorithm change - github
            3. data set changes - dvc
            4. metrics get changes over the period
            5. artifact - generated model file - pkl - if store, we can go back use it
            6. system information - if we know what platform we use, then we can repeat to get same results.
               

# What is Experiment Tracking?

Experiment tracking is the process of **recording everything you do while training a machine learning model** so that you can:

    • Compare different models  
    • Understand what worked and what didn’t  
    • Reproduce a result in the future  
    • Share your results with others  

In machine learning, you rarely train a model just once.  
You try many combinations:

    • Different algorithms  
    • Different hyperparameters (learning rate, batch size, epochs)  
    • Different datasets  
    • Different preprocessing steps  

After a few tries, you forget which run gave the best accuracy.  
Experiment tracking solves this problem.

## What Do We Track?

A good experiment tracking system stores:

    • Parameters → example: learning_rate=0.01, epochs=20  
    • Code version → which Git commit you used  
    • Dataset version → which data file you used  
    • Metrics → accuracy, loss, RMSE  
    • Artifacts → trained model files, plots  
    • System info → OS, Python version, GPU/CPU  

### Real-World Example (Wine Prediction)

Suppose you're building a wine quality prediction model.

Run 1:
    • learning_rate=0.01  
    • accuracy=78%

Run 2:
    • learning_rate=0.05  
    • accuracy=84%

Run 3:
    • decision tree instead of linear regression  
    • accuracy=81%

If you don’t track these:
    You won't remember **why Run 2 was best** or **which settings produced it**.

Tools like MLflow, Weights & Biases, DVC Experiments, Neptune, etc., make this super easy.

### TL;DR

Experiment tracking = **keeping a record of all your model training runs**  
so you can compare, reproduce, and choose the best one.
