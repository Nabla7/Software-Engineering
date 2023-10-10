# Software-Engineering

Collection of factoids and such things from our software engineering course at University of Antwerp

---

## Week 1: Introduction

### Summary (i)

#### 1. How does Software Engineering differ from programming?

   > Software Engineering encompasses the systematic design, development, and maintenance of software applications, considering aspects like requirements, design, testing, and maintenance. Programming, on the other hand, is merely the act of writing code.

#### 2. Why is programming only a small part of the cost of a “real” software project?

   > Beyond programming, a software project incurs costs in requirements gathering, design, testing, documentation, deployment, maintenance, training, and more. These activities often consume more time and resources than just writing the code.

#### 3. Give a definition for “traceability”.
   
   > Traceability refers to the ability to relate software artifacts to one another and to their source requirements, ensuring that all requirements are met and changes can be tracked throughout the software lifecycle.

#### 4. What is the difference between analysis and design?

   > Analysis focuses on understanding the problem, gathering requirements, and specifying what the system should do. Design, on the other hand, focuses on how the system will fulfill those requirements, determining the architecture, components, and their relationships.

#### 5. Explain verification and validation in simple terms.

   > Verification answers the question, "Are we building the product right?" It ensures the product meets its specifications. Validation answers, "Are we building the right product?" It ensures the product meets the user's needs.

#### 6. Why is the “waterfall” model unrealistic? Why is it still used?

   > The waterfall model assumes that each phase (like requirements, design, implementation) is completed before the next begins, which is often unrealistic as requirements can change or issues can be discovered later. However, it's still used because of its simplicity and clear structure.

#### 7. Can you explain the difference between iterative development and incremental development?

   > Iterative development involves refining the system through repeated cycles, enhancing its functionality with each iteration. Incremental development delivers the system in parts or "increments", adding new features with each increment.

### Summary (ii)

#### 1. What is your preferred definition of Software Engineering? Why?
   
   > Software Engineering is the disciplined application of engineering principles to design, develop, and maintain software systems. This definition encapsulates both the technical and process-oriented nature of the field.

#### 2. Why do we choose “Correctness” & “Traceability” as evaluation criteria? Can you imagine some others?

   > Correctness ensures the software behaves as expected, while traceability ensures changes and requirements can be tracked. Other criteria could be maintainability, efficiency, reliability, and usability.

#### 3. Why is “Maintenance” a strange word for what is done during the activity?

   > Because it often involves not just fixing bugs or updating software but also adding new features, adapting to new platforms, or improving performance.

#### 4. Why is risk analysis necessary during incremental development?

   > Incremental development introduces changes with each increment, and risk analysis ensures that these changes don't introduce unforeseen problems or jeopardize the project's success.

#### 5. How can you validate that an analysis model captures users’ real needs?

   > By involving users in the validation process, such as through reviews, walkthroughs, or prototyping, and gathering their feedback.

#### 6. When does analysis stop and design start?

   > Analysis stops once the problem is fully understood and requirements are specified. Design starts when you begin determining how to fulfill those requirements.

#### 7. When can implementation start?

   > Implementation can start after the design phase is completed and there's a clear plan for how the system will be built.

#### 8. Can you compare the Unified Process and the Spiral Model?

   > Both are iterative models, but the Unified Process is more structured with specific phases (Inception, Elaboration, Construction, Transition) and emphasizes use-case driven development. The Spiral Model focuses more on risk-driven development with repeated cycles of planning, risk analysis, engineering, and evaluation.

#### 9. Can you explain the values behind the Agile Manifesto?

   > The Agile Manifesto values:
   > - Individuals and interactions over processes and tools
   > - Working software over comprehensive documentation
   > - Customer collaboration over contract negotiation
   > - Responding to change over following a plan

#### 10. Can you identify some synergies between the techniques used during extreme programming?

   > Pair programming, continuous integration, and test-driven development synergize by promoting code quality, early defect detection, and team collaboration.


