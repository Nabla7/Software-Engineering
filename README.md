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
   > - Presenting results to stakeholders for informed decision making.

#### 8. How can you balance emergent design with intentional architecture?

   >Emergent design evolves with changing requirements, while intentional architecture is planned up front. To balance, start with a clear, intentional architecture to set direction, but remain open to evolving the design as more is learned about requirements, technologies, and other factors during development.

#### 9. What happens when your team goes outside the boundaries of the guardrail?
   >Guardrails provide guidelines or constraints for a project. If a team goes outside these boundaries, it may introduce risks, technical debt, or deviations from the project's goals. It may require corrective actions, discussions with stakeholders, or adjustments to the guardrails themselves.

#### 10. How would you organize an architecture assessment in your team?

>An architecture assessment can be organized by:
   > - Defining clear objectives for the assessment.
   > - Assembling a diverse team including architects, developers, testers, and possibly external experts.
   > - Reviewing documentation and conducting interviews or workshops to understand the architecture.
   > - Using techniques like ATAM to evaluate the architecture against desired quality attributes.
   > - Documenting findings, recommendations, and presenting them to stakeholders.

---

## Week 4: Project Management and Scrum Enhancements

### Summary (i)

#### 1. Name the five activities covered by project management.

   > The five core activities covered by project management are:
   > - **Initiation**: Defining the project scope and objectives.
   > - **Planning**: Detailing the project's steps, resources, and timeline.
   > - **Execution**: Implementing the plan and coordinating people and resources.
   > - **Monitoring and Controlling**: Tracking progress, making adjustments as necessary, and ensuring objectives are met.
   > - **Closing**: Completing the project and evaluating its success.

#### 2. What is a milestone? What can you use them for?

   > A **milestone** is a significant event or achievement in the project timeline. Milestones can be used to:
   > - Mark key decision points.
   > - Indicate the completion of major project phases or deliverables.
   > - Provide checkpoints for evaluating progress and making adjustments.

#### 3. What is a critical path? Why is it important to know the critical path?

   > The **critical path** is the sequence of stages determining the minimum time needed to complete the project. Knowing the critical path is important because:
   > - It highlights the most important tasks.
   > - Delays in critical path tasks delay the entire project.
   > - It aids in optimal resource allocation and risk management.

#### 4. What can you do to recover from delays on the critical path?

   > To recover from critical path delays:
   > - **Fast Tracking**: Performing tasks in parallel that were initially planned in sequence.
   > - **Crashing**: Allocating more resources to critical tasks to complete them faster.
   > - **Adjusting Scope**: Reducing or modifying project requirements.
   > - **Reallocating Resources**: Shifting resources from non-critical to critical tasks.

#### 5. How can you use Gantt-charts to optimize the allocation of resources to a project?

   > **Gantt-charts** visually represent the project timeline, tasks, and their durations. To optimize resource allocation:
   > - Identify overlapping tasks and distribute resources to avoid conflicts.
   > - Allocate resources to critical path tasks first to prevent delays.
   > - Visualize resource availability and adjust task timelines accordingly.
   > - Identify idle periods and reallocate resources to maximize utilization.

#### 6. What is a “Known known”, and “Unknown known” and an “Unknown Unknown”?

   > - **Known Known**: These are things we know that we know. They are clear aspects of the project, like defined requirements.
   > - **Unknown Known**: These are things we don't know that we actually know. They might be subconscious or overlooked aspects that team members are aware of but haven't communicated.
   > - **Unknown Unknown**: These are things we don't know that we don't know. They represent unforeseen challenges or risks that arise during the project.

#### 7. How do you use PERT to calculate the risk of delays to a project?

   > PERT (Program Evaluation and Review Technique) involves:
   > - Estimating the shortest, most likely, and longest time to complete each task.
   > - Calculating the expected time and variance for each task.
   > - Determining the critical path and its overall expected time and variance.
   > - Using the variance to assess the risk of project delays.

#### 8. Why does replacing a person imply a negative productivity?

   > Replacing a team member can:
   > - Cause a learning curve for the new member.
   > - Disrupt team dynamics and collaboration.
   > - Result in loss of domain-specific knowledge from the departing member.
   > - Require training and onboarding time, reducing immediate productivity.

