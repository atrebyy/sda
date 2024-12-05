### Lecture 1: Introduction to Software Architecture

#### **Welcome to the course on Software Design and Architecture!**  
In this lecture, we will explore the foundational concepts of software architecture, its goals, structures, and related disciplines like system and enterprise architectures. Let’s dive into the details step-by-step.

---

### **What is Software Architecture?**

**Definitions:**
1. **Martin Fowler:**  
   - "The highest-level breakdown of a system into its parts; the decisions that are hard to change; there are multiple architectures in a system; and architecture boils down to whatever the important stuff is."

2. **Philippe Kruchten et al.:**  
   - Software architecture involves significant decisions about organizing a system, selecting structural elements and interfaces, behavior, composition, architectural styles, and addressing functionality, usability, resilience, performance, constraints, and trade-offs.

3. **Bass, Clements, and Kazman:**  
   - "Software architecture is the structure of the system, comprising its elements, their externally visible properties, and their relationships. It focuses on the public side of interfaces, not the internal implementation."

---

### **Goals of Software Architecture**
1. Expose system structure while hiding implementation details.
2. Realize use cases and scenarios.
3. Address stakeholder requirements.
4. Balance functional and quality requirements.

---

### **Architectural Structures**

1. **Module Structures:**  
   - **Definition:** Decisions about how the system is organized into code or data units (modules).  
   - **Static perspective:** Assigns functional responsibilities.  
   - **Key Questions:**
     - What is each module responsible for?
     - What other software does it depend on?
     - How are modules related (e.g., generalization, specialization)?

2. **Component-and-Connector Structures:**  
   - **Definition:** Focuses on elements with runtime behavior (components) and their interactions (connectors).  
   - **Key Questions:**
     - How do components interact at runtime?
     - What shared data exists?
     - Can parts of the system run in parallel?
     - Can the system's structure evolve during execution?

3. **Allocation Structures:**  
   - **Definition:** Shows relationships between software elements and external environments (e.g., hardware, networks, teams).  
   - **Key Questions:**
     - Which processor executes each software element?
     - Where are software elements stored?
     - How are elements assigned to development teams?

---

### **What Makes a Good Architecture?**

#### **Process Recommendations:**
1. Architecture should originate from a small, cohesive team.
2. Base architecture on prioritized, well-specified quality requirements.
3. Document using views addressing key stakeholders' concerns.
4. Evaluate architecture against quality attributes.
5. Enable incremental implementation for early issue detection.

#### **Product/Structural Recommendations:**
1. Use well-defined modules based on information hiding and separation of concerns.
2. Leverage well-known architectural patterns and tactics.
3. Avoid dependencies on specific product versions.
4. Separate data producers from consumers.
5. Allow dynamic assignment of processes to processors.
6. Minimize interaction methods among components.
7. Clearly specify resource contention areas.

---

### **System vs. Enterprise Architectures**

1. **System Architecture:**  
   - Maps software to hardware and considers human interactions.
   - Focuses on qualities like performance, reliability, and availability.

2. **Enterprise Architecture:**  
   - Aligns the organization’s processes, information flow, and systems with strategic goals.
   - Specifies data models and interaction rules between systems.

---

### Interactive Questions (Answers Hidden in Markdown)

**Question 1:**  
What are the three types of architectural structures, and how do they differ?

<details>
<summary>Answer</summary>
Module structures focus on static organization (e.g., functional responsibilities); component-and-connector structures emphasize runtime interactions (e.g., components, connectors); allocation structures relate software to external environments (e.g., processors, teams).  
</details>

**Question 2:**  
Why is incremental implementation considered a good practice in software architecture?

<details>
<summary>Answer</summary>
Incremental implementation enables early issue detection, avoids large-scale integration problems, and ensures continuous feedback.  
</details>

**Question 3:**  
What distinguishes enterprise architecture from system architecture?

<details>
<summary>Answer</summary>
Enterprise architecture aligns software systems with business processes and strategic goals, while system architecture focuses on mapping software to hardware and addressing system qualities like performance and reliability.  
</details>

---

### Multiple Choice Questions (MCQs) (Answers Hidden in Markdown)

**Question 1:**  
What is the primary goal of software architecture?  
- [ ] A) To define programming languages to be used.  
- [ ] B) To expose system structure and hide implementation details.  
- [ ] C) To create only runtime component interactions.  
- [ ] D) To design only user interfaces.

<details>
<summary>Answer</summary>
B) To expose system structure and hide implementation details.  
</details>

**Question 2:**  
Which type of architectural structure deals with runtime behavior?  
- [ ] A) Module structures  
- [ ] B) Allocation structures  
- [ ] C) Component-and-connector structures  
- [ ] D) Enterprise structures

<details>
<summary>Answer</summary>
C) Component-and-connector structures  
</details>

**Question 3:**  
What is a key recommendation for making a good architecture?  
- [ ] A) Depend on the latest product versions.  
- [ ] B) Use undocumented approaches.  
- [ ] C) Clearly specify resource contention areas.  
- [ ] D) Ensure a one-to-one module-to-component correspondence.

<details>
<summary>Answer</summary>
C) Clearly specify resource contention areas.  
</details>

---

Does this explanation align with the lecture? Let me know if you'd like to explore any topic further!
