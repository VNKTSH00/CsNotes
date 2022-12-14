Software Engineering Fundementals 

    - Software Development Cycle 
    - Waterfall model 
    - V model 
    - Prototype model 
    - RAD 
    - Spiral Model 
    - ETVX

Software Engineering is the application of a systematic, disciplined, quantifiable approach to the design, development, operation and maintenance of software 

Software Crisis
 
    - Software fails to meet the user requirements 
    - Software crashes frequently 
    - Development of Software became expensive 
    - Difficult to alter, debug, and enhance the software 
    - Software was often delivered late 
    - Software used resources non-optimally 

Software Development Life Cycle (SDLC)

// Software Development Life Cycle is the process used in a project to develop a software product 

    Planning -> Requirement Analysis -> Design -> Implementation -> Testing -> Deployment -> Maintenance 

Phases of SDLC

    Feasiblity -> Analysis -> Design -> Implement -> Test -> Maintain -> Feasiblity 

    Analysis 

        - Requirements gathering and Analysis 
        - Preparing SRS (Software requirement Specification) which is the primary artifact of Analysis Phase

    Design 

        - Software design deals with tranforming the customer requirements into a set of doucments that is suitable implementation in a programming language 
        - It is the process of defining the architecture, interface, component and other characteristics of a system 
        - The design stage takes thre requirements identified in the approved requirement docuemnt (SRS) as its initial input

        DD(Design Document = HLD + LLD)

        levels of design 

            - High level design 
                    1. Architecture Design 
                    2. Data Design 
                    3. Interface Design  

            - Low level design 
                    1. Writing the destailed Algorithm 
                    2. Module Design 

    Construction (Code + Unit Testing)

        - Modular and subsystem programming code will be accomplished during this stage 
        - unit testing / Module testing is done in this stage by the developers
        - This stage produces the source code, executable, and databases applicable 

Testing 

        // Testing is the process of executing the program with the intent of finding errors 
        // Software testing is a process of verifying and validating that a software application or program meets the business and technical Requirements

            Verification -> Confirms that the software meets its technical specifications 
            Validation   -> Confirms that the software meets the business Requirements
            Defect       -> Variance between the expected and actual result 

    levels of Testing 

            - Unit Testing (Module Testing) -> Done by the developer where every unit is tested to check its functional correctness  
            - Integration Testing           -> Is done to check the interface errors between the integrated components 
            - System Testing                -> Testing the integrated system is tested as a whole to check system is functionally or non-functionally correct 
            - Acceptance Testing            -> Is done by the end user for the system accpetance 

Maintenance

        // Any change that is made to the software after is deployed is known as maintenance

