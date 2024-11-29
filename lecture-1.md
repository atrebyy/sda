### Lecture 1: Introduction to Software Architecture and Design

---

#### **Key Concepts of Software Architecture**
1. **Definition**:
   - **Martin Fowler**: The highest-level breakdown of a system into parts; decisions that are hard to change and are architecturally significant throughout a system's lifecycle.
   - **Philippe Kruchten et al.**: Involves selecting structural elements and their interfaces, specifying behavior, and adhering to an architectural style to meet functional and quality requirements.
   - **Bass, Clements, Kazman**: Structures of the system, relationships among components, and externally visible properties.

2. **Goals**:
   - Expose system structure while hiding implementation details.
   - Address requirements of stakeholders.
   - Handle both functional and quality requirements.

---

#### **Types of Architectural Structures**
1. **Module Structures**:
   - Static system representation: modules, areas of functional responsibility.
   - Questions addressed:
     - Functional responsibility of each module.
     - Dependencies among modules.

2. **Component-and-Connector Structures**:
   - Runtime elements (components) and interactions (connectors).
   - Questions addressed:
     - Major components and runtime interactions.
     - System’s parallelism and structure dynamics.

3. **Allocation Structures**:
   - Mapping software elements to non-software environments.
   - Questions addressed:
     - Processor assignments.
     - Directories or files during development.
     - Team assignments for software elements.

---

#### **What Makes a Good Architecture?**
1. **Process Recommendations**:
   - Led by a single architect or small team with a technical leader.
   - Prioritized quality attribute requirements guide decisions.
   - Use architectural views tailored to stakeholder concerns.
   - Allow incremental implementation for early issue detection.

2. **Product Recommendations**:
   - Use well-defined modules with separation of concerns.
   - Leverage known architectural patterns and tactics.
   - Avoid dependency on specific commercial products or tools.
   - Maintain flexibility for module-to-processor assignments.

---

#### **System vs. Enterprise Architecture**
1. **System Architecture**:
   - Integrates hardware, software, and human interactions.
   - Focuses on qualities like performance, reliability, and availability.

2. **Enterprise Architecture**:
   - Aligns software systems with business goals.
   - Defines data models and rules for system interactions.

---

### **Questions**

1. **What are the three types of architectural structures?**
   <details>
   <summary>Answer</summary>
   - Module Structures
   - Component-and-Connector Structures
   - Allocation Structures
   </details>

2. **List three process recommendations for creating good software architecture.**
   <details>
   <summary>Answer</summary>
   - Led by a single architect or small team.
   - Use well-specified, prioritized quality attribute requirements.
   - Incremental implementation to discover issues early.
   </details>

3. **Differentiate between system and enterprise architecture.**
   <details>
   <summary>Answer</summary>
   - System architecture maps functionality to hardware/software and emphasizes performance, reliability, and human interaction.
   - Enterprise architecture focuses on aligning software systems with organizational goals, information flow, and data models.
   </details>

---

### **Definitions**
1. **Software Architecture**: Decisions about the structure, behavior, and style of software systems.
2. **Quality Attribute Requirements**: Non-functional requirements like performance, usability, and resilience.
3. **Architectural Patterns**: Reusable solutions to common design problems, such as MVC or Microservices.

---

### **MCQs for Self-Assessment**

#### Question 1
**What is the primary goal of software architecture?**  
1. Expose the system's structure.  
2. Hide implementation details.  
3. Both 1 and 2.  
4. Neither 1 nor 2.  

<details>
<summary>Answer</summary>
3. Both 1 and 2.
</details>

---

#### Question 2
**Which of the following is NOT a type of architectural structure?**  
1. Module Structure  
2. Component-and-Connector Structure  
3. Allocation Structure  
4. Behavioral Structure  

<details>
<summary>Answer</summary>
4. Behavioral Structure
</details>

---

#### Question 3
**What is the role of an enterprise architecture?**  
1. Align software systems with business goals.  
2. Integrate software with hardware.  
3. Focus on quality attributes like performance.  
4. Design human interactions.  

<details>
<summary>Answer</summary>
1. Align software systems with business goals.
</details>
