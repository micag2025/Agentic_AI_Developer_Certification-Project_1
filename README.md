# FIRST ROUND FEEDBACK (see email 20 June 20225) 

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
- After "Features" and before "Installation" screenshots of the UI, a new section titled **"Example UI Screenshots"** has been enclosed to show relevant UI features such as:  
   - the Home Page    
   - Pubblication Search (Details?)    
   - Q&A Chat Interface    
   - Example Query Result
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
_**The project structure has been refined**, organizing (placing) data files within appropriate subforlders (packages), based on the project structure._

Besides, following further changes (implementations):  
- Since the new section titled **"Example UI Screenshots"** has been enclosed, the code have been slightly implemented.
- **Implementation of the UI**, enclosing (displaying) a **search bar** and **list the available publications** from `project_1_publications.json` on the **main landing page**  before the chat interface (history/chat) 
  using Streamlit in app/main.p. 


**Where to place:**  
Put this code after `st.caption("Ask questions about the Ready Tensor publications.")` and before the chat history/chat input logic.

This will show a search bar and a list of publications on the main page, filtered as the user types.


It will display the **search bar** and the **list of publications** on the main landing page, before the chat interface. 
Here’s a summary of what your code does:

- **Loads publications** from `project_1_publications.json` using the `DATA_DIR` path.
- **Displays a search bar** (`st.text_input`) at the top.
- **Filters publications** based on the search query (title or description).
- **Shows the filtered publications** with their title and description.
- **Initializes chat history and agent** if not already in session state.
- **Displays chat history** and handles user queries.
- **Saves each response** to the `output/` folder.


- You are running the app with `streamlit run app/main.py`.




