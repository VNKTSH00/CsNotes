Logic Development 

Algorithm 

    Algorithm is a step by step instruction for solving a problem 

Flowchart 

    Flowchart is a step by step diagramatic or visual representation of instructions. 

Pseudocode

    It is a method of representing a problem with the combination of natural language and programming language

Flow of a Program 

    The flow of a program can be either 
        1. Sequential 
        2. Conditional 
        3. Iterative

Arrays 

    list of operations can be done in an Arrays

        1. Array manipulation algorithms 

            - Insertion 
            - Deletion 
            - Searching 
                1. Linear Search 
                2. Binary Search 
            - Sorting 
                1. Bubble Sort 
                2. Insertion Sort 
                3. Selection Sort 
                4. Exchange Sort 
                5. Merge Sort 

Properties of Good Design 

    - Component a Independence 
    - Fault prevention and fault tolerance 
    - Design for change 

    With good module design: 

    - Maximal Relationships within modules (Cohesion)
    - Minimal Relationships between modules (Coupling)
    - This is the main contribution of structured design 

    With poor module design 

    - Hard to understand 
    - Hard to locate faults 
    - Difficult to extend or enhance 

Coupling 

    Coupling is the degree of interaction between two modules 

    - When two modules are tightly coupled when they depend a great deal on each other 
    - Uncoupled modules have no interconnections at all. They are completely unrelated

Types of coupling 

    - Content Coupling (best)
    - Common Coupling 
    - Control Coupling 
    - Stamp Coupling 
    - Data Coupling (worst)

    Content Coupling 

        - Occurs when one component modifies and internal data item in another component, or when one component branches inot the middle of another component 

    Common Coupling 

        - Two modules have write access to the same global data 

    Control Coupling 

        - One module passes an element of control to the other 
        - It is impossible for the controlled module to function without some direction from the controlling module 

    Stamp Coupling 

        - Data structure is passed as parameter, but the called module operates on only some of individual components 

    Data Coupling 

        - Every argument is either a simple arguement or a data structure in which all elements are used by the called module
    
Cohesion 

    Cohesion refers to the dependence within and among a module's internal elements(data, functions, internal modules ). Greater the cohesion, the better is the program design 

Types of cohesion 

    1. Functional Cohesion  (best)
    2. Sequential Cohesion 
    3. Communicational Cohesion 
    4. Procedural Cohesion 
    5. Temporal Cohesion 
    6. Logical Cohesion 
    7. Co-incidental Cohesion (worst)

    Functional Cohesion 

        - Functionally cohesive moduel performs exactly one action. Highly recommended cohesion 

    Sequential Cohesion 

        - Elements are involved in activities such that output data from one activity becomes input data to the next activity 
    
    Communicational Cohesion 

        - Module which has activities executed sequentially and work on same data 

    Procedural Cohesion

        - Similar to temporal and functions pertain to some related action or purpose

    Temporal Cohesion 

        - Module's data and functions are related because they are used at the same time in an execution. Elements are grouped by when they are processed. 
    
    Logical Cohesion 
     
        - Here, elements perform similar tasks and the activities to be executed are chosen from outside the module. 
        - Operations are related, but the functions are significantly different. 

    Co-incidental Cohesion 
    
        - Module performs multiple, completely unrelated actions

    









    