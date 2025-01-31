# introduction

jenkins is an **automation server** that helps automate the process of building, testing, and deploying software. pipelines can be defined as code using `groovy`, allowing for complex workflows to be managed.

# working

- can pull code from a VCS whenever changes are detected
- automates the process of compiling code, running tests, and packaging the software
- after successful builds and tests, it can deploy the application to different environments
- provides real-time feedback on the status of builds and deployments

# infrastructure

jenkins operates in a distributed architecture that consists of a **master server** and one or more **agents**.

`master server`

:   it orchestrates all the jobs and tasks, manages the configuration, and provides the web UI. it is responsible for:

    - scheduling build jobs
    - managing agents
    - archiving artifacts
    - plugins and configurations

`agents`

:   they are worker nodes that are responsible for executing build jobs. there are two types of agents - *permanent* (servers) and *digital* (ephemeral). key roles of agents are:

    - job execution
    - isolation of jobs
    - distributed builds

# build types

refers to the different ways jobs can be configured to perform automated tasks.

`freestyle`

:   most basic and flexible type of build, allows to configure and automate simple jobs, which can include tasks like building code, running tests, or deploying applications.

`pipeline`

:   more advanced and modern type of build project, provides a way to define build, test, and deploy processes as code. jenkins pipelines use a domain-specific language written in groovy to define these workflows in a **Jenkinsfile**.