#### 11. Can you explain how the different steps in the scrum process create a positive feedback loop?
    
   > Sprints end with reviews and retrospectives, allowing the team to show progress, gather feedback, and continuously improve, creating a loop of planning, action, feedback, and adjustment.

#### 12. How does scrum reduce risk?
    
   > Scrum's iterative approach, with frequent feedback and regular adjustments, ensures that deviations from the desired outcome are caught and corrected early.

#### 13. Is it possible to apply Agile Principles with the Unified Process?
    
   > Yes, the Unified Process can be tailored to be more agile by emphasizing early and continuous delivery, close customer collaboration, and flexibility to change.

#### 14. Did the UML succeed in becoming the Universal Modeling Language? Motivate your answer.
    
   > UML has become widely accepted as a standard for modeling software systems, especially in object-oriented design. However, while it's a powerful tool, not every project or organization uses it, and some find it overly complex for certain tasks. So, while it's "universal" in the sense of being a standard, it's not universally used in every context.

## Week 2: Requirements and Use Cases

### Summary (i)

#### 1. Why should the requirements specification be understandable, precise and open?

   > Requirements should be understandable to ensure all stakeholders, from developers to clients, can comprehend them. They should be precise to avoid ambiguity, ensuring the software behaves as intended. Being open ensures they can accommodate changes as the project progresses or new information emerges.

#### 2. What’s the relationship between a use case and a scenario?

   > A use case represents a series of actions a system performs that yields an observable result of value to a particular actor. A scenario is a specific sequence of actions detailing a single path through a use case. Essentially, a use case can have multiple scenarios, including the main (happy path) scenario and alternative scenarios.

#### 3. Can you give 3 criteria to evaluate a system scope description? Why do you select these 3?

   > Clarity, Completeness, and Consistency. Clarity ensures that the description is easily understood by all stakeholders. Completeness ensures that all necessary details are captured. Consistency ensures there are no conflicting requirements or descriptions.

#### 4. Why should there be at least one actor who benefits from a use case?

   > An actor represents someone or something that interacts with the system. If no actor benefits from a use case, it suggests the use case may not have meaningful value or purpose in the context of the system.

#### 5. Can you supply 3 questions that may help you identifying actors? And use cases?

   > For Actors:
   > - Who will use the system?
   > - Who will maintain or support the system?
   > - What external systems will our system need to communicate with?
   
   > For Use Cases:
   > - What are the main functions the system must perform?
   > - What tasks will the user want to accomplish using the system?
   > - Are there any regulatory or external processes the system must adhere to?

#### 6. What’s the difference between a primary scenario and a secondary scenario?

   > A primary scenario, often called the "happy path," represents the default sequence of events that occur when everything goes as expected. Secondary scenarios represent alternative paths, accounting for exceptions or variations from the primary scenario.

#### 7. What’s the direction of the <<extends>> and <<includes>> dependencies?

   > The <<extends>> dependency indicates that a use case conditionally adds behavior to another at certain points. The direction is from the extending use case to the base use case. The <<includes>> dependency indicates that a use case always adds behavior to another. The direction is from the base use case to the included use case.

#### 8. What is the purpose of technical stories in scrum?

   > Technical stories, or "tech debt" stories, address non-functional requirements, technical improvements, or architectural changes in the system. They help maintain the system's health and ensure it remains scalable, maintainable, and performs well.

### Summary (ii)

#### 1. List and explain briefly the INVEST criteria for user stories.

   > The INVEST criteria are:
   > - **Independent**: Each story should be self-contained and not rely on another story.
   > - **Negotiable**: Details can be adjusted and discussed with the team and stakeholders.
   > - **Valuable**: Every story should deliver value to the end user.
   > - **Estimable**: The team should be able to estimate its size or effort.
   > - **Small**: Stories should be small enough to be planned and delivered in a single iteration.
   > - **Testable**: It should be clear how to test the story and verify it.

