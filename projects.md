## Projects

There are many ideas you can references in this repo: [Rust MLOps Template](https://github.com/nogibjj/rust-mlops-template)

## Universal Project Requirements

- You are REQUIRED to produce 100% reproducible projects, with binaries that "just work", period with no installation.
- You are REQUIRED to produce 80% of your projects using Rust, and the maximum Python you can use is 20%, i.e., for mini-projects 20% * 15, or full-projects 5 * 20%, Bash or SQL or neutral technologies and don't count towards 80/20 split.
- Each student needs to have a main portfolio website that links all of your mini-projects in the course and individual projects using mdBook and published as a GitHub pages site. See this [site as an example](https://github.com/nogibjj/rust-tutorial), with code [here](https://github.com/nogibjj/rust-tutorial).
- You are REQUIRED to develop your code in a cloud-based development environment and share configuration, i.e. GitHub Codespaces .devcontainer configuration.
- You are REQUIRED to develop your code using AI Pair Programming technology such as GitHub Copilot, AWS Codewhisperer, Google Bard, or ChatGPT.  In many cases, you should use more than one.  The goal is for you to use this tool to tackle more complex problems and to lean heavily on the Rust compiler.
- List 3-5 of the most frequent prompts you used with AI Pair Programming tool and list the tool:  i.e. "1. ChatGPT: 'Find the bugs in this code'.
- Working GitHub Actions:  Install, Lint, Format, Compile, Test, Deploy (binary, container, microservice, etc).
- Makefile containing:  install, lint, format, compile, test, deploy that works with no errors, i.e. lint should pass, and no formatting errors.
- Complete GitHub Readme:
    - Explain the goal of the project
    - Architectural Diagram
    - Highlight key snippets of code
    - Nicely formatted Markdown with grammatically correct English
    - Link to demo video explaining code and the project working
    - List the 3-5 top Prompt Engineering prompts you used (not showing name as well, i.e. ChatGPT, etc.)
- Load test, profile, or both:  Microservices need both load tests showing it can between 1-10k requests/second using a tool like [locust](https://locust.io/). For performance hot spots, a command-line tool or script needs to [be profiled](https://github.com/flamegraph-rs/flamegraph).
- If you use a Docker container, put it in your project and use [Distroless](https://github.com/GoogleContainerTools/distroless)
- Container config and/or codespace container config
- Badge for your code like Github Actions Badge
- Github project with source code and README.md explaining project
- Weekly 30-second demo and link to source code in progress via GitHub branch

#### Notes on Architectural Diagram

- Omnigraffle is pretty good.

![example](https://user-images.githubusercontent.com/58792/188945987-a1643d63-69de-4aff-bc6f-e4f3f84b0845.png)

### Media

- 3-5 minute video (3 is better):  1080p, decent audio, private or public youtube link (unlisted is ok)
- Recommend Camtasia or Davinci Resolve for editing

### Process

- Run Cargo formatting tools
- Run linting tools:  Rust Clippy
- Run human + ai code review
- Testing and Linting on each push to the repo.

### Weekly Rust Mini-Projects (Individual)

Scenario: Your company recognizes your expertise in Rust, which you developed through your studies at Duke. They have requested that you build a series of small mini-projects, each taking between one to four hours to complete (i.e., up to half a workday). You will compile all of these Rust projects into a [Rust mdbook repo like this](https://nogibjj.github.io/rust-tutorial/chapter_1.html), where colleagues in your company can browse and learn from the projects.

Requirements:

- No demo video needed for individual projects, just code.
- Create a new repo for each project.
- Build one project each week to complete a total of 15 projects.
- Spend between one to four hours on each project.
- Each Rust mini-project must be 100% reproducible: i.e., a binary or Docker container with code, and it needs to be runnable (either as a command-line tool or microservice).
- You can learn from and improve upon other students' mini-projects, but your project must demonstrate an improvement.
- Fulfill **Universal Project Requirements**.

Topics:

The topics for the mini-projects can fall within the following domains. Each topic is intentionally broad to allow for creativity and innovation in your projects:

1. ONNX Model Deployment with Rust
2. Machine Learning with Rust and PyTorch
3. AWS Lambda Functions with Rust (Cargo Lambda)
4. Azure Serverless Applications with Rust
5. Deploying Rust Applications on GCP Cloud Run
6. Building Microservices with Rust
7. Command-Line Interface (CLI) Tools with Rust
8. Data Analysis with Rust and Polars
9. Web Assembly Applications with Rust
10. Data Streaming and Processing with Rust
11. Rust and Databases: Interfacing with SQL and NoSQL Systems
12. Rust and Web Scraping: Data Collection and Extraction
13. Rust and Cryptography: Secure Data Handling
14. Rust and Networking: Building Network Applications
15. Rust and Concurrency: Parallel and Asynchronous Programming

Feel free to explore and experiment within these domains, and create projects that showcase your skills and interests in Rust programming.


### Projects (Individual)

There are four individual projects.  You are required to demo the progress of you building the project each week by doing a demo video.  Since the class is 16 weeks, divide the progress into each demo, i.e. end of Week 1: 25% of Project 1, Week 2: 50% of Project 1, Week 5: 25% of Project 2, etc.

The deliverables for each project are:

* See above **Universal Project Requirements**

### Projects (Individual)

There are four individual projects.  You are required to demo the progress of you building the project each week by doing a demo video.  Since the class is 16 weeks, divide the progress into each demo, i.e. end of Week 1: 25% of Project 1, Week 2: 50% of Project 1, Week 5: 25% of Project 2, etc.

The deliverables for each project are:

- See above **Universal Project Requirements**

#### Project #1: Command-line Rust Binary using Polars DataFrame package

Scenario: You've been hired as a data engineer at a globally recognized tech company that is not only committed to delivering top-quality services but also to reducing their carbon footprint. They are well known for their commitment to environmental sustainability and have made public pledges about their carbon neutrality.

Your task is to build a foolproof Command Line Interface (CLI) tool that any scientist, researcher, or analyst can use effortlessly. The tool will be deployed on millions of machines worldwide, and it must have the ability to execute without any installation— a feature that promises to save significant time and energy at scale. 

The company has chosen Rust for this project due to its performance advantages over languages like Python. Rust's memory efficiency, speed, and most importantly, its safety guarantees make it an ideal choice for a tool that needs to be robust, secure, and resource-friendly. Rust’s focus on zero-cost abstractions, minimal runtime, and improved memory safety, while maintaining performance, allows the company to maintain their carbon neutral pledge even with large-scale deployments. 

Requirements:

- Meet **Universal Project Requirements**
- Rust binary that builds via GitHub, [see artifacts](https://docs.github.com/en/actions/publishing-packages/about-packaging-with-github-actions).
- Dataset is embedded in the binary so the executable works without any additional installation.
- Uses [Rust Polars Crate](https://www.pola.rs/)
- Loads an interesting dataset of at least 100mb in size.
- CLI tool that uses [Rust Clap Crate](https://docs.rs/clap/latest/clap/#)
- CLI performs basic descriptive statistics using Polars, for example: `mycli -- --describe` or `mycli -- --row foo --stat median`.
- CLI can export a subset of the dataset as a CSV file.
- The codebase should use Rust's error handling idioms to ensure that the program can recover gracefully from unexpected situations.
- The code should be organized into modules with clear interfaces, adhering to Rust's package, crate, and module system to maintain modularity and readability.
- The project should include comprehensive unit and integration tests, making use of Rust's built-in test framework.

##### Optional Requirements

- Consider embedding a pre-trained machine learning model within the Rust binary. This could provide additional utility to your tool, such as predictive analytics or data classification capabilities. If you choose to implement this, ensure you use a model that is suitable for your chosen dataset and respects the constraints of the binary size and the company's sustainability ethos. You could use crates like [ONNX Runtime for Rust](https://crates.io/crates/onnxruntime) for loading the pre-trained models.
- Create a user-friendly and detailed `--help` message for your binary. This could include examples of usage for each command and subcommand, troubleshooting tips, and explanations of any error messages the user might encounter.
- Demonstrate a complex feature of Rust in your codebase. This could be anything from sophisticated pattern matching, to smart pointer usage, to advanced trait-based generics. Use this as an opportunity to show off your Rust programming skills.

##### Some Example Datasets

- Databricks built-in datasets
- Hugging Face Datasets
- Kaggle Datasets
- Azure Open Datasets
- Google's [Public Datasets](https://cloud.google.com/public-datasets)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
- Your own datasets
- Any other interesting and challenging datasets that can showcase the power of your tool

#### Project #2: Bash Command-Line Tool for Data Preparation

Scenario: You're a data engineer in a fast-paced tech company that handles copious amounts of data on a daily basis. The raw data that comes in is often unstructured and requires substantial cleaning and preparation before it can be utilized for analysis or machine learning tasks. You identify the need for a convenient, robust, and easy-to-use Bash command-line tool that can automate these repetitive data preparation tasks such as truncating, sorting, and cleaning data, as well as executing ETL (Extract, Transform, Load) operations. 

The company believes in the efficiency of containerization and uses Docker Hub for the management of their Docker images. The project's tool, being a key part of the data processing pipeline, must be easily accessible and runnable across different machines, thus it should be pushed to Docker Hub. The company also values lightweight solutions for faster delivery and efficient resource use, hence the requirement of using a Distroless container, which omits any extraneous files and software not needed to run the application. This practice aligns with the company's security best practices as it reduces the surface of attack.

Requirements:

- Meet **Universal Project Requirements**
- The project must be pushed to Docker Hub as a Distroless container. The push operation should be executed programmatically via GitHub Actions.
- Your Bash CLI must support at least two subcommands, for example: `./cli.sh truncate --row nba --count 10`.
- You must include Container Linting, such as `hadolint`, and perform security scanning to ensure the safety and integrity of your tool.
- The codebase should include comprehensive documentation. This includes comments for complex code blocks and complete function/method descriptions.
- The project must include a thorough suite of unit tests to ensure the functionality of the tool remains intact as more features are added or existing ones are modified.
- The Bash CLI should handle errors gracefully, providing informative error messages to the user and logging errors for further debugging.

##### Optional Requirements

- Enhance the versatility of your Bash CLI tool by adding additional subcommands beyond the initial two. This could include commands for additional data preparation tasks such as filtering, aggregating, or reshaping data.
- Embedding some form of lightweight data visualization capability in your tool can be highly beneficial. For instance, your tool could generate basic bar plots or histograms that give a quick overview of the data distribution.
- Add a feature that allows users to customize the tool’s behavior through a configuration file. This way, users can adapt the tool's functionality to their specific needs without modifying the script directly.
- Implement a logging system that tracks the tool's activity. This could be helpful for users to understand what the tool is doing at any point, especially when processing large datasets.
- Explore the idea of integrating your Bash tool with cloud services, like AWS S3 or Google Cloud Storage, for direct data input/output from/to cloud storage.

#### Project #3: SQL System Rust Binary CLI

Scenario: You've made a name for yourself as a proficient Rust programmer after your studies at Duke University, and your talents haven't gone unnoticed in your new role. The company you work for manages a vast amount of data in Big Data Systems such as Snowflake, Google BigQuery, Azure Databricks, and AWS Athena. A crucial task that often arises involves running SQL queries on these systems for data analysis and business intelligence purposes. Your boss has entrusted you with the task of developing a Rust Binary Command-Line Interface (CLI) tool that can execute SQL queries on these systems. This tool should be user-friendly, efficient, and robust, enabling team members with varying levels of SQL knowledge to use it confidently.

Requirements:

- Meet **Universal Project Requirements**
- The Rust binary should build via GitHub. See [artifacts](https://docs.github.com/en/actions/publishing-packages/about-packaging-with-github-actions).
- The tool should support connectivity with at least one of the Big Data Systems: Snowflake, Google BigQuery, Azure Databricks, or AWS Athena.
- The CLI should support multiple SQL operations (e.g., SELECT, INSERT, UPDATE, DELETE).
- The CLI tool should use [Rust Clap Crate](https://docs.rs/clap/latest/clap/#) or similar for command line parsing.
- The tool should handle errors gracefully and provide informative error messages.
- Include a comprehensive suite of unit tests to maintain code reliability.
- The tool should include detailed logging to aid in debugging.

##### Optional Requirements

- Enhance the CLI tool's versatility by adding support for multiple Big Data Systems.
- Implement a feature that allows users to save frequently used SQL queries and run them using an alias.
- Embed functionality for basic data visualizations based on the result of SQL queries.
- Add a feature that provides suggestions or auto-completion for SQL commands, increasing user-friendliness for users with less SQL experience.
- Explore integrating the tool with cloud services for direct input/output from/to cloud storage.

#### Project #4: Continuous Delivery of Rust Actix Web Data Engineering Microservice

Scenario: As an expert in Rust programming, you've been assigned to lead an important initiative in your data engineering team. Your company relies on a series of microservices for their data processing pipelines, and they're planning to launch a new service. This new service will handle critical data engineering tasks, and your boss wants it built using Rust and the Actix web framework for its performance, safety, and concurrency advantages.

To ensure that the service can be updated quickly and reliably, your boss wants a Continuous Delivery (CD) pipeline set up for the service. As the lead, you're responsible for developing the microservice and the CD pipeline, ensuring that any changes to the service can be deployed efficiently and effectively.

Requirements:

- Meet **Universal Project Requirements**
- The microservice should be built using Rust and the Actix web framework.
- The microservice should provide at least one RESTful API endpoint that performs a useful data engineering task.
- Set up a Continuous Delivery pipeline for the microservice. This pipeline should automatically build and deploy the microservice whenever changes are made to the codebase.
- The pipeline should include automated testing to ensure that the service is functioning as expected before it is deployed.
- Make use of Docker to containerize the microservice, ensuring it can be run in any environment.
- Make use of Kubernetes, ECS or serverless for orchestrating the deployment of the microservice.
- Include detailed logging and error handling mechanisms in the microservice to aid in debugging and maintenance.

##### Ideas

* [Rust MLOps Template](https://github.com/nogibjj/rust-mlops-template)
* [Rusty Deploy](https://github.com/nogibjj/rusty-deploy/tree/main/rtorchdist)

##### Optional Requirements

- Enhance the microservice by adding more API endpoints.
- Implement rate limiting on the API endpoints to prevent abuse.
- Incorporate a caching mechanism to improve response times for frequently requested data.
- Implement an authentication mechanism for the API endpoints to enhance security.
- Explore integrating the service with a cloud provider's managed Kubernetes service for deployment.

### Projects (Group)

Scenario: Your company is at the forefront of delivering AI-powered solutions to a diverse clientele. As part of the company's ongoing efforts to enhance its AI offerings, your team has been assigned the challenge of developing a web microservice that hosts and serves a machine learning (ML) model. The goal is to create a scalable and efficient service that can be used to make predictions or perform other ML-related tasks. The ML model can be embedded directly into the Rust binary, within a Docker container, or deployed using AWS Lambda with ONNX (Open Neural Network Exchange) format. This project provides an opportunity to gain practical experience in deploying ML models and building scalable AI services in a production-like environment.

Requirements:

- Meet **Universal Project Requirements**
- Develop a Rust microservice that hosts an ML model. The ML model can be embedded directly into the Rust binary, within a Docker container, or deployed using AWS Lambda with ONNX format.
- The microservice should be capable of receiving and processing requests, leveraging the hosted ML model to provide predictions or other outputs.
- The project should include a comprehensive suite of unit tests to ensure the functionality of the microservice.
- The microservice should handle errors gracefully, providing informative error messages to the user and logging errors for further debugging.
- The codebase should include comprehensive documentation. This includes comments for complex code blocks and complete function/method descriptions.
- The microservice must be deployable via Docker, and the Docker image should be pushed to Docker Hub programmatically via GitHub Actions.

Deliverables:

- **GitHub Repository**: A GitHub project that houses the source code for your microservice. The repository should include a `README.md` file that provides a comprehensive overview of your project.
- **Demonstration Video**: A five-minute demonstration video showcasing the functionality of your microservice.
- **Final Presentation**: This project serves as your FINAL EXAM. On the day of the final exam, your team will present the project and explain its functionality in detail.

Optional Requirements:

- The ML model could be trained using the dataset of your choice, but this dataset should be relevant to a business or research context. Using a pre-trained model is also acceptable.
- Implement additional features like logging, health checks, or metrics collection to make the microservice more robust and production-ready.

References:

* [rtorchdist](https://github.com/nogibjj/rusty-deploy/tree/main/rtorchdist)
* [onnx-efs-lambda](https://github.com/nogibjj/rust-mlops-template/tree/main/onnx-efs-lambda)