SDLC models 

    - Waterfall Model 
    - V Model 
    - Prototype Model 
    - RAD (Rapid Application Development)
    - Incremental Model 
    - Spiral Model 

    Waterfall Model (linear Sequential Model)

        Requirements -> Design -> Implementation -> Verification -> Maintenance 

        // Flow is from one phase to another 
        // Each phase has a well defined start and end point, with identifiable deliverables to the next phase 
        // Can't retrieve to previous phase

        Advantages 

            - Simple and easy to use 
            - Easy to manage due to the rigidity of the model - each phase has a specific deliverables and a reiview process 
            - Phases are processed and completed one at a time 
            - Works well for smaller projects where requirements are very well understood 
            - Linear approach 
            - Equivalent importance to all the phases 
            - Contract Related issues can be addressed effectively 

        Limitations 

            - Suitable only when the requirements are well-defined and stable 
            - Backtracking is high cost 
            - Increaased development of time and cost 
            - Systesm must be defined up front 
            - Hard to estimate costs & project overruns 

        Suitable scenarios 

            - Software requirements are clearly defined and known 
            - Product definition is stable 
            - Software development technologies and tools are well known 
            - New version of the existing software system is created

    V Model (Verification and Validation is done side by side)

        // Extension of Waterfall model 
        // Each phase must be completed before the next phase begins
        // Testing is emphasised in this model more than in the waterfall model 
        // It is a structured approach to testing 
        // Testing is done from the earlier stage therby bringing high quality into the development of our products 
        
            Verification process 

                            Requirement Gathering -> System Analysis -> Software Design -> Module Design -> Coding 

            Validation Process 

                -> Coding -> Acceptance Testing -> System testing -> Integration Testing -> Unit Testing 

        Advantages 

            - Validation and Verification at each level of teh stage contaiment 
            - Stage containment mechanism 
            - Avoids the downward flow of defect 
            - Lower defect Resolution cost due to earlier detection 
            - Allows testers to be active from the initial state of the project life cycle 
        
        Limitations 

            - Least Flexible 
            - Rigid 
            - Backtracking cost is high in case of a problem 
            - increased develpoment time and cost 
            - Hard to estimate costs & project overruns 
    
    Prototype Model 

        // Creates prototypes, which is an incomplete version of the software program being developed. 
        // Simulates only few aspects of the features of the system built 

        // Prototyping can also be used by the end users to describe and prove requirements that the developers have not considered 
        // Developres build a prototype during the requirements phase 
        // Prototype is evalvulated by the end users to provide crrective feedback 
        // Developers futher refine the prototype based on feeback 
        // when the user is satisfied, the prototype code is brought up to the standards needed for the final product 
    
        Identify basic requirements -> Develop Initial Prototype -> Review -> Revise and enhance the Prototype 

        Types of prototype model 

            1. Throw away (quick & Dirty)

                Preliminary Requirement -> Design the prototype -> suggestion from users -> final requirements -> Rapid construction 
                
                // when the requirements are unclear

                // Involves quick requirement assessment, Analysis, design 
                // Focuses on rapid construction 
                // Ad-hoc development approach 
                // Discards prototype after the objective is met 

            2. Evolutionary 
                
                Analysis and Quick Design -> (Refine -> Develop -> Demostrate -> Refine) -> Testing -> Deployment 

                // when the requirements are unstable 

                // Requirements are prioritized and the code is developed initially for stable requirements, with an eye on quality 
                // Software is continuously refined and augmented in close collaboration with the client 
                // Build the software incrementally 
                // Adopt rigorous, systematic approach 
                // Iterative model 

        Advantages

            - Reduced Time and Cost 
            - Active user involvement 
            - Client gets the feel of the product early in the project life cycle 
            - Steady, visible signs of progress produced. 
            - Interaction with the prototype simulates awareness of additional needed functionality 
    
        Limitations

            - User might get confused with the prototype model and the finished product 
            - Documentation is absent 
            - Expense of implementing the prototype is high, therby affecting the development costs 

    RAD (Rapid Application Development)

        // RAD is a high speed version of the linear sequential model 
        // RAD is an incremental model 
        // Characterized by a very short development life cycle 
        // The RAD model follows a component based appraoch 
        // Individual components are developed by different people and assembled to develop a lare software system 

        Phases of RAD

            - Business Modelling        (Information flow is identifed in various modules)
            - Data Modelling            (Information gathered is used to define data objects)    
            - Process Modelling         (Objects are converted to achieve the business objective)
            - Application generation    (Automated tools are used to convert process modesl into the actual system)
            - Testing and turnover      (New components along with all the interfaces are tested)

        Advantages 

            - Due to the emphasis on rapid development, it results in the delivery of a fully functional project in a short period
            - Facilitates rapid development 

        Limitations

            - Developers and clients must be committed to rapid-fie activities in an abbrivated time frame. 
            - If either party is indifferent in needs of other, the project will run into series problem 
            - It is not suitable for large projects

        Suitable scenarios

            - When requirements are not fully understood 
            - User is involved throughout the life cycle 
            - System can be modularized 
    
    Incremental Model 

        // The incremental model prioritizes requiremnts of the system and implements them in groups 
        // Each subsequent release of the system adds function to the previous release, until all designed functionalities have been implemented 
    
        Advantages

            - Users 'divide and conquer' breakdown of tasks 
            - High-risk or major functions are addressed in the first increment cycles
            - Each release delivers an operational product 
            - Customer can repsond to each build 
            - Customers get important functionality early 

        Limitations 

            - Requires early definition of a complete and fully functional system to allow for the definition of increments 
            - Requires good planning and design as basis for the system 
            - Absence of a well-defined moduel interface is a major obstacle for this model of development 

        Suitable Scenarios 

            - When most of the requirements are known up-front but are expected to evolve over time 
            - When projects have lengthy development schedules 

    Spiral Model 

        // Suitable for technically challenging software products that are prone to several kinds of risks 
        // Accomodates prototyping. This model combines the features of the prototyping model and the waterfall model 
        // It is favoured for large, expensive and complicated models
        // Suggested for High-Risk scenarios based projects

        Advantages

            - Provides early indication risk 
            - Users see the system early because of rapid prototyping tools
            - Critical high-risk functions are developed first
            - Eraly and frequent feedback from users

        Limitations 

            - Time spent for evaluating risks are too large for small or low-rick projects and may not prove cost-worthy 
            - Time spent on planning, resetting objectives, doing risk analysis and prototyping may be excessive 
            - Relies on Risk assessment expertise 
        
        Suitable Scenarios 

            - Risk perceived is very high 
            - Requirements are complex
            - Significant changes are expected 
    
    ETVX Model (Entry -> Task -> Validation -> Exit)

        // IBM introduced the ETVX Model to document their Process
        // Each phase in a process performs a well-defined task and generally produces an output 

        EVTX Analogy example 

            - Entry 
                1. Hall Ticket 
            - Task 
                1. Show Hall Ticket 
                2. Get Question Paper 
                3. Get Answer Sheet 
                4. Write Answer for Respective questions 
            - Verification 
                1. Verify whether questions are written for appropriate questions 
                2. Review the answers written 
            - Exit 
                1. Submission of the answer sheet to the invigilator 

            - Entry 
                1. Feasiblity Report  
            - Task 
                1. Collect Requirement 
                2. Analyze Requirement
                3. Write SRS
            - Verification 
                1. Review SRS
            - Exit 
                1. SRS











        
