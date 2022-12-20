# OWASP Code Review Guide (v2.0)

## Table of Contents

### 6.7 Code Review Discovery and Gathering Information

##### Understanding The Design

- Security code review is not simply about the code structure. 

- It is important to remember the data; the reason that
we review code is to ensure that it adequately protects the information and assets it has been entrusted with, such
as money, intellectual property, trade secrets, or lives. 
> The context of the data with which the application is intended
to process is very important in establishing potential risk. If the application is developed using an inbuilt/well-known
design framework the answers to the most of these questions would be pre-defined. But, in case it is custom then this
information will surely aid the review process, mainly in capturing the data flow and internal validations. Knowing
the architecture of the application goes a long way in understanding the security threats that can be applicable to
the application.

###### Design Reviews
- A design is a blueprint of an application; it lays a foundation for its development. It illustrates the layout of the application
and identifies different application components needed for it. It is a structure that determines execution flow
of the application. Most of the application designs are based on a concept of MVC. 

- In such designs different components
interact with each other in an ordered sequence to serve any user request. Design review should be an integral
part of secure software development process. Design reviews also help to implementing the security requirements
in a better way.
> Collecting all the required information of the proposed design including flow charts, sequence diagrams, class diagrams
and requirements documents to understand the objective of the proposed design. The design is thoroughly
studied mainly with respect to the data flow, different application component interactions and data handling. This is
achieved through manual analysis and discussions with the design or technical architect’s team. The design and the
architecture of the application must be understood thoroughly to analyze vulnerable areas that can lead to security
breaches in the application.

## Analyze the threats to the Design
After understanding the design, the next phase is to analyze the threats to the design. This involves observing the
design from an attacker’s perspective and uncovering the backdoors and insecure areas present in it.

### 6.8 Static Code Analysis
