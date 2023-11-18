# Testing-Monitoring-ML-Deployments

## Introduction
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/10750c09-d3b0-40ef-84e2-5a1346b48e4e)
Machine Learning in Production Pipeline </br>

This repository contains details about ML Testing, Shadow Mode Interpretation, and Monitoring. </br>

### Continuous Delivery for Machine Learning: https://martinfowler.com/articles/cd4ml.html

## Model Lifecycle
### Deploying a model to production
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/33689481-ecbf-40d5-a82d-a97ba8164974)

The deployment of a model is a process of making our model available in a working production environment where it can provide prediction systems to other software systems. Research Environment is not in contact with Live Environment and live data.

### Deployment of Machine Learning Pipeline
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/4b41eb93-c281-4daf-adf2-5d10ba08d7f8)

ML Pipeline is a series of steps that must occur from the movement we receive the data to the movement we obtain the prediction. 
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/ade175c8-2973-4a0e-9f18-b3c31357bb9d)

### 3 Scenarios deploying a model to production
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/299037a8-22d7-4c9e-8306-271ce11857ab)

### Use Case Scenario
Replacing an existing live model. Here, we see a model to predict house sale prices. </br>

### Deploying the first ML model
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/ff43b576-85fa-4c55-b5ee-e8d9059964f3)
Here we replace our current model with a new model which is better one. In our case, we replaced the linear regression model with a gradient-boosting algorithm. </br>
We maximize reproducibility using Unit Testing. We also ensure the entire pipeline of the model is as expected using Integration Testing. We also determine if the model's output is expected by comparing the models in the research and production environment using Differential Testing. Finally, we assess if the value we estimated in research environment translates to the production environment using Shallow Mode. We also monitor the model using Graphana and Prometheus. 

### ML System Testing and Monitoring Lifecycle


## Testing Concepts for ML Systems
## Unit Testing ML Systems
## Docker Refresher
## Integration Testing ML Systems
## Differential Testing
## Shadow Mode
## Monitoring Metrics with Prometheus
## Monitoring Logs with Kibana

## References
- On​ “Reproducibility” ​see this conference talk Sole and I gave: </br>
  https://www.datasciencefestival.com/video/dsf-mainstage-day-2019-soledad-and-chris-samiullah-train-in-data/ </br>
- “Hidden technical debt in Machine learning systems” Sculley​​et al.​ (2015) </br>
  https://papers.nips.cc/paper/5656-hidden-technical-debt-in-machine-learning-systems.pdf </br>
- “The ML Test Score: A Rubric for ML Production Readiness and Technical DebtReduction” Breck ​et al. ​(2017) </br>
  https://research.google/pubs/pub46555/ </br>
- Continuous Delivery For Machine Learning (CD4ML) </br>
  https://martinfowler.com/articles/cd4ml.html</br>
- “Rules of Machine Learning” by Martin Zinkevich </br>
  https://developers.google.com/machine-learning/guides/rules-of-ml#top_of_pagePandas&Scikit-Learn6</br>