#### 2. Explain briefly the three levels of detail for Product Backlog Items (Epic, Features, Stories).

   > - **Epic**: A large chunk of work with a broad scope, which can be broken down into multiple features.
   > - **Features**: Smaller than epics but bigger than stories. They describe a specific functionality or characteristic of the system.
   > - **Stories**: Represents a small, implementable requirement that delivers value. It's often written from the user's perspective.

#### 3. What is a minimum viable product?

   > A minimum viable product (MVP) is a version of a product with just enough features to be usable by early customers, providing feedback for future product development. It allows for the quickest way to start learning about the product's viability with minimal resources.

#### 4. Define a misuse case.

   > A misuse case is a type of use case that describes how a system can be used maliciously. It's used in security analysis to identify potential threats and vulnerabilities in the system.

#### 5. Define a safety story.

   > A safety story is a user story focused on ensuring the safety of the system or its users. It might detail requirements related to preventing harm, accidents, or ensuring regulatory compliance.

#### 6. Why do use cases fit well in an iterative/incremental development process?

   > Use cases provide a clear and user-centered view of system functionality. In iterative development, they allow for incremental realization of system functionality, providing frequent feedback and ensuring the system meets user needs.

#### 7. Why do we distinguish between primary and secondary scenarios?

   > Distinguishing allows teams to focus on the main flow of the system while also ensuring that alternative paths and exceptions are considered. It provides a clearer understanding of the system's behavior in different situations.

#### 8. What would you think would be the main advantages and disadvantages of use cases?

   > **Advantages**:
   > - Provides a user-centric view of the system.
   > - Helps in understanding system functionality in real-world scenarios.
   > - Useful for communication among stakeholders.
   
   > **Disadvantages**:
   > - Can become lengthy and complex for large systems.
   > - May not capture non-functional requirements well.
   > - Requires maintenance as requirements evolve.

#### 9. How would you combine use-cases to calculate the risky path in a project plan?

   > By analyzing use cases and their scenarios, one can identify paths that have high complexity, numerous dependencies, or touch critical parts of the system. Combining these "risky" scenarios can help in creating a path that represents the highest risk in the project plan.

#### 10. Do use-cases work well with agile methods? Explain why or why not.

   > Use cases can work well with agile methods as they are user-centric and focus on delivering value. However, in agile, the emphasis is on smaller chunks of functionality (user stories). If use cases are kept lightweight and focused, they can complement agile methods; if they become too bulky, they might slow down the agile process.

#### 11. Can you explain the use of a product roadmap in scrum?

   > A product roadmap in Scrum provides a high-level view of the product's direction, goals, and planned features over time. It helps stakeholders understand the product's trajectory and ensures alignment between the Scrum team's efforts and the product's strategic goals.

#### 12. Choose the three most important items in your “Definition of Ready” checklist. Why are these most important to you?

   > - **Clear Acceptance Criteria**: Ensures everyone knows what's expected for the story to be considered complete.
   > - **Dependencies Identified**: Helps in planning and ensuring no blockers during the sprint.
   > - **Estimable**: If a story can't be estimated, it might be too vague or too big, making planning difficult.

   > These are important as they directly impact the planning, execution, and delivery within a sprint.

#### 13. Can you relate scrum user stories to some of the principles in the Agile Manifesto?

   > Yes, user stories emphasize:
   > - **Customer collaboration**: User stories are written from the user's perspective, focusing on their needs.
   > - **Responding to change**: User stories are small and can be adjusted as feedback is received.
   > - **Working software**: Each user story aims to deliver a piece of functional software.
   
   > These align with the principles of the Agile Manifesto.

#### 14. How would you turn an FMEA analysis into a misuse case diagram?

   > FMEA (Failure Mode and Effects Analysis) identifies potential failure modes and their impact. To convert this into a misuse case diagram:
   > - Identify potential system misuse from the failure modes.
   > - Model these as misuse cases, showing how a malicious actor might exploit these failure modes.
   > - Link misuse cases to regular use cases to show where the system is vulnerable.

