### Projects (Individual)

There are ten individual project types that can be chosen from.  You must do five of them.  If you are new to programming, and/or a beginning MIDS student, it is recommended you mostly stick to the label [General].  If you have strong programming skills it is recommended you choose of mixture of [General] and [Advanced].

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

#### Project #1:  Continuous Delivery of Flask/FastAPI Data Engineering API on GCP/AWS/Azure [General]

* Create a Microservice that returns a JSON payload and performs a Data Engineering related task
* Push tested source code to Github and perform Continuous Integration with Github Actions (or similar SaaS Build service)
* Configure Build Server to Deploy Changes on build (Continuous Delivery)
* Create realistic API (reference here:  [Data Engineering: Chapter 5 aws chapter for pragmatic ai.](https://github.com/noahgift/pai-aws))

Reference Video(s)/Courses:

* [Data Engineering with Python and AWS Lambda LiveLessons](https://learning.oreilly.com/videos/data-engineering-with/9780135964330)
* [Building AI & ML Applications on Google Cloud Platform](https://learning.oreilly.com/videos/building-ai-applications/9780135973462)

Reference Source Code: 

* [GCP Hello ML on Github](https://github.com/noahgift/gcp-hello-ml)
* [Flask-Elastic-Beanstalk](https://github.com/noahgift/Flask-Elastic-Beanstalk)
* [Python MLOps Cookbook](https://github.com/noahgift/Python-MLOps-Cookbook)
* [FastAPI](https://learning.oreilly.com/videos/fast-documented-machine/50117VIDEOPAIML/)

#### Project #2:  Docker & Kubernetes Container Project [Advanced]

* Create a customized Docker container from the current version of Python that deploys a python application
* Push image to DockerHub or Amazon ECR or Google Container Registry
* Pull image down and run it on a cloud platform cloud shell:  Google Cloud Shell or AWS Cloud9.
* Deploy an application to managed Kubernetes cluster

Reference Reading:  

* [Python for DevOps - Chapter 9 Cloud Computing](https://learning.oreilly.com/library/view/python-for-devops/9781492057680/ch09.html#containers-docker)
* [MLOps for Containers and Edge Devices](https://learning.oreilly.com/library/view/practical-mlops/9781098103002/ch03.html#Section-containers)

Reference Source Code: 

* [DevOps SKlearn Microservice on Github](https://github.com/noahgift/container-revolution-devops-microservices)
* [Python MLOps Cookbook](https://github.com/noahgift/Python-MLOps-Cookbook)
* [Docker Flask Locust](https://github.com/noahgift/docker-flask-locust)
* [Container From Scratch](https://github.com/noahgift/container-from-scratch-python)

#### Project #3:  Cloud Map Reduce using Databricks Spark/EMR/Azure Spark [Advanced]

* Perform a Map/Reduce operation using Databrick Spark/EMR/Azure Spark
* Read Chapter 16 in Python for Programmers and implement it on Azure using a free [Azure for Education](https://azure.microsoft.com/en-us/education/) account. 
* Port the example to run on either the GCP or AWS cloud

Reference Reading:  [Python for Programmers, First Edition - Chapter 16 Big Data: Hadoop, Spark, NoSQL and IoT](https://learning.oreilly.com/library/view/python-for-programmers/9780135231364/ch16.xhtml#ch16)

#### Project #4:  Serverless Data Engineering Pipeline [Advanced]

* Reproduce the architecture of the example serverless data engineering project.
* Enhance the project by extending the functionality of the NLP analysis:  adding entity extraction, key phrase extraction, or some other NLP feature.

Reference Reading:  [AWS Lambda on Github](https://github.com/noahgift/awslambda)
Reference Media:  [Data Engineering with Python and AWS Lambda LiveLessons](https://learning.oreilly.com/videos/data-engineering-with/9780135964330)

Reference Architecture Diagram: [Serverless AI Data Engineering Pipeline](https://user-images.githubusercontent.com/58792/55354483-bae7af80-547a-11e9-9909-a5621251065b.png) (accessible transcript of diagram)

#### Project #5:  Cloud SQL [General]

Use a cloud SQL solution such GCP Big Query, or AWS Athena to Query a Public Dataset and find a useful insight.

Reference Reading:

* [BigQuery GIS](https://cloud.google.com/bigquery/docs/gis-getting-started)


#### Project #6:  Small Data Engineering NLP and AI APIs with “No Code/Low Code” [General]

* Scrape all of Hemingway’s writing from this website (or some other author):  http://gutenberg.ca/index.html (Can be manual or with Python)
* Create Data Visualization summarizing what you learned.
* Create one-page in report, in Github using Markdown summarizing the point of the data visualization (give firm recommendation/conclusion)
* Example Walkthrough Video:  https://learning.oreilly.com/videos/no-code-and/62202021VIDEOPAIML/
* Example Repo:  [https://github.com/noahgift/exploratory-data-analysis](https://github.com/noahgift/exploratory-data-analysis)

#### Project #7:  Create Data Engineering Command-line Tool [General]

Create a CLI tool in Python that does a data engineering task

Reference Reading: 

* [CLI Tools]https://learning.oreilly.com/library/view/practical-mlops/9781098103002/ch11.html#idm45713973322232
* [Python CLI Tools](https://paiml.com/docs/home/books/python-command-line-tools/)
* [Optimizing EC2 Instances](https://learning.oreilly.com/library/view/pragmatic-ai-an/9780134863924/ch09.xhtml#ch09lev1sub1)
* [Command Line Tools Python-Python for DevOps](https://learning.oreilly.com/library/view/python-for-devops/9781492057680/ch03.html#idm46114720418584)

Reference Source Code: 
* [Python MLOps Cookbook](https://github.com/noahgift/Python-MLOps-Cookbook
* [Data Engineering API](https://github.com/noahgift/pai-aws)

#### Project #8:  Create End to End Data Visualization Pipeline [General]

Using your scripting skills create an end-to-end automated data pipelines that visualizes a useful dataset.  


* [Exploring Real-Estate Values](https://learning.oreilly.com/library/view/pragmatic-ai-an/9780134863924/ch10.xhtml#ch10lev1)
* [Data Science Pandas](https://paiml.com/docs/home/books/minimal-python/chapter07-data-science-pandas/)
* [Collecting NBA Data](https://learning.oreilly.com/library/view/pragmatic-ai-an/9780134863924/part03.xhtml)

Reference Source Code: 

* [Real Estate ML]https://github.com/noahgift/real_estate_ml
* [Covid Explore](https://github.com/paiml/minimal-python/blob/master/Chapter7_data_science.ipynb)

#### Project #9:  Publish Python Command-line Tool or Library to Python Package Repository [Advanced]

Create a useful CLI tool that solves a data engineering related problem

Reference Reading: 

* [Packaging in Python](https://learning.oreilly.com/library/view/python-for-devops/9781492057680/ch05.html#idm46114712983992)
* [Finding Project Management Insights with Github](https://learning.oreilly.com/library/view/pragmatic-ai-an/9780134863924/ch08.xhtml#ch08lev1)


#### Project #10:  Recreate one of other Individual projects in a non-Python language [Advanced]

Use Go, Scala or a .NET Language (C# or F#) or Node.js to solve a data engineering problem.  My recommendation would be to focus on a functional programming style.

Reference Reading: 

* [F Sharp Map Reduce](https://docs.microsoft.com/en-us/archive/msdn-magazine/2011/april/msdn-magazine-mapreduce-in-fsharp-parsing-log-files-with-fsharp-mapreduce-and-microsoft-azure)

### Projects (Group)

Your team will make a “bet” on a technique or technology in the free resources you have been exposed to.  Maybe you want to demo step by step how to train a Tensorflow model on a TPU on GCP, or how to train an RNN model using AWS Sagemaker, or train a computer vision model using Apple CreateML and deploy it to an iOS device using only data you created from your iPhone.  Pick something you think will “move the needle” in the next two years and help you and your team get a high-paying job.  Alumni of the program are counting on you to give them a demo of what skills they need to invest in.  Soon, you will be alumni and will be hoping other students will show you a demo of something that you can learn from in the coming years when you graduate.

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
