#You can get the training dataset from kaggle.com

                                         CHAPTER-1 INTRODUCTION

INTRODUCTION TO PROJECT
 
The H-1B is an employment-based, non-immigrant visa category for temporary foreign workers in the United States. For a foreign national to apply for H1-B visa, a US employer must offer a job and petition for H-1B visa with the US immigration department. This is the most common visa status applied for and held by international students once they complete college / higher education (Masters, PhD) and work in a fulltime position. H-1B visa class is very industry relevant and many individuals and companies rely heavily on this yearly allotment. Currently there’s no way for knowing how application attributes contribute towards the final visa-status outcome. In this report, we proceed in the following manner to achieve our objective. In section II, we introduce the dataset that we experimented on and our analysis on it. Then we talk about the details of our predictive task. It describes the various features we extracted from the data based on our analysis. Then, we present the related work that has been done on H1- B visa classification.It discusses the models in details, their advantages and the issues we faced. In the last section, we present our results and conclusion.

1.1 DATASET
 We found the dataset from Kaggle https://www. kaggle.com/nsharan/h-1b-visa and it contains 1048543 samples for year 2015 and 2016. 
 

   Fields 
CASE STATUS:Status associated with the last significant event or decision. Valid values include Certified, Certified-Withdrawn, Denied, and Withdrawn. 
EMPLOYER NAME:Name of employer submitting labor condition application. 
SOC NAME:Occupational name associated with the SOC CODE. SOC CODE is the occupational code associated with the job being requested for temporary labor condition, as classified by the Standard Occupational Classification (SOC) System. 
JOB TITLE: Title of the job. FULL TIME POSITION: Y = Full Time Position; N = Part Time Position.
 PREVAILING WAGE: Prevailing Wage for the job being requested for temporary labor condition. The wage is listed at annual scale in USD. The prevailing wage for a job position is defined as the average wage paid to similarly employed workers in the requested occupation in the area of intended employment. The prevailing wage is based on the employers minimum requirements for the position. 
YEAR: Year in which the H-1B visa petition was filed. 
WORKSITE: City and State information of the foreign worker’s intended area of employment.
lon:longitude of the Worksite. 
lat:latitude of the Worksite.

PROJECT CATEGORY
This project falls in the category of Application based projects.
The field of the project is Data Analysis.
H-1B visa class is amongst the most sought after visa categories .

OBJECTIVES
The main objective of the project is predicting the future prices of the stocks using previous dataset available. To achieve this objective there are some basic requirements to be fulfilled. These requirements are:

To train machine learning algorithm program using this dataset.
To predict the status of the application.
To create a graphical user interface (GUI) for the program to make it easy for user to operate.



PROBLEM FORMULATION

Collect  sufficient amount of  data from various sources.
Using this data, to train the machine learning program.
Once trained, the program can be used to predict if the visa would be approved or not.
Plot the data on the graph and show the output to user through graphical interface.

IDENTIFICATION OF NEED
To implement the problem’s solution there are few requirements needed to be fulfilled. These requirements are:
Source of the dataset required to train the program.
Algorithm that will used to train the dataset.
Programming language to implement the algorithm and all other required modules.
User Interface through which user can interact.

EXISTING SYSTEM
The existing system in case of H-1B visa predictions uses various kinds of machine learning methods. These methods use various mathematical functions to analyze data and predict future data. Most of methods are quite complex for beginners and some are easy to implement. The result of these methods depends on the validity of the predictions. They normally use large dataset of previous applications to enhance the quality of predictions. This in turn causes difficulty in implementing these methods as they require more time to process and better systems to operate. This increases the total cost of the project.

PROPOSED SYSTEM  
The proposed system is based on a machine learning algorithm called as Random Forest Classifier. Random Forest Classifier is a based on Decision tree and other algorithms of machine learning for modeling the relationship between a scalar dependent variable Y and one or more explanatory variables (or independent variables) denoted by X. The dependent variable can be salary, location, job title and independent variable is ID, lon, lat.  It forms a linear relation between both the variables using the dataset and then uses independent variable to predict next value of dependent. This is a simple approach and easy to implement. It can work with dataset of any size. It uses modeled data for the training purpose and then predict the visa application status of a person.