#### 15. Elaborate on the relationship between an FMEA analysis and the variants of safety stories.



   > FMEA identifies potential failures and their effects. Safety stories aim to address safety concerns in a system. The outcomes of FMEA can be used to craft safety stories, ensuring that the identified failures are addressed in the system's requirements, and that safeguards are put in place.

---

## Week 3: Software Architecture and Design Patterns

---

### Pattern: Layered Architecture 

**Context:**
- Requirements imply various levels of abstraction (low & high level).

**Problem:**
- Need for portability and interoperability between abstraction levels.

**Solution:**
- Decompose system into layers; each layer encapsulates issues at the same level.
- Layer \( n \) provides services to layer \( n + 1 \).
- Layer \( n \) can only access services at layer \( n - 1 \).
    - Call-backs may be used to communicate back to higher layers.
    - Relaxed variant allows access to all lower layers.

**Tradeoffs:**
- How stable and precise can you make the interfaces for the layers?
- How independent are the teams developing the different layers?
- How often do you exchange components in one layer?
- How much performance overhead can you afford when crossing layers?

---

### Pattern: Pipes and Filters 

**Context:**
- Processing data streams.

**Problem:**
- Flexibility (and parallelism) is required.

**Solution:**
- Decompose system into filters, each with 1 input- and 1 output stream.
- Connect output from one filter to input of another.
    - Need a data source and data sink.
    - Variants:
        - Push filter: filter triggers next one by pushing data on the output.
        - Pull filter: filter triggers previous one by pulling data from the input.

**Tradeoffs:**
- How often do you change the data processing?
- How well can you decompose data processing into independent filters?
- Sharing data other than in/out streams must be avoided.
- How much overhead (task switching, data transformation) can you afford?
- How much error-handling is required?

---

### Pattern: Blackboard (a.k.a. Repository) 

**Context:**
- Open problem domain with various partial solutions.

**Problem:**
- Flexible integration of partial solutions.

**Solution:**
- Decompose system in 1 blackboard, several knowledge sources, and 1 control.
    - Blackboard is a common data structure.
    - Knowledge sources independently fill and modify the blackboard contents.
    - Control monitors changes and launches next knowledge sources.

**Tradeoffs:**
- How well can you specify the common data structure?
- How many partial solutions exist? How will this evolve?
- How well can you compose an overall solution from the partial solutions?
- Can you afford partial solutions that do not contribute to the current task?

---

### Pattern: Model-View-Controller 

**Context:**
- Interactive application where multiple widgets act on the same data.

**Problem:**
- Ensure consistency between the various widgets.

**Solution:**
- Decompose system into a model, and several view-controller pairs.
    - Model: provides functional core (data).
        - Registers dependent views/controllers.
        - Notifies dependent components about changes (send update).
    - View: creates and initializes associated controller.
        - Displays information.
        - Responds to notification events (receive update).
    - Controller: accepts user input events.
        - Translates events into requests to model and view.
        - Responds to notification events (receive update).

**Tradeoffs:**
- How many widgets? How consistent? Should they be “plugable”?
- Increased complexity, especially without a library of views/controllers.
- Excessive number of updates if not carefully applied.
- Close coupling between View-Controller; average coupling from ViewController to Model.

---

### Pattern: Observer 

**Context:**
- Change propagation: when one class changes (the subject) others should adapt (the observers).

**Problem:**
- Change propagation implies a circular dependency: 
    - Adapting requires the observers to access the subject.
    - Changing requires the subject to notify the observers.

**Solution:**
- Split the circular dependency; move one direction in new superclasses.
- Force observers to register themselves on a subject before they will be notified.
- Notification becomes anonymous and asymmetrical: subject notifies all observers.

**Tradeoffs:**
- Extra complexity: observers will receive more updates than necessary.
- Extra program logic to filter the applicable notifications.
- Restricts communication between subject and observer.

---

### Pattern: Abstract Factory 

**Context:**
- Class hierarchy with abstract roots representing a family of objects.
- Concrete leaves representing particular configurations.

