# reddit_nfl_sentiment
How does reddit sentiment look like currently for the different nfl team subreddits? Is there a noticeable pattern with team performance and sentiment? How has sentiment changed recently? These are the questions I want to answer with this project. 

https://nfl-pulse-5w5kpqv4ea-ue.a.run.app/

Kaggle dataset I made for team logo images since I could not find a good pre-existing dataset: https://www.kaggle.com/datasets/debby99/nfl-team-logos-as-of-2023

I used: 
- Cloud Scheduler & Cloud Functions
    - schedule job to get recent reddit comments
    - run sentiment classification pipeline
- Vertex AI Pipelines
    - run Kubeflow pipeline to conduct sentiment analysis and aggregate scores
- GCS
    - stores data and pipeline metadata
- DASH
    - frontend
- Cloud Run
    - deployment