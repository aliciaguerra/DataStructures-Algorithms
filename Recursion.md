Some computer programming languages allow a module or function to call itself. This technique is known as recursion. 
In recursion, a function a either calls itself directly or calls a function B that in turn calls the original function a.

Example: A Function Calls Itself

                           int function(int value) {
                            if(value<1)
                             return;
                            function(value-1);
                            printf("%d", value);
                            }
                            
Example: a function that calls another function which in turn calls it again

                            int function(int value) {
                             if(value < 1)
                              return;
                             function(value-1);
                             printf("%d", value);
                             }
                             
#Properties
A recursive function can go infinite like a loop. To avoid infinite running of recursive function, there are two properties
that a recursive function must have - 

- Base Critera: There must be at least one base criteria or condition, such that, when this condition is met, the function
  stops calling itself recrusively
- Progressive Criteria: The recursive calls should progress in such a way that each time a recursive call is made it becomes
  closer to the base criteria.

#Implementation
Many programming languages implement recursion by means of stacks. Generally, whenever a function (caller) calls another function (callee) or itself as callee, the caller function transfers execution control to callee. The transfer process
may also involve some data to be passed from the caller to callee. 

This implies, the caller function has to suspend its execution temporarily and resume later when the execution control
returns from the callee function. Here, caller function needs to start exactly from the point of execution where it put 
itself on hold. It also needs the exact same data values it was working on. For this purpose, an activation record (or stack
frame)is created for caller function. This activation record keeps the information about local variables, formal parameters,
returns address and all informations passed to call function.

#Analysis of Recursion
One may argue that why to use recursion as the same task can be done with iteration. The first 


                             

                           
