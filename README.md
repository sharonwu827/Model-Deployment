# Model Deployment

## Key Principles For Designing ML System

- Build for reproducibility from the start: Persist all model inputs and outputs, as well as all relevant metadata such as config, dependencies, geography, timezones and anything else you think you might need if you ever had to explain a prediction from the past. Pay attention to versioning, including of your training data.
- Treat your ML steps as part of your build: Which is to say, automate training and model publishing
- Plan for extensibility: If you are likely to be updating your models on a regular basis, you need to think carefully about how you will do this from the beginning.
- Modularity: To the largest extent possible, aim to reuse preprocessing and feature engineering code from the research environment in the production environment.
- Testing: Plan to spend significantly more time on testing your machine learning applications, because they require additional types of testing