CHAPTER-2 REQUIREMENT ANALYSIS AND SYSTEM SPECIFICATION

2.1 FEASIBILTY STUDY
The main goal of feasibility study is to determine whether it would be financially and technically feasible to develop the software. The feasibility study involves carrying out several activities such as collection of basic information relating to the software such as the different data item that would be input to the system, the processing required to be carried out on these data, the output data required to be produced by the system as well as various constraints on the development. 

2.1 PROJECT GOALS AND SCOPE
A chief goal of this project is to  predict the application status for H-1B visa. The hope is that we would be able to find the staus of the application. The project will evaluate some existing strategies from a rigorous scientific perspective and provide a quantitative evaluation of new strategies. It will focus exclusively on predicting the application status of candidate. More so, the project will analyze the accuracies of these predictions.

TECHNICAL FEASIBILITY: This project will be able to analyze the available H-1B visa applicants dataset and predict the status of their application. This project requires various resources
for its implementation. These resources include datasets, programming language, modules and packages, etc.
There are basically three data resources. 
∙ Files, such as EXCEL, CSV, and TEXT. 
∙ Database, such as SQLite, MySQL. 
∙ Python.

ECONOMICAL FEASIBILITY: All the software’s and packages used in this project are free of cost. The hardware used is basic and easily available in systems now days. Only cost of the project can be the developing and maintenance cost. Any module or package other than one used in this project may cost something. 

OPERATIONAL FEASIBILITY: The proposed system is able to analyse the dataset, visualize graphical representation of the data and predict the next value of the dependent. It can analyze the data and provide graphical representation of status of application. It is easy to use and simple to understand.
2.2 Software Requirement Specification
 1.INTRODUCTION:
A software requirements specification (SRS) is a document that captures complete description about how the system is expected to perform. It is usually signed off at the end of requirements engineering phase.The output of the requirements phase of the software development process is Software Requirements Specification (SRS) (also known as requirements document). This document lays a foundation for software engineering activities and is created when entire requirements are elicited and analyzed. SRS is a formal document, which acts as a representation of software that enables the users to review whether it (SRS) is according to their use. The aim of this document is to gather and give a complete in-sight of the H1-B VISA data analysis by defining its applications in detail. In addition, it includes user requirements for a system as well as detailed specifications of the system requirements.
Qualities of SRS:
·       Correct
·       Unambiguous
·       Complete
·       Consistent
·       Ranked for importance and/or stability
·       Verifiable
·       Modifiable
·       Traceable

A. PURPOSE:
The purpose of the document is to collect and analyze all assorted ideas that have come up to define the system, its requirements with respect to consumers. Also, we shall predict and sort out how we hope this product will be used in order to gain a better understanding of the project, outline concepts that may be developed later, and document ideas that are being considered, but may be discarded as the product develops. In short, the purpose of this SRS document is to provide a detailed overview of our software product, its parameters and goals. This document describes the project target audience and its user interface,hardware and software requirements. It defines how our user can predict the chance of getting an h1-b visa.
 In short the purpose of the srs is to provide a detailed overview of our software product,its parameters and goals.This project defines the product target and audience ,its user interface,hardware and software requirements.
 
B. OVERVIEW:
This document contains the problem statement that the current system is facing which is hampering the growth opportunities of the company. It further contains a list of the stakeholders and users of the proposed solution. It also illustrates the needs and wants of the stakeholders that were identified in the brainstorming exercise as part of the requirements workshop. It further lists and briefly describes the major features and a brief description of each of the proposed system. The following SRS contains the detail product perspective from different stakeholders. It provides the detail app function withuser characteristics permitted constraints, assumptions and dependencies and requirements subsets.
 
C. ENVIRONMENTAL CHARACTERISTICS:
 i) SOFTWARE REQUIREMENTS:
·       Any windows based operating system.
·       DBMS for database.
·       IDE for developing code
 ii) HARDWARE:
   ·       An internet enabled device such as Laptop.
   ·       i5 processor with 8gb of ram and 500gb of storage is recommended

2. GOALS OF IMPLEMENTATION:
The H-1B is an employment-based, non-immigrant visa category for temporary foreign workers in the United States. For a foreign national to apply for H1-B visa, an US employer must offer a job and petition for H-1B visa with the US immigration department. This is the most common visa status applied for and held by international students once they complete college/ higher education (Masters, PhD) and work in a full-time position. This system would help employers to select candidates who would be eligible for applying the visa.It would help them in saving application fees
 