#### 9. What’s the difference between the 0/100; the 50/50 and the milestone technique for calculating the earned value?

   > - **0/100**: Earned value is only recognized once the task is fully completed.
   > - **50/50**: 50% of the value is recognized at the start of the task, and 50% upon completion.
   > - **Milestone**: Earned value is recognized based on predefined milestones within the task.

#### 10. Why shouldn’t managers take on tasks in the critical path?

   > Managers taking on critical path tasks can:
   > - Divert them from their primary roles of oversight and coordination.
   > - Create bottlenecks if they're unable to prioritize the task.
   > - Risk the project if they're unable to complete the task as effectively as a specialized team member.

#### 11. What is the “definition of done” in a Scrum project?

   > The “definition of done” in Scrum provides a clear and shared understanding among the team of what it means for a task, feature, or user story to be considered complete. It ensures consistency, quality, and that all acceptance criteria, testing, documentation, and other necessary activities have been addressed.

#### 12. Give a definition for a Squad, Tribe, Chapter and Guild in the spotify scrum model.

   > - **Squad**: A small cross-functional team focused on a specific feature or product area.
   > - **Tribe**: A larger collection of squads that work in related areas.
   > - **Chapter**: A group of individuals with similar skills or roles (e.g., all backend developers) from different squads.
   > - **Guild**: A community of members from across the organization interested in sharing knowledge on a specific topic.

### Summary (ii)

#### 1. Name the various activities covered by project management. Which ones do you consider most important? Why?

   > Project management activities include:
   > - Initiation
   > - Planning
   > - Execution
   > - Monitoring and Controlling
   > - Closing
   
   > I consider **Planning** and **Monitoring and Controlling** as most important. Planning sets the direction and expectations for the entire project, while Monitoring and Controlling ensures the project stays on track and adapts to any unforeseen challenges.

#### 2. How can you ensure traceability between the plan and the requirements/system?

   > Traceability can be ensured by:
   > - Using traceability matrices to map requirements to specific tasks, milestones, or deliverables.
   > - Embedding requirement identifiers in design documents, code comments, and test cases.
   > - Using specialized tools that link requirements to project artifacts.
   > - Regularly reviewing and updating the traceability artifacts as requirements evolve.

#### 3. Compare PERT-charts with Gantt charts for project planning and monitoring.

   > **PERT Charts**:
   > - Focus on task sequences and dependencies.
   > - Show the critical path and task durations.
   > - Useful for understanding task relationships and project flow.
   
   > **Gantt Charts**:
   > - Display tasks against time.
   > - Show when each task starts and ends.
   > - Useful for resource allocation and monitoring project progress.
   
   > While both are valuable, Gantt charts offer a clearer visual representation of the timeline, while PERT charts emphasize task dependencies.

#### 4. How can you deal with “Unknown Unknowns” during project planning?

   > Dealing with “Unknown Unknowns” involves:
   > - Building contingencies into the schedule and budget.
   > - Encouraging open communication so that unforeseen issues are identified and addressed quickly.
   > - Adopting an iterative approach, allowing for regular reviews and adjustments.
   > - Conducting regular risk assessments to identify and mitigate potential unknowns.

#### 5. Choose between managing a project that is expected to deliver soon but with a large risk for delays, or managing a project with the same result delivered late but with almost no risk for delays. Can you argue your choice?

   > I would choose managing a project with the same result delivered late but with almost no risk for delays. Predictability and reliability can often outweigh speed, especially when stakeholders are involved. A project with minimal risks ensures better planning, resource allocation, and stakeholder management. However, this decision would also depend on the specific context and the nature of the project's deliverables.

#### 6. Describe how earned-value analysis can help you for project monitoring.

   > Earned-value analysis provides a snapshot of project performance by comparing the planned progress (Planned Value) to the actual progress (Earned Value) and the actual costs (Actual Cost). It helps in:
   > - Identifying cost overruns or schedule slippages early.
   > - Gauging project health and forecasting future performance.
   > - Making informed decisions based on actual vs. planned metrics.

#### 7. Would you consider bending slip lines as a good sign or a bad sign? Why?

   > Bending slip lines generally indicate a deviation from the planned schedule. If the slip line bends towards the time axis, it's a bad sign, indicating the project is falling behind schedule. If it bends away, it's a good sign, indicating the project is ahead of schedule.

