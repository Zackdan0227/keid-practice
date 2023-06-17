## 00:
1. BIOS is the software for controlling hardware connected to the data, responsible for running OS
2. JVM is the software that allows different OS to run Java programs
3. Input device, storage, arithmetic, control device, output device
4. Unix, Linux, Microsoft, Mac OS, IOS, BSD
5. C, Java, R, Ruby, Swift,Perl, Python

## 01:
1. The waterfall development process is a sequential and linear approach to software development.
2. Each phase typically relies on the completion of the previous phase before proceeding, lack flexibility in accommodating changes or feedback that arise later in the development process. 
3. Prototyping emphasizes quick validation of requirements, Agile focuses on iterative development and collaboration, and Spiral emphasizes risk management in a structured iterative process. 

## 02:

1. while external design focuses on defining the overall system structure and user experience, internal design delves into the technical implementation details and ensures the software is well-structured and maintainable. Both design aspects are essential for the successful development of software that meets user requirements and technical specifications.
2. Imagine we have componenet A, B, and C, they are developed sequentialy. If we are doing a bottom up testing, drivers can be used to test individual componenet C, when A and B are not finished yet. 
    - Driver example:
    ```
    # Driver for Component B
    def driver_for_b():
        input = "expected_input"
        result = component_c(input)
        if result == "expected_output":
            print("Component C works correctly with input: ", input)
        else:
            print("Component C failed with input: ", input)

    # The real Component C
    def component_c(input):
    ```
    Stubs can be used as 'dummies' to mimic the behavior of a lower-lever module.

    - Stub example:
    ```
    # Stub for Component B
    def component_b_stub(input):
        if input == "expected_input":
            return "expected_output"
        else:
            return "error"
    ```