3 FUNCTIONAL REQUIREMENTS:
A functional requirement document defines the functionality of a system or one of its subsystems. It also depends upon the type of software, expected users and the type of system where the software is used.
Functional user requirements may be high-level statements of what the system should do but functional system requirements should also describe clearly about the system services in detail.
 
USER ACTIVITY
. User Details:This activity contains some fields which requires to take input from user and this data is being transferred to a dbms and then processed and results are being fetched and displayed to the user i.e the final prediction which is based on test data.
 
4. NON-FUNCTIONAL REQUIREMENTS:-
In systems engineering and requirements engineering, a non-functional requirement (NFR) is a requirement that specifies criteria that can be used to judge the operation of a system, rather than specific behaviors. They are contrasted with functional requirements that define specific behavior or functions. The plan for implementing functional requirements is detailed in the system design. The plan for implementing non-functional requirements is detailed in the system architecture, because they are usually Architecturally Significant Requirements.
 Broadly, functional requirements define what a system is supposed to do and non-functional requirements define how a system is supposed to be. Functional requirements are usually in the form of "system shall do <requirement>", an individual action or part of the system, perhaps explicitly in the sense of a mathematical function, a black box description input, output, process and control functional model or IPO Model. In contrast, non-functional requirements are in the form of "system shall be <requirement>", an overall property of the system as a whole or of a particular aspect and not a specific function. The system's overall properties commonly mark the difference between whether the development project has succeeded or failed.Non-functional requirements are often called "quality attributes" of a system. Other terms for non-functional requirements are "qualities", "quality goals", "quality of service requirements", "constraints" and "non-behavioral requirements". Informally these are sometimes called the "ilities", from attributes like stability and portability. Qualities—that is non-functional requirements—can be divided into two main categories:
1. Execution qualities, such as safety, security and usability, which are observable during  operation (at run time).
2. Evolution qualities, such as testability, maintainability, extensibility and scalability, which are embodied in the static structure of the system.

2.3 SDLC MODEL TO BE USED
SDLC is a process followed for a software project, within a software organization. It consists of a detailed plan describing how to develop, maintain, replace and alter or enhance specific software. The life cycle defines a methodology for improving the quality of software and the overall development process.
SDLC - Spiral Model

The spiral model combines the idea of iterative development with the systematic, controlled aspects of the waterfall model. This Spiral model is a combination of iterative development process model and sequential linear development model i.e. the waterfall model with a very high emphasis on risk analysis. It allows incremental releases of the product or incremental refinement through each iteration around the spiral.


                                                               Fig1



CHAPTER-3 SYSTEM DESIGN
3.1 Design Approach
This design approach used on this project is function-oriented. In this, the system is comprised of many smaller subsystems known as functions. These functions are capable of performing significant task in the system, the system is considered as top view of all the systems. This project is designed only to be simple and easy to implement and understand. To accomplish this any complex measures are avoided. All the processing and modelling of data is done using functional approach.
3.2 Detail Design
The core of this project is machine learning, and it is implementing using linear regression algorithm. The dataset required can be obtained from Kaggle or any other provider. This data is fitted into a model that will be used for random forest classification. This model is processed and the data is analyzed to train the algorithm. Then the algorithm can be used to predict the  acceptability of visa.
The outline of the design of system is:
●   Getting the previous dataset of stock prices, available at yahoo finance.  
●   Using machine learning algorithms to train the program using the dataset.
●   To predict the value of stock price using the trained program and analyzing the graph.
●   Creating a graphical user interface (GUI) for the program to make it easy for user to operate.
3.3 System Design 
Flow of data when compiled by the python’s idle.xlwings:Python library that makes it easy to call Python from Excel and vice versa.SQL Alchemy is the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL.

                                                                  Fig 2


3.4 METHODOLOGY
Once we have the previous dataset and machine learning algorithm suitable for the purpose, we need to provide it the dataset and let it train the program. After that it will be able to predict the future prices up to some accuracy.
The various steps to be followed for the development of the project are:
Getting the previous dataset of H-1B visa dataset, available at kaggle. 
Using machine learning algorithms to train the program using the dataset.
To predict the visa application status using the trained program and analyzing the graph.
Creating a graphical user interface (GUI) for the program to make it easy for user to operate.

