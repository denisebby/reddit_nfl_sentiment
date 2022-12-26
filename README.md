# reddit_nfl_sentiment
How does reddit sentiment look like currently for the different nfl team subreddits? Is there a noticeable pattern with team performance and sentiment? How has sentiment changed recently? These are the questions I want to answer with this project. 

Tools used:
I use
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