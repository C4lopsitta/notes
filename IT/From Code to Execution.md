## Compilation
```mermaid
flowchart TD

Source --> Compiler
Compiler --> Linker
Linker --> Binary
```
## Interpretation
```mermaid
flowchart TD
Source --> Interpreter
Interpreter --> Machine
```
## Bytecode
```mermaid
flowchart TD
A["Intermediate Language"]
B["Runtime Enviroment"]

Source --> Pseudo-Compiler
Pseudo-Compiler --> A
A --> B
B --> Machine
```
### Runtime Environment examples
- CLR => Common Language Runtime (C#, visual basic)
- JRE => Java Runtime Environment
- DVK => Dalvik Virtual enviroment
### Intermediate Language examples
- MSIL => MicroSoft Intermediate Language
- Bytecode (*.class*) => Java's Intermediate language
## JIT
Just In Time compilation