#### 8. You’re a project leader and one of your best team members announces that she is pregnant. You’re going to your boss, asking for a replacement and for an extension of the project deadline. How would you argue the latter request?

   > I would argue that:
   > - The departing team member possesses critical skills and knowledge that will take time for a replacement to acquire.
   > - The onboarding and ramp-up period for the new member will affect productivity.
   > - The change in team dynamics might slow down the project initially as the team adjusts.
   > - Ensuring a smooth transition and maintaining quality requires additional time.

#### 9. You have to manage a project team of 5 persons for building a C++ compiler. Which team structure and member roles would you choose? Why?

   > For a C++ compiler project, I'd structure the team as:
   > - **Lead Developer/Architect**: Oversees design, ensures alignment with technical standards.
   > - **Front-end Developer**: Focuses on lexical analysis, parsing, and syntax tree generation.
   > - **Back-end Developer**: Handles optimization, code generation, and target machine code.
   > - **Test Engineer**: Responsible for testing the compiler against various codebases, identifying bugs.
   > - **Documentation/Support Engineer**: Manages documentation, user feedback, and support.
   
   > This structure ensures each critical aspect of compiler development is addressed by a dedicated expert.

#### 10. Can you give some advantages and disadvantages of scrum component teams and scrum feature teams.

   > **Scrum Component Teams**:
   > - **Advantages**: Deep expertise in specific components; Clear ownership of components.
   > - **Disadvantages**: Potential for silos; Might struggle with end-to-end feature delivery.
   
   > **Scrum Feature Teams**:
   > - **Advantages**: Can deliver end-to-end features; Promotes broader skill sets and understanding.
   > - **Disadvantages**: Might lack deep expertise in specific components; Potential for overlapping work on shared components.

---

### Week 5: Design by Contract

### Summary (i)

#### 1. What is the distinction between Testing and Design by Contract? Why are they complementary techniques?
   
   > **Testing**: The process of executing a program or system to find errors.
   
   > **Design by Contract (DbC)**: Specifies precise and verifiable interface specifications for software components, which includes preconditions, postconditions, and invariants.
   
   > While testing aims to find and rectify bugs in a system, DbC establishes clear expectations for a component's behavior, helping prevent bugs. They're complementary because DbC sets the expectations, and testing verifies them.

#### 2. What’s the weakest possible condition in logic terms? And the strongest?
   
   > The **weakest possible condition** is always true (`True`), and the **strongest possible condition** is always false (`False`).

#### 3. If you have to implement an operation on a class, would you prefer weak or strong conditions for pre- and postcondition? And what about the class invariant?
   
   > - **Precondition**: Prefer weaker conditions to allow more flexibility for callers.
   > - **Postcondition**: Prefer stronger conditions to guarantee specific results after the operation.
   > - **Class Invariant**: Should be strong to ensure the consistency of the class's state.

#### 4. If a subclass overrides an operation, what is it allowed to do with the pre- and postcondition? And what about the class invariant?
   
   > - **Precondition**: Can be kept the same or weakened.
   > - **Postcondition**: Can be kept the same or strengthened.
   > - **Class Invariant**: Must remain unchanged.

#### 5. Compare Testing and Design by contract using the criteria “Correctness” and “Traceability”.
   
   > - **Correctness**: 
   >   - Testing: Ensures correctness by finding and fixing bugs.
   >   - DbC: Ensures correctness by defining clear contracts that the system must adhere to.
   > - **Traceability**: 
   >   - Testing: Provides traceability by linking test cases to requirements.
   >   - DbC: Directly ties the expectations (contracts) to the implementation, enhancing traceability.

#### 6. What’s the Liskov substitution principle? Why is it important in OO development?
   
   > The **Liskov substitution principle** states that objects of a superclass should be replaceable with objects of a subclass without affecting the correctness of the program. It's crucial in OO development to ensure that a subclass truly represents a subtype of the superclass, maintaining system integrity.

#### 7. What is behavioral subtyping?
   
   > **Behavioral subtyping** is a form of polymorphism where a subclass maintains the expected behavior of its superclass. It ties closely to the Liskov substitution principle.

