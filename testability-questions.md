# Testability Questions - TestabilityQuestions.com

See [`README.md`](README.md) for more details on how to use these questions.

These **testability questions** that are useful for assessing the testability of software systems. These questions can be used with a number of test strategy tools like the [Agile Testing Quadrants](https://lisacrispin.com/2011/11/08/using-the-agile-testing-quadrants/) to identify more gaps in testing and enhance testability to enable your teams to fill those gaps.

Each question requires answers to these key questions: 

* **Who? (What?)**: What kind of user or persona will do this? (Or what kind of system?) 
* **How?**: Which tool (or set of tools) or process will help to do this?
* **Evidence**:  How will you demonstrate this using evidence?
* **Score**: a score of 1 to 5 for how well your approach compares to industry-leading approaches (1 is poor; 5 is excellent)

Use the _Poor_ and _Excellent_ criteria to help guide your scores. These are examples of bad and good extremes; your situation may demand slightly different critera.

> Print this page and record questions using pen & paper with your team

Copyright © 2018 [Conflux Digital Ltd](https://confluxdigital.net/)

Licenced under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)

_Permalink: [TestabilityQuestions.com](http://testabilityquestions.com/)_

## EXAMPLE: How well do we separate components within our system?

> We need to be able to isolate components in order to test effectively, debugging issues easier and knowing which components are impacted by change.

### Who?

_The software delivery team and the Web Operations team do this_

### How?

_We have implemented circuit breakers between our services in order to both isolate them when errors in adjacent components occur. In addition they can be opened intentionally when needed for testing_

### Evidence

_We have a grafana dashboard showing circuit breaker behaviour over the past month, with events detailing how often they have opened, been intentionally opened, automatically recovered or required intervention to close._

### Score

_4_

# OBSERVABILITY

## OBSERVABILITY: Does each member of the team have a method of consuming the application logs from Production?

> We recognise the importance that all team members can see below the application with organised logging which shows important system events, so we aren't fooled by what we see on the surface of the applications we test.

* Poor: _Limited team members have access to disparate hosts to inspect log files_
* Excellent: _We have tooling which centralises, aggregates and displays our logging which is available to all team members_

### Who?

### How?

### Evidence 

### Score

## OBSERVABILITY: Does the team know what value the 95th percentile of response times is for their system?

> We recognise the need to performance and capacity test, gather data for analysis, and analyse data without outliers to expose the system limits.

* Poor: _We regularly defer performance and capacity testing_
* Excellent: _We actively track our performance and capacity with regular testing and review on a consistent basis_

### Who?

### How?

### Evidence 

### Score

## OBSERVABILITY: Does the team collaborate regularly with teams that maintain their dependencies?

> We recognise the importance of our internal and external dependencies. The testability of dependencies effects your testability.

* Poor: _We contact our dependencies when there is a problem_
* Excellent: _We collaborate with our dependencies by attending their ceremonies where appropriate and monitoring their uptime_

### Who?

### How?

### Evidence 

### Score

## OBSERVABILITY: Can the team test both the synchronous and asynchronous parts of their system?

> We need the ability to test both scheduled tasks which lifts and shifts or replicates data and other operations which occur on demand.

* Poor: _We wait to test scheduled tasks in later environments_
* Excellent: _We can trigger both synchronous and asynchronous tasks when needed, close to development_

### Who?

### How?

### Evidence 

### Score

# CONTROLLABILITY

## CONTROLLABILITY: Can you set your system into a given state to repeat a test?

> We need the ability to set both data and configuration to recreate the conditions for a specific test, to assist with consistency and reproducability.

* Poor: _Data and configuration is static, requires a separate team to schedule a change_
* Excellent: _Data and configuration is dynamic and can be set by the team_

### Who?

### How?

### Evidence 

### Score

## CONTROLLABILITY: Is each member of the team able to create a disposable test environment?

> We need all members of the team to be able to build a test environment with a specific version of the application and tear it down afterwards to enable early showcasing and testing.

* Poor: _All our environments are persistent with a long build performed outside the team_
* Excellent: _An environment can be created and destroyed by each team member in a self service manner_

### Who?

### How?

### Evidence 

### Score

## CONTROLLABILITY: If you ask the team to change their codebase do they react positively?

> We need confidence when changes that add value are required we can change the code or configuration with knowledge of potential impacts.

* Poor: _We are reluctant to change some or part of the codebase without deep analysis_
* Excellent: _We are confident that we can make isolatable changes which can realise business value while minismising risk_

### Who?

### How?

### Evidence 

### Score

## CONTROLLABILITY: Is each member of the team able to run automated unit tests?

> We need a clear understanding what a unit is in the context of our system and each team member can execute our lowest level test suite on demand.

* Poor: _We have no unit tests_
* Excellent: _Unit tests are part of our definition of done, run as part of continuous integration and executable by any team member_

### Who?

### How?

### Evidence 

### Score

# UNDERSTANDING

## UNDERSTANDING: Does the team curate a living knowledge base about the system it maintains?

> We need a store of information that is kept up to date in order for our stakeholders to integrate with the team which is up to date with our system.

* Poor: _We have a team wiki page which is updated periodically_
* Excellent: _We have a living executable specification describing our system and documentation such as [Swagger](https://swagger.io/) for those who wish to integrate with us_

### Who?

### How?

### Evidence 

### Score

## UNDERSTANDING: Does the team know which parts of the codebase are subject to the most change?

> We need a clear understanding which areas of our codebase are subject to the most change so we can target testing appropriately.

* Poor: _We rely on intuition alone to describe changes_
* Excellent: _We visualise our source code repositories using tooling such as [Gource](https://gource.io/)_

### Who?

### How?

### Evidence 

### Score

## UNDERSTANDING: Does each member of the team have access to the system source control?

> We need all members of the team to access one of the main collaboration artefacts for a development team, for code and configuration.

* Poor: _Only the developers have access to the code_
* Excellent: _Developers, test, operations and product stakeholders can at least view the code_

### Who?

### How?

### Evidence 

### Score

## UNDERSTANDING: Does the team have regular contact with the users of the system?

> We need regular contact with our users, internal or external, with a preference for face to face if possible.

* Poor: _We fix any operator problems after go-live_
* Excellent: _We collaborate with our users often, inviting internal users to our ceremonies and with monitoring of journeys to complement direct feedback by external users_

### Who?

### How?

### Evidence 

### Score