Fig3 Data Flow

                                         Fig 4
The flow of the project is defined in the figure above.Firstly data is collected from Kaggle and then is passed to the model and after preprocessing of  the previous data and predicted application status  will be displayed.
           CHAPTER-4 IMPLEMENTATION, TESTING, AND MAINTENANCE

4.1 INTRODUCTION TO LANGUAGES, IDE’S, TOOLS AND TECHNOLOGIES USED FOR IMPLEMENTATION

Python is an interpreted high-level programming language for general-purpose programming. It is a simple and easy to use language having clean syntax and powerful structure. Python is most suited for data science and machine learning problems. Due it.1 
s large set of libraries python makes it easy to implement certain tasks. It provides constructs that enable clear programming on both small and large scales. It provides constructs that enable clear programming on both small and large scales.
IDLE (short for integrated development environment or integrated development and learning environment) is an integrated development environment for Python, which has been bundled with the default implementation of the language. It is packaged as an optional part of the Python packaging with many Linux distributions. It is completely written in Python and the Tkinter GUI toolkit (wrapper functions for Tcl/Tk). IDLE is intended to be a simple IDE and suitable for beginners, especially in an educational environment. To that end, it is cross-platform, and avoids feature clutter.
The main technology to be used for the project is machine learning and data analysis. The machine learning algorithm used is linear regression.
Machine Learning: Machine learning is a field of computer science that gives computers the ability to learn without being explicitly programmed. Within the field of data analytics, machine learning is a method used to devise complex models and algorithms that lend themselves to prediction.
Data Analysis: Data analysis, also known as analysis of data or data analytics, is a process of inspecting, cleansing, transforming, and modeling data with the goal of discovering useful information, suggesting conclusions, and supporting decision-making. Data analysis has multiple facets and approaches, encompassing diverse techniques under a variety of names, in different business, science, and social science domains.
Random Forest is a flexible, easy to use machine learning algorithm that produces, even without hyper-parameter tuning, a great result most of the time. It is also one of the most used algorithms, because it’s simplicity and the fact that it can be used for both classification and regression tasks. In this post, you are going to learn, how the random forest algorithm works and several other important things about it.
Machine learning libraries used in this project are Scikit-Learn and numpy. Scikit-learn make it easy to perform machine learning tasks by providing predefined method for data processing and program training like linear_regression_model.
Matplotlib is used to plot a graph with given dataset. It makes visualization of data easier. 

4.2 CODING STANDARDS OF LANGUAGE USED
The programming language used in this project is Python. Python is a higher level interpreted language which supports both functional and object oriented programming. 
The approach used in this project is functional approach.
The coding standards used are default standard for Python PEP 8 created by its developers.
It marks rules some basic functions of the language like indentation, docstrings, logging, imports, blank lines, comments, etc.
4.3 Testing Techniques
The testing of the proposed work is quite easy, the major method for testing is to manually compare its predicted values with the values obtained from the other resources i.e. internet. Secondly, by obtaining the values from different models using the same data set and then comparing the values with each other. Since, it is a learning model so by repeatedly generating the output the output of the model can also be tested.
                                    Chapter-5  Results And Discussion
5.1 System With Brief Details
 
    


                                                     Fig5  
This represents the pie chart representing the application status of the applicants as predicted by the model .The graph below is showing the applications received from different states
                                                                                  
 
                                                               Fig 6

5.2 Backend Representation/Database Table

 
                                                              Fig 7
                                  Chapter-6   Conclusion And Future Scope
H-1B visa analysis is a prediction system to predict the application status of candidate . It is easy to implement and being hardware independent it can be implemented on any hardware system compatible with python packages.
The future of this can be included with more complex prediction models like RNN or Non-linear regression models, a better user interface in the form of app or website, giving a layman an opportunity to select any attribute from the desired dataset which will in mean will increase the flexibility in its application












   
                                                    BIBLIOGRAPHY
www.wikipedia.org
www.tutorialspoint.com
www.python.org
www.kaggle.com
www.github.com
