## Projects

### Generalized Best Practices


* README.md is very well polished. (Grammarly, Architectural, Diagram, Key Objectives of Project, Markdown)

#### Notes on Architectural Diagram

* Omnigraffle is pretty good.

![example](https://user-images.githubusercontent.com/58792/188945987-a1643d63-69de-4aff-bc6f-e4f3f84b0845.png)

### Media

* 3-5 minute video (3 is better):  1080p, decent audio, private youtube link (unlisted is ok)

### Content

* Makefile
* requirements.txt
* Container config and/or codespace container config
* Badge for your code like Github Actions Badge
* Some functional/integration test and/or some loadtest: [locust](https://locust.io/) and [loader.io](https://loader.io/)

### Process

* Run formatting tools
* Run linting tools:  pylint and pyflake
* Run human + ai code review
* Testing and Linting on each push to the repo.



### Projects (Individual)

There are four individual projects
The deliverables for each project are:

* Github project with source code and README.md explaining project
* Weekly 30-second demo and link to source code in progress via GitHub branch
* Five-minute final demo video showing how it works.  This demo video should be submitted into group discussion for the week it is due.  This will allow other students to learn from each other and exchange ideas.
* (Optional, but recommended:)
    * Publish source code to the Duke Data Engineering Capstone Github Organization
    * Publish your demo to Duke Data Engineering Capstone YouTube channel and your own channel
    * Create a post with a link to source code and video and share via Linkedin.  Add the following hashtags:  #Duke #dataengineering #mids
    * The video should be at least 1080p with 16:9 aspect ratio.
    * Consider recording with a  low-cost mic like follows:  [Samson Go Mic Portable USB Condenser Microphone](https://www.amazon.com/Samson-Mic-Portable-Condenser-Microphone/dp/B001R76D42/)


#### Project #1: Write a Big Data Script that uses the Pandas API for Spark or Dask

[Example of Databricks end to end tutorial](https://learning.oreilly.com/videos/doing-mlops-with/062592022VIDEOPAIML/)

##### Targets

* Jupyter/Colab Notebook
* CLI
* FastAPI/Flask
* AWS Lambda
* Streamlit/Gradio

##### Datasets

* Databricks built in datasets
* Hugging Face Datasets
* Kaggle Datasets
* Azure Open Datasets
* Your own datasets
* Anything


##### One Example:
Grab a Kaggle project and convert it to run on Dask or Spark using a Pandas API. It should be portfolio worthy.

#### Project #2:  Bash Command-Line Tool

Build a Bash command-line tool that performs a useful data preparation task such as truncating data, sorting it, cleaning data, or doing ETL.  It should be portfolio worthy.

#### Project #3:  SQL [General]

Generate a script that queries a database:  MySQL, Sqlite, Spark or a cloud system.  The query should be something useful to the user and be portfolio worthy.

Reference Reading:

* [BigQuery GIS](https://cloud.google.com/bigquery/docs/gis-getting-started)
* [SQL Mastery Resources](https://noahgift.github.io/data-engineering-and-dataops/sqlmastery)


#### Project #4:  Continuous Delivery of Flask/FastAPI Data Engineering API on AWS 

* Create a Microservice that returns a JSON payload and performs a Data Engineering related task
* Push tested source code to Github and perform Continuous Integration with Github Actions (or similar SaaS Build service)
* Configure Build Server to Deploy Changes on build (Continuous Delivery)
* Create realistic API (reference here:  [Data Engineering: Chapter 5 aws chapter for pragmatic ai.](https://github.com/noahgift/pai-aws))

Reference Video(s)/Courses:

* [Data Engineering with Python and AWS Lambda LiveLessons](https://learning.oreilly.com/videos/data-engineering-with/9780135964330)
* [Building AI & ML Applications on Google Cloud Platform](https://learning.oreilly.com/videos/building-ai-applications/9780135973462)

Reference Source Code: 

* [Containerized FastAPI](https://github.com/noahgift/functions-from-zero2)
* [GCP Hello ML on Github](https://github.com/noahgift/gcp-hello-ml)
* [Flask-Elastic-Beanstalk](https://github.com/noahgift/Flask-Elastic-Beanstalk)
* [Python MLOps Cookbook](https://github.com/noahgift/Python-MLOps-Cookbook)
* [FastAPI](https://learning.oreilly.com/videos/fast-documented-machine/50117VIDEOPAIML/)


### Projects (Group)

Your team will build web microservice that has an API with Swagger Documentation that performs a query using a Pandas, SQL or Dask/Spark Query and returns useful information to the user.

Create the following:

* Github project with source code and README.md explaining the project your group works on.  The README.md should be of professional quality and use a business writing style.
* Five-minute final demo video showing how it works.  This demo video should be submitted into group discussion for the week it is due.  This will allow other students to learn from each other and exchange ideas.
* The demo needs to be very technical and show exactly how to accomplish a task, i.e. you need to teach someone step by step.  _(Think about a cooking show where a chef demonstrates how to make chocolate chip cookies.  This needs to be at the same level of detail)._
* (Optional, but recommended:)
    * Publish source code to the Duke Data Engineering Github Organization
    * Publish your demo to Duke Data Engineering  YouTube channel and your own channel
    * Create a post with a link to source code and video and share via Linkedin.  Add the following hashtags:  #Duke #dataengineering #mids
    * The video should be at least 1080p with 16:9 aspect ratio.
    * Consider recording with a  low-cost mic like follows:  [Samson Go Mic Portable USB Condenser Microphone](https://www.amazon.com/Samson-Mic-Portable-Condenser-Microphone/dp/B001R76D42/)

References:

* [AutoML and KazienML](https://learning.oreilly.com/library/view/practical-mlops/9781098103002/ch05.html#idm45713986170936)
