### **Lecture 4: Architectural Styles**  
*Exploring **architectural styles**, their properties, and how they guide the design of software systems. Providing a framework for selecting and applying these styles in your projects.*

---

### **1. What Are Architectural Styles?**  
An **architectural style** is a **named collection of design decisions** that:  
1. Apply to a specific development context.  
2. Constrain design decisions for systems within that context.  
3. Result in systems with desirable qualities like scalability, efficiency, or evolvability.  

---

### **2. Basic Properties of Styles**  
Every architectural style provides:  
1. **A Vocabulary:**  
   - Components and connectors (e.g., pipes, filters, servers).  
2. **Configuration Rules:**  
   - Define how components and connectors are composed (e.g., a filter can connect to only one pipe).  
3. **Semantic Interpretation:**  
   - Gives meaning to the compositions (e.g., data flows from source to destination in pipe-and-filter).  

**Benefits:**  
- Design and code reuse.  
- Improved system understandability.  
- Interoperability and standardization.  
- Style-specific analysis and visualizations.  

**Interactive Pause:** Why do you think vocabulary and rules are essential for architectural styles?  

---

### **3. Common Architectural Styles**  

#### **A. Layered Style**  
- Components are grouped into layers, each providing services to the layer above and consuming services from the layer below.  
- **Connectors:** Communication protocols or interfaces (APIs).  

**Example:**  
- Client-Server architecture.  
- Three-tier architecture (UI → Business Logic → Database).  

**Advantages:**  
- Loose coupling and separation of concerns.  
- Scalability and maintainability.  

---

#### **B. Data-Flow Styles**  

1. **Batch Sequential:**  
   - Data is passed as a complete batch between processing components.  
   - **Example:** Transaction processing in financial systems.  

2. **Pipe-and-Filter:**  
   - Components (filters) transform data incrementally, and connectors (pipes) transfer data between components.  
   - **Example:**  
     - UNIX command pipelines: `ls | grep "log" | sort`.  

**Advantages of Pipe-and-Filter:**  
- Reusability and concurrent execution.  

**Disadvantages:**  
- Not suitable for interactive applications.  

---

#### **C. Blackboard Style**  
- Used for problems without deterministic solutions.  
- **Components:**  
  - Central blackboard (data store).  
  - Agents that contribute to solutions.  

**Example:**  
- AI systems for speech recognition or protein structure identification.  

**Advantages:**  
- Facilitates collaboration among independent components.  
- Suitable for exploratory or heuristic-based systems.  

---

#### **D. Rule-Based Style**  
- Involves an **inference engine** that processes rules and queries in a **knowledge base**.  
- **Example:**  
  - Expert systems like medical diagnosis tools.  

**Advantages:**  
- Easy to modify behavior by adding or removing rules.  
- Highly flexible.  

**Disadvantages:**  
- Hard to manage when there are too many rules.  

---

#### **E. Implicit Invocation (Event-Based)**  
- Components announce events without specifying which other components will handle them.  
- **Example:**  
  - GUI systems, where clicking a button triggers multiple events.  

**Advantages:**  
- Decoupled components for high scalability.  

---

#### **F. Peer-to-Peer Style**  
- **Peers:** Act as both clients and servers.  
- **Example:** File-sharing systems like BitTorrent.  

**Advantages:**  
- Robust and scalable.  

---

### **4. Case Study: Lunar Lander Game**  
Let’s apply architectural styles to the **Lunar Lander game**:  
1. **Batch Sequential:** The game could calculate the next state (height, velocity) in stages.  
2. **Pipe-and-Filter:** Data streams like burn rates and velocities are processed sequentially.  
3. **Rule-Based Style:** Rules govern the game logic, such as "if velocity exceeds X, the ship crashes."  

---

### **5. Style Analysis Dimensions**  
When evaluating an architectural style, consider:  
- What is the design vocabulary (components and connectors)?  
- What structural patterns are allowed?  
- What are its strengths and limitations?  
- In which domains is it commonly applied?  

**Interactive Pause:** Which style do you think is best for real-time systems, and why?  

---

### **MCQs to Test Understanding**

1. **Which style processes data incrementally through independent components?**  
   a) Batch Sequential  
   b) Pipe-and-Filter  
   c) Rule-Based  
   d) Peer-to-Peer  

2. **What is a key advantage of the layered style?**  
   a) Tight coupling between layers.  
   b) Scalability and maintainability.  
   c) Single point of failure.  
   d) Complex debugging.  

3. **Which style is best suited for heuristic-based systems like speech recognition?**  
   a) Client-Server  
   b) Blackboard  
   c) Pipe-and-Filter  
   d) Peer-to-Peer  

4. **Which style uses an inference engine to process rules?**  
   a) Implicit Invocation  
   b) Rule-Based  
   c) Batch Sequential  
   d) Event-Based  

5. **In the Lunar Lander game, which style would be most efficient for computing the ship's velocity in stages?**  
   a) Pipe-and-Filter  
   b) Layered Style  
   c) Peer-to-Peer  
   d) Interpreter  
