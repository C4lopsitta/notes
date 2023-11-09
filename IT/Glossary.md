# EntrypointRemoved unused imports
The beginning of a program, it **must** be present in every single one of them because it's where the CPU starts executing from. It's accompanied by one or more[^1] ending point.

[^1]: Usually programs have only one entrypoint and one exitpoint but for simplicity reasons we often use more than one
# Precompiler
A piece of software that runs before the [[#Compiler|compiler]] and runs specific instructions in the code for itself that won't be present in the final program. An example of these precompiler directories are the ones in [[The C programming language|C]] that start with a `#` (*sharp*) and contain conditions, declarations and imports. These instructions actually change the structure of the file for the compiler.
# Overloading
When you have multiple methods with the same name but different parameters you do something that is defined as Overloading. Not all programming languages support this.