#### 8. When is a pre-condition reasonable?
   
   > A pre-condition is reasonable when it specifies necessary and sufficient conditions for a method to execute correctly without being overly restrictive.

#### Tasks:
   
   - **Pre- and post-conditions for `top` and `isEmpty` in Stack**:
     > **top**:
     > - Pre-condition: Stack is not empty.
     > - Post-condition: Returns the top element without modifying the stack.
     > 
     > **isEmpty**:
     > - Pre-condition: None.
     > - Post-condition: Returns `true` if stack is empty, `false` otherwise.
     > 
     > If a `size` method is added:
     > - Pre-condition: None.
     > - Post-condition: Returns the number of elements in the stack.
   
   - **Design by Contract for class Rectangle**:
     > **move(dx, dy)**:
     > - Pre-condition: None.
     > - Post-condition: The rectangle's position is changed by `(dx, dy)`.
     > 
     > **resize(width, height)**:
     > - Pre-condition: `width` and `height` are positive.
     > - Post-condition: The rectangle's dimensions are updated to the new width and height.

   - **Consumer-driven contracts for a REST-API**:
     > It would involve consumers specifying their expectations and needs from an API, and these contracts being verified against the actual API to ensure compatibility.

### Summary(ii)

#### 1. Why are redundant checks not a good way to support Design by Contract?

   > Redundant checks go against the principles of Design by Contract (DbC) as they introduce unnecessary complexity and potential inconsistencies. The essence of DbC is clear delineation of responsibilities; when a contract is defined, it should be trusted. Redundant checks can:
   > - Waste computational resources.
   > - Obscure code, making maintenance more challenging.
   > - Create confusion about the true source of truth in a system.

#### 2. You’re a project manager for a weather forecasting system, where performance is a real issue. Set-up some guidelines concerning assertion monitoring and argue your choice.

   > **Guidelines for Assertion Monitoring**:
   > - **Selective Monitoring**: Given performance concerns, enable assertions only in critical paths or high-risk components.
   > - **Environment-based Activation**: Activate assertions in development and testing environments, but consider disabling them in production.
   > - **Threshold-based Monitoring**: Use assertions to monitor deviations beyond acceptable performance thresholds.
   > 
   > The rationale is to strike a balance between ensuring system correctness and optimizing performance. Monitoring only the most crucial parts ensures potential errors are caught without excessive overhead.

#### 3. If you have to buy a class from an outsourcer in India, would you prefer a strong precondition over a weak one? And what about the postcondition?

   > - **Precondition**: I would prefer a **strong precondition** as it clearly specifies the requirements the client must fulfill for the class to function correctly. This reduces ambiguity and helps ensure that the class works as expected.
   > - **Postcondition**: I would also prefer a **strong postcondition** as it guarantees specific outcomes given the preconditions are met. This gives clarity on what to expect from the class after its execution.
   
#### 4. Do you feel that design by contract yields software systems that are defect free? If you do, argue why. If you don’t, argue why it is still useful.

   > I don't believe that Design by Contract (DbC) guarantees defect-free software. However, it is still valuable because:
   > - **Clarity of Responsibilities**: DbC clearly defines expectations between modules or components, reducing integration issues.
   > - **Facilitates Testing**: Well-defined contracts provide a basis for focused and effective testing.
   > - **Documentation**: Contracts serve as in-built documentation, aiding maintenance and onboarding.
   > - **Reduces Ambiguity**: Clearly defined preconditions and postconditions reduce potential misunderstandings.
   
#### 5. How can you ensure the quality of the pre- and postconditions?

   > Ensuring the quality of pre- and postconditions involves:
   > - **Thorough Review**: Conduct peer reviews to identify potential oversights.
   > - **Test Against Contracts**: Design tests based on the contracts to verify their accuracy.
   > - **Iterative Refinement**: As the system evolves, revisit and adjust contracts accordingly.
   > - **Use Formal Methods**: Employ formal methods or tools that facilitate rigorous contract definition.
   
