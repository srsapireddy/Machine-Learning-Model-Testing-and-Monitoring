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
We maximize reproducibility using Unit Testing. We also ensure the entire pipeline of the model is as expected using Integration Testing. We also determine if the model's output is expected by comparing the models in the research and production environment using Differential Testing. Finally, we assess if the value we estimated in the research environment translates to the production environment using Shallow Mode. We also monitor the model using Graphana and Prometheus. 

### ML System Testing and Monitoring Lifecycle
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/811e4d75-b18a-4a50-b774-b44b7853803e)
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/f4953373-44e1-418e-94ab-62b755b25095)
For the purposes of testing and monitoring, we are particularly interested in these components in red.

### ML System Testing and Monitoring
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/4756899d-2af8-4ad9-9dc4-200fa9bda4ac)
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/d7a6148a-1d50-427e-b0f8-5f9c326a5165)

How do these steps interact with each other? (CD4ML) </br>
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/7cb7bf5a-98da-44c9-8deb-a18b9392b648)

## Testing Concepts for ML Systems
### Building ML System Key Phases
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/04e2d3bf-79d8-40c2-a89b-6fc148cc085b)

### Why Test?
Testing is the way we show our system functionality is what we expect to it be, even as we make changes to the system.
1. Confidence
To analyze data provided by monitoring historic system behavior and making predictions from data about past system behavior. </br>
2. Predicting
We also need to care about systems' future reliability. Analyze the uncertainty incurred by any system change. </br>
3. Functionality
What changes are we tracking? It is not just which lines have changed; it's about the entire system functionality, from the user interface through the database.

### Testing Theory
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/55731308-df7e-42ca-9da4-773bdb88b4d0)
1. Unit Test: The smallest and simplest form of software testing. These tests assess a class or function for correctness independent of larger software systems that contain that unit.
2. Integration Tests: Unit Tests are assembled into more significant components called Integration Tests.
3. System Tests: Covers end-to-end functionality of the system. 

The amount of testing depends on the reliability of the system. As the percentage of code-based coverage increases, we should balance the impact of any change in the system.
#### Reference: https://sre.google/sre-book/table-of-contents/

### Testing ML Systems
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/68b1520f-38ad-44ee-9a27-b464a9e0e0ac)
#### Key Testing Principles
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/ea8e8876-bc23-4790-a7e6-d3f9ddde3139) </br>
![image](https://github.com/srsapireddy/Machine-Learning-Model-Testing-and-Monitoring/assets/32967087/58d32d13-6294-45cc-ad98-8b499d04d035)

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
