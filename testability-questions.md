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

## EXAMPLE: How do we trace a call/request end-to-end through the system?

> We need to be able to trace a request across multiple servers/containers/nodes for runtime diagnostic purposes.

### Who?

_The software delivery team and the Web Operations team do this_

### How?

_We use Correlation IDs in HTTP headers, logging the ID at each subsystem, and then searching for the ID in Kibana_

### Evidence 

_We test that Correlation IDs are working properly with BDD tests written in Cucumber. See `tests/correlation-tests` folder e.g. `trace-id.feature`_ 

### Score

_4_

# USABILITY

## USABILITY: Which people or groups do we collaborate with to ensure an effective operator experience? 

> We need a clear understanding of the people and teams that can help to make the software systems work well. 

* Poor: _We fix any operator problems after go-live_
* Excellent: _We collaborate with the live service / operations teams from the start of the project_

### Who?

### How?

### Evidence 

### Score