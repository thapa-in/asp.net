### Managed Code	
---
1. `CLR` executes code
2. Code compile **C#** to **IL** then **Native**

Original | by Compiler | by CLR
--- | --- | ---
*C# code* | `Intermediate Language` | **Native**

3. Provide Services in runtime 
	- Garbage collector
	- Type checking
	- Exception Handling
4. Example : **C#**

### UnManaged Code		
----------------------------------------
1. `OS` executes code
2. Code direct compile **C#** to **Native**

Original  | by CLR
--- | ---
*C# code* | **Native**

3. Not Provide Services in runtime. 
   Programmer has to take care these services
	- Garbage collector
	- Type checking
	- Exception Handling
5. Example : **C**, **C++**
