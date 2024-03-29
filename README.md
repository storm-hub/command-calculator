
## CommandCalculator

This project provides functionality to read calculation instructions from a file and return the result. Examples of the input files can be found within the project. The solution provides a console application that can be used to calculate using test file names like ex1.txt, ex2.txt or whole path could be specified as well.

## Project Structure

**Calculators**
Contains SimpleCalculator class, that provides four basic operations: add, substract, multiply and divide.

**Converters**
Contains InstructionConverter that validates raw string array input and converts into a list of instructions.

**Models**
A set of of models used in the project.
ValidationResult demonstrates FluentAPI approach and makes the development easy to maintain and read.

**Readers** 
Contains FileReader that provides functionality to read files as array of strings. 

**UIPresenters**
Contains ConsolePresenter that provides Console.Writer functionality

**Validators**
Contains InstructionValidator class that parses and validates each instruction line to ensure that it does contain a valid command, value and the value is not zero for the divide command.

## Tests
The test project contains a range of tests to cover the positive and negative scenarios on each level. It uses Moq to mock non-direct functionaly, where needed. Fluent Assertions is used to make the tests more readable.

