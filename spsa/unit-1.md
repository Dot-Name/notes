# Evolution of Components Systems Programming

## Compiler

A compiler is a software tool that translates high-level programming code into low-level machine code that can be executed by a computer. It performs this translation in several distinct phases. Here are the key points to understand about the compilation process:

1. **Lexical Analysis**: This is the first phase of the compiler. It involves scanning the source code and breaking it down into tokens, which are meaningful units of the programming language. The lexical analyzer, also known as the scanner, reads the characters from the source program and groups them into lexemes (sequences of characters that "go together"). Each lexeme corresponds to a token. Tokens are defined by regular expressions that are understood by the lexical analyzer. The lexical analyzer also removes lexical errors, comments, and whitespace.

2. **Syntax Analysis**: The second phase of the compiler is syntax analysis, also known as parsing. In this phase, the compiler checks whether the sequence of tokens generated by the lexical analyzer follows the rules of the programming language's grammar. It builds a parse tree or an abstract syntax tree (AST) to represent the structure of the program. The parse tree/AST helps in further analysis and code generation.

3. **Semantic Analysis**: Once the syntax has been analyzed, the compiler performs semantic analysis. This phase checks whether the components of the source program are meaningful or not. It verifies that the program adheres to the semantic rules of the programming language. Semantic analysis includes type checking, scope resolution, and other checks to ensure that the program is semantically correct.

4. **Intermediate Code Generation**: After the semantic analysis, the compiler generates an intermediate representation of the source code. This intermediate code is a lower-level representation of the program that is easier to analyze and optimize. It serves as a bridge between the high-level source code and the target machine code. There are different forms of intermediate code, such as three-address code, abstract syntax trees, or bytecode.

5. **Optimization**: The next phase is optimization, where the compiler applies various techniques to improve the performance of the generated machine code. Optimization aims to reduce the execution time, memory usage, and other resources required by the program. It analyzes the intermediate code and applies transformations to make the code more efficient while preserving its functionality.

6. **Code Generation**: The final phase of the compilation process is code generation. In this phase, the compiler takes the optimized intermediate code and generates the actual machine code that can be executed by the target hardware. The code generator translates the intermediate code into a sequence of machine instructions that perform the same tasks as the original program. The generated code should have the same meaning as the source code and be efficient in terms of memory and CPU resource usage.

To summarize, the steps required for compilation are:

1. Lexical Analysis: Break down the source code into tokens.
2. Syntax Analysis: Check the sequence of tokens for adherence to the programming language's grammar.
3. Semantic Analysis: Verify the meaning and correctness of the program.
4. Intermediate Code Generation: Create an intermediate representation of the program.
5. Optimization: Apply transformations to improve the performance of the code.
6. Code Generation: Translate the optimized intermediate code into machine code.

These steps are performed in a sequential manner, with each phase taking input from the previous phase and producing output for the next phase. The compiler's goal is to produce an executable program that behaves correctly and efficiently on the target hardware.

## Assembler
An assembler is a type of computer program that takes in basic instructions and converts them into a pattern of bits that the computer's processor can use to perform basic operations. The assembler's job is to convert assembler or assembly language code into machine code that the computer can then read and execute.
**Types of assemblers**
Assembler programs bridge the gap between assembly language and machine language that the computer's processor and memory can read. The assembler type is defined by the number of times it takes the program to scan the source code to translate it into machine language. There are two main types of assemblers.

**Single-pass assembler**
A single-pass or one-pass assembler translates the entire assembly language program into its equivalent machine language program in one go. In a single scan, the assembler substitutes the pseudo or symbolic instructions in the assembly program with computer-readable machine code.

**Multipass assembler**
In a multipass assembler, the assembler must scan the assembly language program multiple times before it can be translated to its equivalent machine language avatar. In the first pass, the assembler generates a symbol code where it records and processes the pseudo instructions in assembly language. In the second pass, it generates the equivalent machine code.
**How assemblers work**
Most computers come with a basic set of instructions called assembler instructions that correspond to the basic machine operations that the computer can perform. For example, a load instruction causes the processor to move a string of bits from a location in the processor to a special holding place called a register.

A programmer uses a sequence of these assembler instructions to write the source code. The assembler program then takes each statement in the source program and generates a corresponding bit stream or pattern called the object code. This output remains relative to the input source program and can then be executed as needed. The bit stream that constitutes the object program is called the machine code.

The assembler identifies the symbolic names associated with each instruction and allocates memory to each instruction. It also maintains a program counter or location counter (LC) to keep track of the memory addresses of every instruction. As it processes these instructions, it updates the LC and generates the target machine code.

