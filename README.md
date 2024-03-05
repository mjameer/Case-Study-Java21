# Case-Study-Java21

One of the application I support had been triggering frequent alerts for CPU and memory spikes as observed through Dynatrace. To address this concern, I conducted an experiment by executing its integration test cases across Java 8, Java 17, and Java 21. 

Remarkably, by simply changing the compiler with no alterations to the codebase, significant reductions were observed in heap usage, thread count, and CPU usage.

To summaries the heap reduced by 50% and CPU usage reduced by 74% between Java 8 and 21.  All this w/o code change, but if we try to refactor the code to Java 21, then the impact will be phenomenal. 

I have attached JConsole metrics for your reference, highlighting the substantial differences observed across Java versions.

Considering the potential impact, I strongly recommend evaluating the transition to Java 21 for your Java applications if performance issues are a concern.  


![image](https://github.com/mjameer/Case-Study-Java21/assets/11364104/8103a7ba-22a8-4a52-afb1-9b26d869a479)


JConsole Java 8 : 

![Java 8](https://github.com/mjameer/Case-Study-Java21/assets/11364104/e6938f70-6367-488f-b268-8f6a4e9c829d)



JConsole Java 17 : 

![Java 17s](https://github.com/mjameer/Case-Study-Java21/assets/11364104/c853493b-b3c9-4525-b830-f39af35d6389)


 
JConsole Java 21 :

![Java 21s](https://github.com/mjameer/Case-Study-Java21/assets/11364104/2a26888a-c62f-4da9-9609-ed12fff3079c)