**Problem:**
- Invoking constructors implies tight coupling with concrete leaves instead of abstract roots.

**Solution:**
- Create an abstract factory class with operations for creating all abstract roots.
- Create concrete factory classes for all possible configurations.

**Tradeoffs:**
- How many members in the family? How many configurations?
- When do you switch configurations?
- How strict are the configurations?
- Can clients rely on the abstract interfaces?

---

### Pattern: Adapter (a.k.a. Wrapper) 

**Context:**
- Merge two separately developed class hierarchies.

**Problem:**
- Class provides (most of) needed functionality but interface does not match.

**Solution:**
- Create an adapter class with one attribute of the adaptee class.
- Adapter class translates the required interface into the adaptee class.

**Tradeoffs:**
- How much adapting is required?
    - For one class.
    - For the whole hierarchy.
- How will the separately developed classes evolve?
- Does the merging work in one direction or in both directions?
- How much overhead in performance and maintenance can you afford?

---

### Pattern: MicroServices 

**Context:**
- Distributed system (cloud) with multiple access points.
- Many read access - few write and update.

**Problem:**
- Elastic scaling of access points to deal with peak demand.

**Solution:**
- Microservices structure an application as a collection of small, loosely coupled, and independently deployable services.
    - Each of these services corresponds to a specific business functionality and can be developed, deployed, and scaled independently.
    - Each service is independent and communicates with others via well-defined APIs and protocols (REST-API).

**Tradeoffs:**
- How much data sharing is needed?
    - Database per service (Database sharding — elastic split of database).
    - Event mechanism to notify updates.
- How much communication is needed?
    - Each service deployed by a separate DevOps team.
    - Business transactions that span multiple services? (the Saga pattern).
- Resilience: what if a service is down?
    - Reroute calls to failing service (the Circuit breaker pattern).

---


### Summary (i)

#### 1. What’s the role of a software architecture?

   > Software architecture defines the system’s structure and serves as a blueprint for its construction and evolution. It describes the components, their relationships, and the principles guiding their design and evolution, ensuring the system satisfies its specified requirements.

#### 2. What is a component? And what’s a connector?

   > A **component** is an independent module or unit in a system, which typically encapsulates specific functionality or behavior. A **connector** is a mechanism that facilitates communication, interaction, or cooperation among components, enabling data or control flow between them.

#### 3. What is coupling? What is cohesion? What should a good design do with them?

   > **Coupling** refers to the degree to which one component depends on another. **Cohesion** relates to how closely the internal elements of a component are related to one another. A good design should aim for low coupling and high cohesion, ensuring components are independent and maintainable while encapsulating related functionality.

#### 4. What is a pattern? Why is it useful for describing architecture?

   > A **pattern** is a reusable solution to a commonly occurring problem within a given context. In architecture, patterns are useful because they provide proven solutions, encapsulate best practices, and facilitate effective communication through a shared vocabulary.

#### 5. Can you name the components in a 3-tiered architecture? And what about the connectors?

   > Components in a 3-tiered architecture: 
   > - Presentation Layer (User Interface)
   > - Business Logic Layer (Application Server)
   > - Data Layer (Database)
   
   > Connectors may include:
   > - Data communication protocols (like HTTP, JDBC)
   > - Middleware software (like message queues)
   > - API calls or service interfaces
   
#### 6. Why is a repository better suited for a compiler than pipes and filters?

   > A repository allows components to read and write data independently without needing to manage the data flow explicitly, which is beneficial for a compiler that may require multiple passes and random access to the data. Pipes and filters may impose a linear data flow, which can be limiting for compiler design.

#### 7. What’s the motivation to introduce an abstract factory?

   > An abstract factory provides an interface to create a family of related or dependent objects without specifying their concrete classes. It allows a system to be independent of how its objects are created, composed, and represented, and enables the system to be configured with multiple families of objects.

