Datatypes and Operators 

Comments       

   1.  //                   single line comment 
   2.  /* aaaaaaaaaa        multi line comment
       */         

Java Identifiers

    - Identifiers names given to a variable, class or method  
    - Identifier names can start with an alphabet, underscore(_) or dollar sign($) 

Keywords 

    - Reserved words and cannot be used as identifiers
    - throws a compile time error 

    list of keywords in java 

    abstract        default     if              private         this
    assert          do          implements      protected       throw
    boolean         double      import          public          throws
    break           else        instanceof      return          transient   
    byte            enum        int             short           try
    case            extends     interface       static          void
    catch           final       long            strictfp        volatile
    char            finally     native          super           while   
    class           float       new             switch          continue
    for             package     synchronized

Data types

    Primitive Data types

        when the variable is going to hold a value 

        1. Boolean
            -boolean                depends on JVM
                1. True
                2. False

        2. Numeric
            - Character
                1. char             2 byte (UNICODE)
            - Integral
                1. Integer
                    a. byte         1 byte
                    b. short        2 byte
                    c. int          4 byte
                    d. long         8 byte
                2. Floating point 
                    a. float        4 byte
                    b. double       8 byte

    Reference data type             default value is null

        when the variable is going to hold an object 

        1. String 
        2. Array

Casting and Conversion 

    Implicit Coversion 
        
        - Lower size data type can be assigned to higher size data type automatically

    Explicit Conversion 

        - Casting the process of converting the value to different type than its source 

Types of Operators 

    - Arithmetic 

        1. Addition 
        2. Subtraction 
        3. Multiplication
        4. Division - gives quotient 
        5. Modulo   - gives remainder 
        6. increment (++)
        7. Decrement (--)

    - Unary Arithmetic 
    - Relational and Logical 

        1. Equalance (==)
        2. Not equal to (!=)
        3. Greater than (>)
        4. Less than (<)
        5. Greater than and equal to (>=)
        6. Less than and equal to (<=)

        7. Logial AND (&&)
        8. Logical OR (||)
        9. Logical NOT (~)

    - Bitwise 

        1. AND (&)
        2. OR (|)
        3. XOR (^)
        4. Ones Complement (~)
        5. Left Shift (<<)
        6. Right Shift (>>)
        7. Shift right zero fill (>>>)

    - Ternary 
    - Miscellaneous 

        1. Conditional Operator (?:)
            variable x = (expression) ? value if true : value if false
            - int a=10, b=2;
            - b = a > 10? a:b;

Precdence and Associativity of operators