#### 6. Why is (consumer-driven) contract testing so relevant in the context of microservices?

   > **Consumer-driven contract testing** is crucial for microservices because:
   > - **Decoupled Development**: Allows teams to develop, test, and deploy services independently.
   > - **Ensures Compatibility**: Verifies that changes in one service don't break dependent services.
   > - **Facilitates Evolution**: Ensures that services can evolve without unexpected regressions.
   > - **Promotes Clear Communication**: Encourages clear expectations between service providers and consumers.
   
#### 7. Assume you have an existing software system and you are a software quality engineer assigned to apply design by contract. How would you start? What would you do?

   > - **Audit Existing System**: Begin by understanding the current system's components, interfaces, and dependencies.
   > - **Identify Critical Components**: Prioritize components with the most dependencies or highest risk.
   > - **Draft Initial Contracts**: Define initial preconditions, postconditions, and invariants for these components.
   > - **Review with Stakeholders**: Collaborate with developers, testers, and architects to refine contracts.
   > - **Implement Contracts**: Use contract enforcement tools or mechanisms to integrate contracts into the system.
   > - **Iterative Enhancement**: Over time, expand the coverage of contracts across the system and refine existing contracts as needed.

---

### Week 6: Testing

### Summary (i)

1. **What is (a) Testing, (b) a Testing Technique, (c) a Testing Strategy?**
   > - (a) Testing is the process of executing a program with the intent of finding errors.
   > - (b) A Testing Technique is a method or procedure used to determine how to test an application for errors systematically.
   > - (c) A Testing Strategy is a high-level approach to test planning and execution to ensure that the application meets its objectives and requirements.

2. **What is the difference between an error, a failure, and a defect?**
   > - An error is a human action that produces an incorrect result.
   > - A failure is a deviation of the software from its expected delivery or service.
   > - A defect is an imperfection or deficiency in the product that fails to meet its requirements.

3. **What is a test case? A test stub? A test driver? A test fixture?**
   > - A test case is a set of conditions under which a tester will determine whether an application or software system is working correctly.
   > - A test stub is a piece of code used to simulate the behavior of some module in controlled ways.
   > - A test driver is a program or test tool used to execute a test harness, which orchestrates the testing and collects the results.
   > - A test fixture sets up the conditions necessary for a test.

4. **What are the differences and similarities between basis path testing, condition testing, and loop testing?**
   > - Basis path testing is a white-box testing technique that involves creating test cases based on flows or paths within a module.
   > - Condition testing is focused on the boolean expression and decision points within the code.
   > - Loop testing specifically targets the validity of loop constructs within the code.
   > - They are similar in that they are all white-box testing methods, which means they require knowledge of the internal workings of the program.

5. **How many tests should you write to achieve MC/DC coverage? And multiple condition coverage?**
   > - For MC/DC (Modified Condition/Decision Coverage), you need enough tests to cover all the combinations of conditions in a decision that can independently affect the outcome of the decision.
   > - Multiple condition coverage requires a test case for all possible combinations of conditions, so the number depends on the number of conditions.

6. **Where do you situate alpha/beta testing in the four quadrants model?**
   > - Alpha and Beta testing would be situated in Quadrant 2 of the Agile Testing Quadrants, which is about testing business-facing applications where the tests are carried out by the business.

7. **What are the differences and similarities between unit testing and regression testing?**
   > - Unit testing is performed to check individual units or components of a software, whereas regression testing is performed to ensure that a recent program or code change has not adversely affected existing features.
   > - Both are systematic testing strategies and can be automated. They aim to identify defects early and ensure that the software is working as expected.

8. **How do you know when you tested enough?**
   > - This is often determined by the test coverage and the criticality of the application. Testing should cover all functional and non-functional requirements, all code paths, and user scenarios. It's also influenced by the risk assessment and when the failure rate falls below a certain threshold.

9. **What is Alpha-testing and Beta-Testing? When is it used?**
   > - Alpha testing is an internal validation effort to identify bugs before releasing the product to real users or the public. Beta testing is the next phase, where a version of the product is released to a limited audience outside of the company but not yet publicly available.
   > - These are used after rigorous in-house testing and before the final release of the software to the public.

10. **What is the difference between stress-testing and performance testing?**
    > - Stress testing involves evaluating how the system behaves under extreme conditions, such as high load or traffic, which is beyond the system's specifications.
    > - Performance testing measures the system's performance, such as response time, reliability, and resource usage under a particular workload.
