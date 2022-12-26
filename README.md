# reddit_nfl_sentiment
How does reddit sentiment look like currently for the different nfl team subreddits? Is there a noticeable pattern with team performance and sentiment? How has sentiment changed recently? These are the questions I want to answer with this project. 

https://nfl-pulse-5w5kpqv4ea-ue.a.run.app/

Additionally, here is the Kaggle dataset I made for team logo images since I could not find a good pre-existing dataset: https://www.kaggle.com/datasets/debby99/nfl-team-logos-as-of-2023

I used: 
- Cloud Scheduler & Cloud Functions
    - schedule job to get recent reddit comments
    - run sentiment classification pipeline
- Vertex AI Pipelines
    - run Kubeflow pipeline to conduct sentiment analysis and aggregate scores
- Hugging Face 
    - use default sentiment classification model (DistilBERT base uncased finetuned SST-2)
- GCS
    - store data and pipeline metadata
- DASH
    - frontend
- Cloud Run
    - deployment

TODO:
- improve responsiveness of frontend
- improve model used (classification of reddit comments not always correct)