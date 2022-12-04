was able to get transformers pipeline working in vertex ai notebook
- apparently can schedule vertex ai notebooks, but can we turn them off

a more general solution, building vertex ai pipelines
- https://cloud.google.com/vertex-ai/docs/pipelines/notebooks


N1 Predefined Instance Core running in Americas costs like 6 cents in a day


use cluoud scheduler, cloud function, pu sub to access data, used as input to 

uses vertex pipeline to do model inference, code as a pipeline,py file and deploy and schedule
- so will only need 1 component for using the hugging face package


# Notes
wirh function based componenets, hard to know what versions of pacakges to use, 
how do i know when i specify base image like us-docker.pkg.dev/vertex-ai/training/pytorch-xla.1-11:latest