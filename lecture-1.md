### Lecture: Introduction to Requirements Engineering and Software Architecture

#### Topics Covered
1. **Definition and Importance of Software Architecture**
2. **Key Goals of Software Architecture**
3. **Types of Architectural Structures**
4. **Characteristics of Good Architecture**
5. **System and Enterprise Architectures**

---

### Lecture Notes

#### 1. **What is Software Architecture?**
Software architecture refers to the high-level design and organization of a software system. Key definitions include:
- **Martin Fowler's Definition:** It's the "important stuff," focusing on the decisions that are hard to change and involve multiple architectures in a system.
- **Bass, Clements, and Kazman:** Emphasizes the structures of a system, software elements, their relationships, and externally visible properties.

**Key Aspects:**
- Selection of structural elements and their interfaces.
- System behavior and organization into subsystems.
- Balancing functionality, usability, performance, and constraints.

---

#### 2. **Goals of Software Architecture**
The architecture must:
- Expose the structure while hiding implementation details.
- Fulfill all use cases and stakeholder requirements.
- Balance functional and quality requirements.

---

#### 3. **Types of Architectural Structures**
1. **Module Structures:** Static organization of code or data.
   - Questions answered: Functional responsibility, dependencies, and relationships.
2. **Component-and-Connector Structures:** Runtime behaviors and interactions.
   - Questions answered: Component interactions, parallelism, and runtime structure changes.
3. **Allocation Structures:** Relation between software and external environments.
   - Questions answered: Resource allocation and development assignments.

---

#### 4. **Characteristics of Good Architecture**
1. **Process Recommendations:**
   - Single architect or a small team with clear technical leadership.
   - Based on quality attributes and stakeholder concerns.
   - Documented with views for evaluation and incremental implementation.
2. **Product/Structural Recommendations:**
   - Well-defined modules with clear separation of concerns.
   - Use of known patterns for quality attributes.
   - Independence from specific tools or products.
   - Clear interaction methods and minimal resource contention.

---

#### 5. **System and Enterprise Architectures**
- **System Architecture:** Mapping software and hardware, emphasizing performance and reliability.
- **Enterprise Architecture:** Aligning software systems with organizational goals, specifying data models, and interaction rules.

---

### Interactive Questions

#### **Question 1:**
Why is it critical for software architecture to focus on "decisions that are hard to change"?  
<details>
<summary>Show Answer</summary>
Changing foundational architectural decisions later can be costly and may lead to significant rework, impacting the system's overall quality and timeline.
</details>

#### **Question 2:**
What are the three types of architectural structures, and what is the primary concern of each?  
<details>
<summary>Show Answer</summary>
1. Module Structures: Static organization of code/data.  
2. Component-and-Connector Structures: Runtime behaviors and interactions.  
3. Allocation Structures: Relation between software and external resources.
</details>

#### **Question 3:**
Name two characteristics of a "good architecture" according to the process recommendations.  
<details>
<summary>Show Answer</summary>
1. Developed by a small team with clear technical leadership.  
2. Based on a prioritized list of quality attribute requirements.
</details>

---

### MCQs

**Question 1:**  
What is NOT a primary concern of software architecture?  
- A) Functional responsibility.  
- B) Relationship between modules.  
- C) GUI Design and styling.  
- D) System performance.  

<details>
<summary>Answer</summary>
C) GUI Design and styling.
</details>

---

**Question 2:**  
Which type of structure considers runtime behavior?  
- A) Module Structures  
- B) Component-and-Connector Structures  
- C) Allocation Structures  
- D) Data Flow Structures  

<details>
<summary>Answer</summary>
B) Component-and-Connector Structures.
</details>

---

**Question 3:**  
What is a key aspect of enterprise architecture?  
- A) Allocation of processors to software elements.  
- B) Interaction rules between organizational systems.  
- C) Assigning functional responsibilities to modules.  
- D) Defining runtime components.  

<details>
<summary>Answer</summary>
B) Interaction rules between organizational systems.
</details>
