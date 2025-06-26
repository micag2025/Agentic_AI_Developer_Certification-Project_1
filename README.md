# FIRST ROUND FEEDBACK 

## Publication Feedback:   
The publication includes a well-written TL;DR that effectively covers the project overview and introduction. 
While the tools section provides a general overview, it would be more impactful to specify which tool was used to implement each feature. 
Incorporating a flowchart to illustrate the application's workflow would enhance clarity and offer readers a better understanding of the system architecture.
 It’s great to see an open call for collaboration. Along similar lines, including a “Future Implementations” section would be valuable in outlining 
the project’s growth potential and guiding contributors on possible directions for expansion.
 
## Repository Feedback:   
The README is well-structured and provides a clear overview of the project. However, its effectiveness could be further enhanced by including 
usage examples or instructions on how to run the program. Your attempt at adopting a class-based modular design is commendable, and the use of 
type hints significantly improves code readability. To further strengthen type safety, consider integrating Python's typeguard decorator. 
As you scale the project, refining the project structure will be beneficial. For example, organizing utility classes and functions into dedicated 
modules, and placing data files within appropriate packages, can contribute to a more maintainable and scalable codebase.


# OVERVIEW CHANGES BASED ON THE FIRST ROUND FEEDBACK 

# Publication: 
-  While the tools section provides a general overview, it would be more impactful to specify which tool was used to implement each feature.   
_To enhance clarity and offer readers a better understanding of the system architecture, the tool section of the pubblication has been implemented with 
a **flowchart** illustrating the core workflow and system architecture of the application._

- It’s great to see an open call for collaboration. Along similar lines, including a “Future Implementations” section would be valuable in outlining 
the project’s growth potential and guiding contributors on possible directions for expansion.    
_A paragraph **"Future Implementations"** in the section "Contributing" has been enclosed to give an overview on features that users might proposed to implement 
the application._  

Besides, following further changes (implementations):   
- Short **description of the sample dataset** used, explanaing why it has been selected, and how it can be used in the application.
-  



# Repository: 
- The README is well-structured and provides a clear overview of the project. However, its effectiveness could be further enhanced by including 
usage examples or instructions on how to run the program.     
_To improve the effectiveness of the README, paragraphs such as **"Instruction"**, "**How to run locally"** and "**Usage Examples"** have been enclosed in the GitHub._  

- To further strengthen type safety, consider integrating Python's typeguard decorator.   
_To helps catch type errors during execution, not just during static analysis, **Python's typeguard decorator** has been enclosed in the .py files 
(to enforce type hints at runtime) and further the use the `@typechecked` decorator on functions._  

- As you scale the project, refining the project structure will be beneficial. For example, organizing utility classes and functions into dedicated 
modules, and placing data files within appropriate packages, can contribute to a more maintainable and scalable codebase.  
_**The project structure has been refined**, organizing utility classes and functions into dedicated modules, and placing data files within appropriate packages._    

Besides, following further changes (implementations):     
- 


