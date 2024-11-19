### **Lecture 5: Architecture Representation and Views**  
*How we represent software architecture, the various types of architectural views, and their importance in addressing different concerns of stakeholders. Explore the tools and techniques used for documenting architecture effectively.*

---

### **1. What Are Architecture Views?**  
**Definition:**  
Architecture views are **formal models** of a software system. They document the architecture and focus on specific concerns from particular perspectives.  

#### **Key Characteristics:**
1. Each view omits entities irrelevant to its specific perspective.  
2. The **entities** in a view are described in terms of **components** (building blocks) and **connectors** (relationships).  

**Example:**  
An execution view might focus on runtime interactions between processes, while an allocation view could show how modules are assigned to teams or hardware.

**Interactive Pause:** Why do you think documenting different views is essential for stakeholders?  

---

### **2. The Three Basic Views**  
The software industry has settled on **three primary architectural views**, though many more can be considered:  

#### **A. Conceptual View (Structural View):**  
- Focuses on domain-level functionality and relationships.  
- **Components:** Modules, classes, or packages.  
- **Connectors:** Relationships like inheritance or dependency.  
- **Key Questions Answered:**  
  - What responsibilities are assigned to each module?  
  - What are the relationships between modules?  
  - How is the system structured in terms of code units?  

**Example:**  
In a class-based structure:  
- Modules = classes.  
- Connectors = "inherits-from" or "uses" relationships.  

---

#### **B. Execution View:**  
- Focuses on runtime behavior and dynamic interactions.  
- **Components:** Processes or threads.  
- **Connectors:** Messages, data exchanges.  
- **Key Questions Answered:**  
  - How do components interact at runtime?  
  - What parts can run in parallel?  
  - How does data flow through the system?  

**Example:**  
A concurrency structure that identifies opportunities for parallel execution to enhance performance.

---

#### **C. Allocation View:**  
- Focuses on the relationship between software elements and their environment.  
- **Components:** Software modules, libraries, developers, hardware.  
- **Connectors:** Assignments (e.g., "assigned-to," "stored-in").  
- **Key Questions Answered:**  
  - How are elements mapped to hardware?  
  - What is the file structure during development?  
  - How are responsibilities assigned to development teams?  

**Example:**  
Mapping a database module to a specific server in a deployment scenario.

---

### **3. Beyond the Basics: Specialized Views**  
For complex systems, additional views may be necessary:  
1. **Data/Information View:** Focus on data structures and persistence (e.g., database design).  
2. **Physical View:** Describes hardware architecture, including servers and firewalls.  
3. **Security View:** Highlights security mechanisms and protocols.  

**Guidelines:**  
- Add a **physical view** for network-based systems.  
- Add a **security view** for high-security systems.  
- Add a **data view** for business-critical systems.

---

### **4. Tools for Representing Architecture Views**  
Unified Modeling Language (UML) is commonly used to represent and document architectural views. UML provides both **structural** and **behavioral** diagrams:  

#### **Structural Diagrams:**
- **Class Diagram:** Shows classes and their relationships.  
- **Component Diagram:** Depicts components and their interfaces.  
- **Package Diagram:** Groups elements logically.  
- **Deployment Diagram:** Maps software to hardware.  

#### **Behavioral Diagrams:**
- **Sequence Diagram:** Visualizes interactions over time.  
- **State Machine Diagram:** Depicts state transitions.  
- **Activity Diagram:** Defines workflows and processes.  

---

### **5. Examples of Good Architectural Practices**
1. Separate data-producing modules from data-consuming modules.  
2. Ensure processes/tasks can be easily reassigned to different processors.  
3. Use simple, consistent interaction patterns.  

---

### **6. Real-World Application: Sales Order Business Process**  
Let’s consider the sales order process as an example:  

#### **Conceptual View:**  
- Modules: Order Management, Shipping, Payment.  
- Connectors: Interfaces for communication between modules.  

#### **Execution View:**  
- Components: Order processing threads, shipping processes.  
- Connectors: Messages exchanged between processes.  

#### **Allocation View:**  
- Work Assignment: Developers assigned to modules.  
- Deployment: Modules distributed across servers.  

---

### **Interactive Questions**
1. **Why might an execution view be more critical for a real-time system than a conceptual view?**  
2. **What would be the focus of an allocation view for a distributed cloud-based system?**  
3. **How do UML diagrams help stakeholders understand architecture?**  
4. **Which additional view would you prioritize for a high-security online banking system? Why?**

---

### **MCQs to Test Understanding**

1. **Which architectural view focuses on runtime behavior?**  
   a) Conceptual View  
   b) Execution View  
   c) Allocation View  
   d) Security View  

2. **In which view would you map modules to specific hardware?**  
   a) Conceptual View  
   b) Execution View  
   c) Allocation View  
   d) Physical View  

3. **Which UML diagram would best represent runtime interactions?**  
   a) Class Diagram  
   b) Sequence Diagram  
   c) Deployment Diagram  
   d) Package Diagram  

4. **Which view is critical for assigning development responsibilities in a large team?**  
   a) Allocation View  
   b) Data View  
   c) Execution View  
   d) Conceptual View  

5. **Which of the following is a characteristic of a good architectural structure?**  
   a) All modules should handle both data production and consumption.  
   b) Tasks should be tightly coupled to specific processors.  
   c) Processes should have simple interaction patterns.  
   d) Every process must include redundant interactions.  
