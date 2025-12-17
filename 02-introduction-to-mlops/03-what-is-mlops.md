# What is MLOps?

Before understanding MLOps, it’s important to understand **where it comes from**.

MLOps is **directly inspired by DevOps**.

Just like DevOps transformed how we build and operate software, **MLOps brings those same principles into the Machine Learning world**.

---

## How DevOps Inspired MLOps

### What DevOps Solved

Before DevOps:
- Developers wrote code
- Ops teams deployed and maintained it
- Deployments were slow, manual, and risky
- Failures were hard to debug

The above process they need to repeat atleast 5 to 6 times to deploy into production. like they need develop in dev env, test it, then SIT, then UAT, then Test, then Production etc., so if they manually follow above steps it takes lot of time.

DevOps introduced: Devops is a unified activitiy, these priniciples are standarized by industry and created certain process implementing via automtion tool and technologies:

- Automation
- CI/CD pipelines
- Infrastructure as Code
- Monitoring and feedback loops
- Shared ownership between Dev and Ops

The result:
- Faster releases
- More reliable systems
- Continuous improvement

---

## The Same Problem Happened in Machine Learning

In ML, a similar gap appeared:
I a company they trying to create a model for recommendation engine, they spend time 

          1. collect data set
          2. create model
          3. trin and eval
          4. package
          5. save.

Then they take help from operations team help to

          1. create api
          2. deploy in k8s
          3. create Load balancer
          4. create CDN

overall this whole process iterate 10 - 20 times untill the accuracy reach and also it need ship from Dev to prod.

- Data Scientists trained models in notebooks
- Models worked locally
- Production teams struggled to deploy them
- No clear ownership after deployment
- Models degraded silently over time

Just like Dev vs Ops, ML had a gap between:
- **Model development**
- **Model operations**

That gap is what **MLOps** was created to solve.

---

## MLOps = DevOps Practices for Machine Learning

MLOps takes proven DevOps ideas and applies them to ML systems.

| DevOps Concept | MLOps Equivalent |
|----------------|------------------|
| Source code versioning | Data + model versioning |
| CI pipelines | Model training pipelines |
| CD pipelines | Automated model deployment |
| Monitoring services | Monitoring model performance |
| Rollbacks | Model version rollback |
| Automation | End-to-end ML lifecycle automation |
