# Terminology

### Software
A program or a set of programs that fulfill desired functionality. It contains organised code written by programmers in any programming language.

### Software Engineering
Application of Engineering concepts in Software development in a systematic method.

### Software Requirement Specification
A document that contains complete information about how a software is expected to perform.

### Software Development Life Cycle
A designed process for planning, developing, testing and deploying a software.

### Requirement Analysis
- First stage in software development life cycle. 
- Determines the needs or conditions to meet for a new or altered product.
- Takes account of the possibly conflicting requirements of the various stakeholders.

**ISO 9000** is a set of international standards on quality management and quality assurance developed to help companies effectively document the quality system elements to be implemented to maintain an efficient quality system. They are not specific to any one industry and can be applied to organizations of any size.

### Dual role of Software
Software can act in two different ways:
- As a product
- As a medium to deliver product

### Program vs Software
| Program                                             | Software                                                                       |
| --------------------------------------------------- | ------------------------------------------------------------------------------ |
| Program is a set of instructions related each other | Software is a collection of program designed for specific task                 |
| Usually small in size                               | Usually large in size                                                          |
| Developed by individuals                            | Developed by large no of users                                                 |
| Lack in proper documentation                        | Proper documentation and user manual prepared                                  |
| Unplanned, usually not Systematic                   | Well Systematic, organized, planned approach                                   |
| Provide Limited functionality and less features     | Provides more functionality as they are big in size more options and features. |

# Software Engineering

Software engineering is an engineering discipline that’s applied to the development of software in a systematic approach (called a software process).It’s the application of theories, methods, and tools to design build software that meets the specifications efficiently, cost-effectively, and ensuring quality. It is not only concerned with the technical process of building a software, it also includes activities to manage the project, develop tools, methods and theories that support the software production.

Not applying software engineering methods results in more expensive, less reliable software, and it can be vital on the long term, as the changes come in, the costs will dramatically increase.

## Objectives

- Maintainability
- Correctness
- Reusability
- Testability
- Reliability
- Portability
- Adaptability

## Importance

- Reduces complexity
- To minimize software cost
- To decrease time
- Handling big projects
- Reliable software
- Effectiveness

# Software Development Life Cycle

Software Development Life Cycle (SDLC) is a process used by the software industry to design, develop and test high quality software. The SDLC aims to produce high-quality software that meets or exceeds customer expectations, reaches completion within times and cost estimates. The life cycle defines a methodology for improving the quality of software and the overall development process. It consists of a detailed plan describing how to develop, maintain, replace and alter or enhance specific software.

## Phases

### 1. Planning and Requirement Analysis

- Performed by the senior members of the team with inputs from the customer, the sales department, market surveys and domain experts in the industry.
- This information is then used to plan the basic project approach and to conduct product feasibility study in the economical, operational and technical areas. 
- Planning for the quality assurance requirements and identification of the risks associated with the project is also done in the planning stage. 
- The outcome of the technical feasibility study is to define the various technical approaches that can be followed to implement the project successfully with minimum risks.

### 2. Defining Requirements

- Clearly define and document the product requirements and get them approved from the customer or the market analysts. 
- This is done through an SRS (Software Requirement Specification) document which consists of all the product requirements to be designed and developed during the project life cycle.

### 3. Designing the Product Architecture

- SRS is the reference for product architects to come out with the best architecture for the product to be developed.
- Based on the requirements specified in SRS, usually more than one design approach for the product architecture is proposed and documented in a **DDS - Design Document Specification.**
- This DDS is reviewed by all the important stakeholders and based on various parameters as risk assessment, product robustness, design modularity, budget and time constraints, the best design approach is selected for the product.
- A design approach clearly defines all the architectural modules of the product along with its communication and data flow representation with the external and third party modules (if any).
- The internal design of all the modules of the proposed architecture should be clearly defined with the minutest of the details in DDS.

### 4. Building or Developing the Product

- The actual development starts and the product is built. The programming code is generated as per DDS during this stage.
- If the design is performed in a detailed and organized manner, code generation can be accomplished without much hassle.
- Developers must follow the coding guidelines defined by their organization and programming tools like compilers, interpreters, debuggers, etc. are used to generate the code.
- Different high level programming languages such as C, C++, Pascal, Java and PHP are used for coding. The programming language is chosen with respect to the type of software being developed.

### 5. Testing the Product

- The testing only stage of the product where product defects are reported, tracked, fixed and retested, until the product reaches the quality standards defined in the SRS.

### 6. Deployment in the Market and Maintenance

- Once the product is tested and ready to be deployed it is released formally in the appropriate market. 
- Sometimes product deployment happens in stages as per the business strategy of that organization.
- The product may first be released in a limited segment and tested in the real business environment (UAT- User acceptance testing).

# SDLC Models
## Classic Waterfall Model

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.pngkey.com%2Fpng%2Ffull%2F836-8364648_waterfall-model-diagram.png&f=1&nofb=1&ipt=feb99141b28506d1da58e12c52eacf9c4ae4712c85de100f63194f1d596551f7&ipo=images" height = 400>
The Waterfall Model was the first Process Model to be introduced. It is also referred to as a linear-sequential life cycle model. It is very simple to understand and use. 

In a waterfall model:
- Each phase must be completed before the next phase can begin and there is no overlapping in the phases.
- Illustrates the software development process in a linear sequential flow.
- The phases do not overlap.

### Advantages

- Simple and easy to understand and use
- Easy to manage due to the rigidity of the model. Each phase has specific deliverables and a review process.
- Phases are processed and completed one at a time.
- Works well for smaller projects where requirements are very well understood.
- Process and results are well documented.

### Disadvantages

- No working software is produced until late during the life cycle.
- High amounts of risk and uncertainty.
- Not a good model for complex and object-oriented projects.
- Not suitable for the projects where requirements are at a moderate to high risk of changing. So, risk and uncertainty is high with this process model.
- It is difficult to measure progress within stages.

### Applications

This model is applicable in projects where:
- Requirements are very well documented, clear and fixed.
- Product definition is stable.
- Technology is understood and is not dynamic.
- There are no ambiguous requirements.
- Ample resources with required expertise are available to support the product.
- The project is short.

## Prototype Model

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmedia.geeksforgeeks.org%2Fwp-content%2Fuploads%2F20200508170244%2F11147.png&f=1&nofb=1&ipt=9a286b0ca7077b307a6519520fc4523cf2efda30c440c2e36f6872c5ebd25e79&ipo=images" style="background:#d8dee9">