#### 8. Can you give two reasons not to introduce an Adapter (Wrapper)?

   > - **Performance Overhead**: Adapters can introduce additional processing, potentially affecting system performance.
   > - **Complexity**: Introducing adapters can add complexity to the codebase, which may complicate maintenance and understanding.

#### 9. What problem does an abstract factory solve?

   > An abstract factory addresses the problem of creating families of related or dependent objects without having to specify their concrete classes. It promotes loose coupling and allows code to be independent of the system's object implementations, enhancing flexibility and configurability.

#### 10. List three tradeoffs for the Adapter pattern.

   > - **Flexibility vs. Complexity**: Adapters add flexibility by enabling interoperability but can increase system complexity.
   > - **Maintainability**: Adapters can isolate system dependencies, but maintaining additional adapter code can be a burden.
   > - **Performance**: Adapters enable integration but can introduce a performance overhead due to additional indirection.

#### 11. How do you decide on two architectural alternatives in scrum?

   > Decision-making in Scrum may involve:
   > - Analyzing the impact of each alternative on the product backlog and sprint planning.
   > - Evaluating how each alternative aligns with the product vision and goals.
   > - Considering feedback from all team members and possibly stakeholders.
   > - Weighing technical merits, risks, and potential impediments.
   
#### 12. What’s the distinction between a package diagram and a deployment diagram?

   > A **package diagram** shows how elements are grouped together into packages and the dependencies among them, focusing on the system's source code structure. A **deployment diagram** depicts the physical deployment of artifacts on nodes, focusing on the system's runtime configuration and communication.

#### 13. Define a sensitivity point and a tradeoff point from the ATAM terminology.

   > A **sensitivity point** is an architectural decision point where variations can significantly impact a quality attribute response. A **tradeoff point** is a decision point where satisfying one attribute means sacrificing another; it represents a balance among competing requirements.

### Summary (ii)

#### 1. What do architects mean when they say “architecture maps function onto form”? And what would the inverse “map form into function” mean?

   > "Architecture maps function onto form" means that the architecture defines how functional requirements (what the system must do) are realized in the system’s structure or form (components and connectors). Inversely, "map form into function" would mean deducing the intended functionalities or capabilities by examining the architecture or structure of the system.

#### 2. How does building architecture relate to software architecture? What’s the impact on the corresponding production processes?

   > Both building and software architecture involve designing structures to satisfy certain requirements and constraints, considering aesthetics, functionality, and performance. However, in software, changes can be more easily accommodated even after "construction", whereas in building architecture, changes become progressively harder and more costly after construction begins.

#### 3. Why are pipes and filters often applied in CGI-scripts?

   > Pipes and filters are often used in CGI-scripts because they allow for the easy chaining and composition of independent processing steps, facilitating data flow and transformation in a linear and understandable manner, which is often suitable for web request processing.

#### 4. Why do views and controllers always act in pairs?

   > In the Model-View-Controller (MVC) pattern, views and controllers act in pairs to separate concerns: the view manages the display of information, while the controller handles user input and updates the model. They work together to provide a synchronized, interactive user interface.

#### 5. Explain the sentence “Restricts communication between subject and observer” in the Observer pattern.

   > This means that in the Observer pattern, the subject (the object being observed) and the observers (the entities watching the subject) are decoupled. The subject does not need to know which observers are subscribed to it or their functionalities; it merely notifies them of changes without being concerned with how these changes are handled.

#### 6. Can you explain the difference between an architecture and a pattern?

   > Architecture refers to the overarching structure of a system, defining its components and their interactions. A pattern is a reusable solution applicable to recurring problems within a given context in architecture. Architecture is specific to a particular system, while a pattern can be applied across different systems.

#### 7. Explain the key steps of the ATAM method?

   > ATAM (Architecture Tradeoff Analysis Method) involves:
   > - Identifying architectural approaches and quality attribute goals.
   > - Evaluating how well approaches satisfy quality goals.
   > - Identifying sensitivity and tradeoff points.
   > - Presenting results to stakeholders for

