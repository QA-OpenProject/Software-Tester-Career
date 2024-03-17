# Advanced Test Automation Engineer

## Introduction and Objectives for Automation Testing
- Purpose of Automation Testing
  - Automation Scope
    - Software
    - Documentation
    - Test Cases
    - Test Data
    - Test Environment
  - Automation Necessary Activities
    - Implementation of Automation Test Cases
    - Monitoring and Controlling the Execution
    - Interpreting, Reporting and Logging the Results
  - Approaches to Automation Testing
    - API Testing: Through the public interface of the software
    - GUI Testing: Through the user interface of the software
    - Service/Protocol Testing: Through the communication protocols of the software
  - Objectives of Automation Testing
    - Improving test efficiency
    - Improving test coverage
    - Reducing test execution costs
    - Reducing test cycle time
- Success Factors for Automation Testing
  - Test Automation Architecture (TAA)
  - SUT (System Under Test) Testability
  - Test Automation Strategy
  - Test Automation Framework (TAF)

## Preparing for Automation Testing
- SUT Factors Influencing Automation
- Tools Evaluation and Selection
- Design for Testability and Automation

## General Test Architecture of Automation (gTAA)
- Introduction to gTAA
  - Principles of gTAA
    - Single Responsibility
    - Extensibility (Open-Closed Principle)
    - Replaceability (Liskov Substitution Principle)
    - Component Segregation (Interface Segregation Principle)
    - Dependency Inversion
  - Structure of gTAA
    - Test Generation
      - Support for:
        - Test Data: Developing, capturing, and deriving test data
        - Test Cases: Manually/Automatically generating test cases
      - Used to:
        - Edit and navigate test suite structure
        - Relate test cases to requirements
        - Document test design
    - Test Definition
      - Support for:
        - Test Cases: Specifying test cases(at a high/low level)
        - Test Data: Defining test data for low level test cases
        - Specifying test procedures for a test case or a set of test cases
        - Defining test scripts for the execution of test cases
        - Providing access to test libraries as needed
    - Test Execution
      - Support for:
        - Executing test cases automatically
        - Logging test executions
        - Reporting test results
    - Test Adaptation
      - Support for:
        - Controlling the test harness
        - Interacting with the SUT
        - Monitoring the SUT
        - Simulating the environment
    - Configuration Management
    - Test Management
    - Project Management
  
  ![gTAA](/99-Resources/gTAA.png)

- TAA Design
  - Technical Considerations of SUT
    - Interface of SUT
    - Data of SUT
  - Dev/QA Process Considerations
    - Test Execution Control Requirements
    - Reporting Requirements
    - Role and Access Rights
    - Established too landscape
- TAA Development
  - Synchronization of SUT and TAS evolution
  
  ![TAA Development](/99-Resources/SUTandTAS.png)
  ![TAA Development2](/99-Resources/SUTandTAS2.png)

  - Build Reuse into the TAS

## Risks and Contingences in Deployment
- Selection of Automation Approach and Planning of Development
  - Polit Project
  - Deployment
  - Development of the TAS
- Risk Assessment and Mitigation Strategies
  - Techniqcal Risks
    - Too much abstraction lead to hard to maintain
    - (Data-Driven Context) Data table can become too large to manage
    - Dependency would be deprecated
  - Deployment Risks
    - Staff Issues: Staff turnover, lack of skills
    - New SUT Versions: New versions of SUT may not be compatible with TAS
  - Potential Failure Risks
    - Migration to a different environment
- Test Automation Maintenance
  - Types of Maintenance
    - Corrective Maintenance
    - Adaptive Maintenance
    - Perfective Maintenance
    - Preventive Maintenance
  - Scope and Approach

## Reporting and Metrics
- Selection of TAS Metrics
  - External TAS Metrics
    - Automation Benefits
    - Effort to build automation test cases
    - Effort to analyze and interpret results
    - Effort to maintain automation test cases
    - Ratio of failures to defects
    - Time to execute automation test cases
    - Number of automation test cases
    - Number of defects found by automation test cases
    - Code coverage
  - Internal TAS Metrics
    - Tool Scripting Metrics
    - Automation code defect density
    - Speed and efficiency of TAS components
- Implementation of Measurement
  - Features of automation that support measurement and report generation
  - Integration with other third party tools
  - Visulization of results
- Logging of TAS and SUT
- Test Automation Reporting

## Transitioning Manual Testing to Automation

## Verifying the TAS

## Continuous Improvement