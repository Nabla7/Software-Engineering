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

## Week 5: Design by Contract

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

## Week 6: Testing

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

### Summary (ii)

1. **You’re responsible for setting up a test program. To whom will you assign the responsibility to write tests? Why?**
   > - The responsibility for writing tests is often assigned to the person or team developing the unit or feature. This is because they have the deepest understanding of the implementation and the intended behavior, which allows them to write more effective and comprehensive tests. It is also a best practice to write tests first, even before the code (Test-Driven Development), as it can lead to better-designed software.

2. **Why do we distinguish between several levels of testing in the V-model?**
   > - Different levels of testing in the V-model address different scopes and aspects of the software. For example, unit tests check individual components for correct behavior, integration tests verify that these components work together as expected, and system tests evaluate the complete and integrated software system against the specified requirements. This hierarchical approach ensures thorough testing at different stages of software development.

3. **Explain why basis path testing, condition testing, and loop testing complement each other.**
   > - These testing methods target different structural elements of the code. Basis path testing ensures that all possible paths through the code are executed. Condition testing verifies every possible outcome of boolean expressions. Loop testing focuses on the correctness of loop constructs. Together, they provide a comprehensive check of the code logic and structure.

4. **Why is mutation coverage a better criterion for assessing the strength of a test suite?**
   > - Mutation coverage measures the effectiveness of a test suite by introducing changes or mutations to the code and checking if the tests can detect them. It's considered better because it can reveal whether the tests can catch errors and not just whether they cover the code.

5. **Explain fuzzing (fuzz testing) in your own words.**
   > - Fuzz testing involves providing random, unexpected, or invalid data inputs to a software system to find vulnerabilities and errors. It's useful for discovering security flaws that might not be found through conventional testing methods.

6. **Explain what FIT tables are.**
   > - FIT tables, part of the Framework for Integrated Testing, are a way to specify and conduct acceptance tests by providing a tabular format where testers can define inputs and expected outputs in a way that can be directly executed as tests.

7. **When would you combine top-down testing with bottom-up testing? Why?**
   > - Combining top-down with bottom-up testing can leverage the strengths of both. Top-down allows for early stub testing of high-level functions, while bottom-up tests lower-level components first. Together, they ensure comprehensive coverage of the system.

8. **When would you combine black-box testing with white-box testing? Why?**
   > - Combining black-box and white-box testing allows testers to cover both functional and structural aspects of the software. Black-box testing ensures that the software meets user requirements without regard to internal workings, while white-box testing ensures that the internal operations are performed as intended.

9. **Is it worthwhile to apply white-box testing in an OO context?**
   > - While white-box testing is less relevant in object-oriented contexts due to encapsulation and abstraction, it can still provide value in testing the interactions and integrations between objects, as well as ensuring that all logic paths are tested.

10. **What makes regression testing important?**
    > - Regression testing is important because it ensures that new code changes do not adversely affect existing functionality. It's crucial for maintaining software quality over time, especially as software systems grow and evolve.

11. **Is it acceptable to deliver a system that is not 100% reliable? Why (not)?**
    > - While 100% reliability is often the goal, it may not always be feasible or cost-effective. The acceptable level of reliability depends on the risk associated with potential failures, the criticality of the system, and the impact on users.

12. **Explain the subtle difference between code coverage and test coverage.**
    > - Code coverage measures how much of the code is executed by the tests, while test coverage assesses how much of the functional requirements are verified by the tests. High code coverage doesn't guarantee that all functional scenarios are tested, whereas test coverage focuses on the breadth of testing in terms of requirements satisfaction.


## Week 7 : Formal Specification

### Summary (i) :

1. **Why is a UML class diagram a semi-formal specification?**
   - A UML class diagram is considered a semi-formal specification because it is based on a notation with precise syntax but loose semantics. This means that while the structure and relationships between elements are well-defined, the exact meaning or interpretation of these elements may not be strictly formalized.

2. **What is an automated theorem prover?**
   - An automated theorem prover is a tool that supports the process of formally verifying specifications by mathematically proving that certain conditions hold. These provers use logic and mathematical reasoning to confirm that given preconditions lead to specific postconditions, as defined in the specification.

3. **What is the distinction between “partially correct” and “totally correct”?**
   - The distinction lies in the concept of termination of a function or procedure:
     - Partially Correct: Assuming the precondition is true just before the function executes, if the function terminates, the postcondition is true. Infinite loops or raising exceptions is allowed.
     - Totally Correct: Again, assuming the precondition is true before function execution, the function is guaranteed to terminate and when it does, the postcondition is true.

4. **Give the mathematical definition for the weakest precondition of a Hoare triple {P} S {Q}**
   - The weakest precondition for a Hoare triple {P} S {Q} is defined as the least restrictive precondition that needs to hold before executing statement S to ensure that postcondition Q holds after S is executed. Mathematically, it can be denoted as `wp(S, Q)`, meaning that for all preconditions `P'` such that `{P'} S {Q}`, it follows that `P'` implies `P`.

5. **Why is it necessary to complement sequence diagrams with statecharts?**
   - Sequence diagrams and statecharts serve complementary purposes in modeling system behavior. Sequence diagrams are great for depicting interactions and message sequences between objects over time, showing how processes operate with one another. However, they do not effectively represent the different states an object can be in or the transitions between these states. Statecharts fill this gap by showing the various states of an object and how it transitions from one state to another, providing a more complete understanding of the system’s behavior.

6. **What is the notation for the start and termination state on a statechart? What is the notation for a guard expression on an event?**
   - In statecharts, the start state is often represented by a solid circle and the termination state by a circle with a solid circle inside it. Guard expressions on an event are conditions that must be true for the transition to occur and are usually written in square brackets `[ ]` following the event name.

7. **What does it mean for a statechart to be (a) consistent (b) complete and (c) unambiguous?**
   - (a) Consistent: Every state in the statechart is reachable from the initial state, and the final state is reachable from every other state.
   - (b) Complete: Every possible event/state pair has a defined transition in the statechart.
   - (c) Unambiguous: No event, including guard conditions, appears more than once in the transitions leaving any given state, ensuring deterministic behavior.

8. **How does a formal specification contribute to the correctness of a given system?**
   - Formal specifications contribute to the correctness of a system by providing a mathematically precise description of the system’s behavior and properties. This allows for rigorous verification of the system against its requirements, ensuring that it behaves as intended under all defined conditions. Formal specifications also enable the generation of test cases that cover all aspects of the system’s functionality, further ensuring its correctness.


You should be able to complete the following tasks
  - Use a theorem prover (Daphny) to prove that a given piece of code is correct. 
  - Create a statechart specification for a given problem.
  - Given a statechart specification, derive a test model using path testing.

### Summary (ii) :

1. **(Based on the article “A Formal Approach to Constructing Secure Air Vehicle Software”.)
+ What is according to you the most effective means to achieve “provably secure against cyberattacks”?**
   - Based on the article "A Formal Approach to Constructing Secure Air Vehicle Software," the most effective means to achieve software that is "provably secure against cyberattacks" involves a combination of formal methods in software development and rigorous testing. Formal methods, like formal specifications and automated theorem proving, provide a mathematically sound basis for verifying the correctness and security of software algorithms and architectures. This approach is complemented by thorough testing, including penetration testing and scenario-based testing, to ensure the software is resilient to known and emerging cyber threats.

2. **Why is it likely that you will encounter formal specifications?**
   - Formal specifications are likely to be encountered in complex, high-stakes, or safety-critical systems where precision, correctness, and reliability are paramount. Examples include aerospace, automotive, financial systems, and medical devices. The growing complexity of software and the increasing importance of cybersecurity further drive the adoption of formal specifications in these areas.

3. **Explain why we need both the loop variant and the loop invariant for proving total
correctness of a loop?**
   - For proving total correctness of a loop, both the loop invariant and loop variant are essential. The loop invariant is a condition that holds true before and after each iteration of the loop, ensuring the correctness of the loop's functionality. The loop variant, on the other hand, is a measure (usually a non-negative integer) that decreases with each iteration and ensures that the loop terminates. The combination of these two proves that the loop works correctly (invariant) and eventually terminates (variant).

4. **What do you think happened with the bug report on the broken Java.utils.Collection.sort
()? Why do you think this happened?**
   - The incident with the bug in `Java.utils.Collection.sort()` likely occurred due to an oversight in handling edge cases or incorrect assumptions in the algorithm. Such bugs often arise from complex interactions within the code or unexpected inputs that were not fully considered during development. It highlights the importance of thorough testing and the potential limitations of informal or semi-formal verification methods in capturing all possible scenarios.

5. **Explain the relationship between “Design By Contract” on the one hand “State based
specifications” on the other hand.**
   - "Design by Contract" (DbC) and state-based specifications are complementary concepts in software design. DbC focuses on the explicit specification of contractual obligations between a method and its clients (preconditions, postconditions, and invariants), thereby ensuring a clear and formal understanding of how methods should behave. State-based specifications, on the other hand, describe the allowed states of a system and the transitions between these states. They provide a high-level view of the system's behavior over time. DbC can be seen as specifying the contract at a method level, while state-based specifications provide a broader, system-level view.

6. **Explain the relationship between “Testing” on the one hand and “State based
specifications” on the other hand.**
   - Testing and state-based specifications also have a complementary relationship. State-based specifications provide a formal description of the expected states and state transitions of a system, which can be used to derive test cases. These test cases can validate whether the system correctly implements the specified states and transitions. Testing, in this context, becomes a means to empirically verify that the state-based specifications have been correctly implemented in the system.

7. **You are part of a team build a fleet management system for drones transporting medical
goods between hospitals. You must secure the system against cyber-attacks. Your boss asks you to look into formal specs; which ones would you advise and why?**
   - For securing a drone fleet management system against cyber-attacks, I would advise considering formal specifications that focus on security, reliability, and real-time requirements. Specifications like Z notation or Alloy could be used for modeling complex data and interactions, while Temporal Logic could be employed for specifying and verifying real-time constraints. Additionally, considering automated theorem provers and model checking tools would be beneficial to rigorously verify the correctness and security of the system against the specified requirements. The choice of formal specifications would be driven by the need to ensure not just functional correctness but also resilience against potential cyber threats, given the critical nature of transporting medical goods.

## Week 8 : Domain Modelling 2023 

### Summary (i) 

#### Question 1: Why is it necessary to validate and analyze the requirements?
**Answer:** 
- **Validation of requirements** ensures that the system being developed aligns with the actual needs and expectations of the stakeholders, answering the question: "Are we building the right system?"
- **Analysis of requirements** helps in understanding the problem correctly and ensuring the problem domain is adequately modeled, addressing the question: "Did we understand the problem correctly?"

#### Question 2: What’s the decomposition principle for functional and object-oriented decomposition?
**Answer:** 
- **Functional Decomposition:** Breaks down a complex process or system into simpler, manageable sub-processes or functions.
- **Object-Oriented Decomposition:** Involves breaking down a system based on the objects in the system, focusing on their attributes and behaviors.

#### Question 3: Can you give the advantages and disadvantages for functional decomposition? What about object-oriented decomposition?
**Answer:** 
- **Functional Decomposition:**
  - **Advantages:** Good for stable requirements, clear problem decomposition.
  - **Disadvantages:** Limited in handling evolving systems, can lead to maintenance issues.
- **Object-Oriented Decomposition:**
  - **Advantages:** Better for complex and evolving systems, encapsulation offers robustness.
  - **Disadvantages:** Not explicitly mentioned, but can imply complexity in understanding and implementing.

#### Question 4: How can you recognize “god classes”?
**Answer:** 
- **God Classes** can be recognized by their characteristics:
  - Large classes doing most of the work.
  - Having numerous responsibilities.
  - Often having a suffix like “System,” “Manager,” “Controller.”

#### Question 5: What is a responsibility? What is a collaboration?
**Answer:** 
- **Responsibility:** Refers to the services or functions an object provides in a system, including the knowledge it maintains and actions it performs.
- **Collaboration:** Involves interactions between objects to fulfill their responsibilities.

#### Question 6: Name 3 techniques to identify responsibilities.
**Answer:** 
1. **Scenarios and Role Play:** Using scenario walk-throughs where different roles are acted out.
2. **Verb Phrase Identification:** Identifying candidate responsibilities from verb phrases in requirements.
3. **Class Enumeration:** Listing all candidate classes and assigning initial responsibilities.

#### Question 7: What do feature models define?
**Answer:** 
- **Feature Models:** Define a set of reusable and configurable requirements for systems in a domain. They focus on commonalities and variations among the members of a software product line.

#### Question 8: Give two advantages and disadvantages of a “clone and own” approach.
**Answer:** 
- **Advantages:** 
  1. Efficiency - Saves time and reduces costs.
  2. Independence and immediate availability.
- **Disadvantages:** 
  1. Overhead - Difficulty in propagating changes and adapting clones.
  2. Governance issues - Lack of reuse tracking and organizational processes.

#### Question 9: Explain the main difference between a social fork and a variant fork.
**Answer:** 
- **Social Fork:** Involves temporary branching for specific modifications with the intention of merging back into the main branch.
- **Variant Fork:** Represents a separate, maintained variant of the project, not intended for merging back.

#### Question 10: How does domain modeling help to achieve correctness? Traceability?
**Answer:** 
- **Correctness:** By focusing on modeling the problem domain accurately from the customer's perspective and specifying "what" rather than "how."
- **Traceability:** Through proper naming conventions and modeling, linking requirements directly to system elements like classes and operations.

### Summary (ii)

#### Question 1: How does domain modeling help to validate and analyze the requirements?
**Answer:**
- Domain modeling helps validate and analyze requirements by ensuring that the system reflects the real-world aspects it is supposed to model. It focuses on the 'what' (goals) rather than the 'how' (procedures), enabling an accurate representation of the problem domain and ensuring that the system meets its intended purpose.

#### Question 2: What’s the problem with “god classes”?
**Answer:**
- "God classes" are problematic because they centralize too many responsibilities, leading to maintenance difficulties, reduced modularity, and decreased flexibility in the system. They are typically large, complex, and difficult to manage, making them prone to errors and challenging to adapt to changing requirements.

#### Question 3: Why are many responsibilities, many collaborators, and deep inheritance hierarchies suspicious?
**Answer:**
- Having many responsibilities in a class, numerous collaborators, and deep inheritance hierarchies are suspicious because they often indicate poor design. Such structures can lead to complex, tightly-coupled systems that are hard to maintain, understand, and extend. They can also hinder code reuse and make the system less adaptable to changes.

#### Question 4: Can you explain how role-playing works? Do you think it helps in creative thinking?
**Answer:**
- Role-playing in domain modeling involves stakeholders and developers acting out scenarios to understand and validate system requirements and behaviors. It helps in creative thinking by allowing participants to explore different perspectives, identify potential issues, and brainstorm solutions in a collaborative and interactive way.

#### Question 5: Can you compare Use Cases and CRC Cards in terms of the requirements specification process?
**Answer:**
- Use Cases and CRC Cards are both used in the requirements specification process but in different ways. Use Cases focus on describing the interactions between users and the system, outlining the steps to accomplish specific goals. CRC Cards, on the other hand, focus on identifying and organizing the responsibilities of different classes in the system and their collaborations. They complement each other, with Use Cases highlighting user interactions and CRC Cards focusing on system structure and behavior.

#### Question 6: Do CRC cards yield the best possible class design? Why not?
**Answer:**
- CRC cards do not necessarily yield the best possible class design but are a valuable tool in the design process. They help in identifying and organizing class responsibilities and collaborations, but the effectiveness of the final design also depends on other factors like the complexity of the problem, the skill of the designers, and the evolving nature of requirements.

#### Question 7: Why are CRC cards maintained with paper and pencil instead of electronically?
**Answer:**
- CRC cards are often maintained with paper and pencil because this approach facilitates easy modification, reorganization, and collaboration during brainstorming and design sessions. The tangible nature of paper cards allows for a more flexible and interactive design process, encouraging creativity and team involvement.

#### Question 8: What would be the main benefits for thinking in terms of “system families” instead of “one-of-a-kind development”? What would be the main disadvantages?
**Answer:**
- **Benefits of thinking in terms of “system families”:**
  - Encourages reuse of components and features across similar systems.
  - Facilitates more efficient and consistent development for similar products.
  - Promotes scalability and adaptability within a product line.
- **Main disadvantages:**
  - Increased initial complexity in setting up a product line.
  - Potential for feature bloat or unnecessary complexity in individual systems.
  - Challenges in maintaining consistency and compatibility across the product family.

#### Question 9: Can you apply scrum to develop a product line? Argue your case.
**Answer:**
- Scrum can be applied to develop a product line as it provides a flexible and iterative approach, which is beneficial for handling the complex and evolving nature of product lines. Scrum's focus on regular feedback, adaptability, and iterative development aligns well with the needs of product line development. However, challenges may include managing the scope of work across the product line and ensuring coherence and compatibility among different products within the line.

## Week 8 : Software Quality

### Summary (i) 

### Answers to Summary (i) Questions

#### 1. Why is software quality more important than it was a decade ago?
   - **Answer**: Software quality has become increasingly important due to several factors including the ubiquitous nature of software in modern life, the complexity of contemporary software systems, the critical role software plays in safety and security, and the economic impact of software failures. The reliance on software for essential functions in business, healthcare, transportation, and communication means that software quality directly impacts functionality, user satisfaction, and safety.

#### 2. Can a correctly functioning piece of software still have poor quality? Why?
   - **Answer**: Yes, a software can function correctly and still have poor quality. This is because software quality encompasses more than just functional correctness. It includes aspects like usability, maintainability, performance, reliability, and security. A software may meet its functional requirements but may be difficult to use, maintain, or scale, may perform poorly, or may have security vulnerabilities, all of which contribute to poor overall quality.

#### 3. If quality control can’t guarantee results why do we bother?
   - **Answer**: Quality control is important even if it can't guarantee perfect results because it significantly reduces the likelihood of defects, improves the overall quality of the product, and helps in identifying and fixing issues early in the development process. This prevention and early detection reduce costs, improve customer satisfaction, and enhance the reputation of the organization.

#### 4. What’s the difference between an external and an internal quality attribute? And between a product and a process attribute?
   - **Answer**: 
     - **External vs. Internal Quality Attributes**: External quality attributes are those that are visible to the user, like usability, reliability, and performance. Internal quality attributes, on the other hand, are inherent to the software system and not directly visible to the user, such as modularity, readability, and testability.
     - **Product vs. Process Attribute**: Product attributes are characteristics that relate to the software product itself, like functionality, reliability, and usability. Process attributes pertain to the process used to develop the software, like efficiency, documentation quality, and compliance with standards.

#### 5. What’s the distinction between correctness, reliability, and robustness?
   - **Answer**: 
     - **Correctness** refers to the software’s ability to perform its intended functions accurately as per the specifications.
     - **Reliability** is the measure of the software's ability to function under predetermined conditions for a specified period.
     - **Robustness** is the ability of the software to handle errors or unexpected inputs gracefully and maintain stable operation.

#### 6. How can you express the “user friendliness” of a system?
   - **Answer**: User friendliness of a system can be expressed in terms of its usability. This includes the system's ease of use, intuitiveness, consistency in design, clarity of user interface, availability of help and documentation, and the system’s ability to cater to the needs of its intended users efficiently and effectively.

#### 7. Can you name three distinct refinements of “maintainability”? What do each of these names mean?
   - **Answer**: 
     - **Repairability**: The ease with which defects or issues in the software can be fixed.
     - **Adaptability (Evolvability)**: The ability of the software to evolve and adapt to changing requirements or environments.
     - **Portability**: The ease with which the software can be transferred from one environment or system to another.

#### 8. What is meant with “short time to market”? Can you name 3 related quality attributes and provide definitions for each of them?
   - **Answer**: "Short time to market" refers to the ability to develop and release software products quickly to meet market demands or take advantage of market opportunities. Three related quality attributes are:
     - **Productivity**: The efficiency with which software is produced.
     - **Timeliness**: The ability to deliver software on or before the agreed deadline.
     - **Visibility**: The transparency and accessibility of the software development process to stakeholders.

#### 9. Name four things which should be recorded in the review minutes.
   - **Answer**:
     - What was reviewed.
     - Who reviewed it.
     - The findings and conclusions of the review.
     - Decisions made during the review, such as acceptance, provisional acceptance, or rejection of the reviewed item.

#### 10. Explain briefly the three items that should be included in a quality plan.
   - **Answer**:
     - Desired product qualities and methods for their assessment.
     - Significant quality attributes specific to the project.
     - The quality assessment process, including standards to be applied and quality review methods.

#### 11. What’s the relationship between ISO9001, CMMI standards, and an organization’s quality system? How do you get certified?
   - **Answer**: ISO9001 and CMMI standards provide frameworks for quality management and process improvement. They guide organizations

 in establishing a quality system that ensures consistent quality and continuous improvement. To get certified, an organization must implement these standards and then undergo an external audit by a certified body to verify compliance.

#### 12. Can you name and define the 5 levels of CMMI?
   - **Answer**: 
     - **Level 1 - Initial**: Processes are ad hoc and chaotic. Success depends on individual effort.
     - **Level 2 - Managed**: Processes are planned and executed in accordance with policy; there are basic project management processes.
     - **Level 3 - Defined**: Processes are well characterized and understood, and are described in standards, procedures, tools, and methods.
     - **Level 4 - Quantitatively Managed**: Processes are controlled using statistical and other quantitative techniques.
     - **Level 5 - Optimizing**: Focus on continuous process improvement, enabled by quantitative feedback and from piloting innovative ideas and technologies.

#### 13. Where would “use-cases” as defined in chapter 3 fit in the table of core process areas (p. 32)? Motivate your answer shortly.
   - **Answer**: Use-cases would fit under "Requirements Management" in the table of core process areas. They are instrumental in defining and managing the requirements of a project, providing a clear and detailed description of how users will interact with the system and the expected outcomes of these interactions.

### Summary (ii)

### Answers to Summary (ii) Questions

#### 1. Given a piece of code and a coding standard, review the code to verify whether the standard has been adhered to.
   - **Task Description**: This task involves a meticulous examination of the provided code against the specified coding standard. The review process should focus on assessing adherence to coding conventions, including naming standards, commenting practices, code structure, and any specific programming practices outlined in the standard.

#### 2. Given the Quality Attributes Overview table, argue why the crosses and blanks occur at the given positions.
   - **Answer**: The crosses and blanks in the Quality Attributes Overview table represent the presence or absence of specific quality attributes in different contexts. Crosses indicate where a particular quality attribute is relevant or applicable, while blanks signify its irrelevance or non-applicability in that context. The placement of crosses and blanks reflects the specific characteristics and requirements of the software system and the project environment.

#### 3. Why do quality standards focus on process and internal attributes instead of the desired external product attributes?
   - **Answer**: Quality standards focus on process and internal attributes because these are foundational to achieving desired external product attributes. A well-defined and controlled process ensures consistent quality and efficiency in development. Internal attributes like code maintainability, modularity, and readability are crucial for long-term product stability and scalability. By emphasizing these aspects, quality standards aim to create a solid foundation that naturally leads to high-quality external product attributes.

#### 4. Why do you need a quality plan? Which topics should be covered in such a plan?
   - **Answer**: A quality plan is necessary to define and guide the quality assurance and control processes within a project. It should cover topics such as the desired quality attributes of the product, significant quality metrics, the standards and methodologies to be used for quality assurance, roles and responsibilities for quality management, and procedures for monitoring and improving quality throughout the project lifecycle.

#### 5. How should you organize and run a review meeting?
   - **Answer**: A review meeting should be organized with a clear agenda, objectives, and a defined participant list. The meeting should be time-bound, with sufficient preparation by all participants. A moderator should guide the meeting, ensuring adherence to the agenda and facilitating discussions. Key points, decisions, and action items should be documented in the review minutes.

#### 6. Why are coding standards important?
   - **Answer**: Coding standards are important as they ensure consistency, readability, and maintainability of code. They facilitate collaboration among developers, make the codebase more understandable and navigable, and help in identifying issues more easily. Adhering to coding standards also improves the overall quality and reliability of the software.

#### 7. What would you include in a documentation review checklist?
   - **Answer**: A documentation review checklist should include items such as completeness and accuracy of information, clarity and readability, consistency in format and terminology, adherence to documentation standards, correctness of technical details, and up-to-date references and links.

#### 8. How often should reviews be scheduled?
   - **Answer**: The frequency of reviews should be based on the complexity and duration of the project, criticality of the components being developed, and the stage of the project lifecycle. Regular reviews are crucial for early detection of issues and ensuring alignment with project goals.

#### 9. Could you create a review checklist for ATAM (Architecture Tradeoff Analysis Method)?
   - **Answer**: Creating a review checklist for ATAM involves identifying key architectural decisions, assessing trade-offs between competing quality attributes, evaluating risk and sensitivity points, and ensuring alignment with business goals. The checklist would include items specific to architectural approaches, scalability, performance, security, maintainability, and stakeholder priorities.

#### 10. Would you trust software from an ISO 9000 certified company? And if it were CMMI?
   - **Answer**: Trust in software from an ISO 9000 or CMMI certified company would be higher as these certifications indicate a commitment to quality management and process improvement. However, it's important to note that these certifications focus more on processes than the final product quality, so a holistic evaluation including product performance and user feedback would be advisable.

#### 11. You are supposed to develop a quality system for your organization. What would you include?
   - **Answer**: Developing a quality system would involve establishing quality policies, objectives, processes, and metrics. It should include procedures for quality control and assurance, standards for software development and documentation, training programs for staff, mechanisms for continuous improvement, and methods for monitoring and measuring quality performance.

#### 12. Where would “testing” fit in the table of core process areas (p. 32). Does it cover a single row or not? Argue why (not)?
   - **Answer**: Testing would fit into multiple rows in the table of core process areas as it is a cross-cutting activity impacting various stages of software development. It is integral to validating the functionality (correctness, reliability, performance, etc.) of software, ensuring that the product meets its specifications and user needs. Testing intersects with requirements management, design, development, and maintenance, reflecting its pervasive role in software quality assurance.

## Week 9 : Metrics

### Summary (i) 

### Answers to Summary (i) Questions

#### 1. Can you give three possible problems of metrics usage in software engineering? How does the measurement theory address them?
   - **Answer**: 
     - **Problem 1**: Misinterpretation or misuse of metrics, leading to incorrect conclusions.
     - **Problem 2**: Overreliance on metrics, neglecting qualitative aspects.
     - **Problem 3**: Using inappropriate metrics for a given context or goal.
     - **Measurement Theory Address**: It provides a framework for understanding and interpreting metrics correctly, ensuring they are used appropriately and effectively in different contexts.

#### 2. What’s the distinction between a measure and a metric?
   - **Answer**: A measure is a quantification of an attribute (like lines of code), whereas a metric is a standard of measurement that combines multiple measures and adheres to certain mathematical properties. Metrics are often more complex and are used to assess or compare attributes.

#### 3. Can you give an example of a direct and an indirect measure?
   - **Answer**: 
     - **Direct Measure**: Lines of Code (LOC), which directly measures the length of source code.
     - **Indirect Measure**: Code Complexity, which is calculated based on multiple direct measures such as the number of decision points.

#### 4. What kind of measurement scale would you need to say “A specification error is worse than a design error”? And what if we want to say “A specification error is twice as bad as a design error?”
   - **Answer**: 
     - To say “A specification error is worse than a design error,” an ordinal scale is needed, which allows for ranking or ordering of items.
     - To claim “A specification error is twice as bad as a design error,” a ratio scale is required, as it allows for expressing the magnitude of difference.

#### 5. Explain the need for a calibration factor in Putnam’s model.
   - **Answer**: The calibration factor in Putnam’s model adjusts the model to fit the specific context and characteristics of a project. It accounts for variations in team productivity, project complexity, and other environmental factors, thereby enhancing the accuracy of effort and time estimation.

#### 6. Fill in the blanks in the following sentence. Explain briefly based on the Putnam’s model: “If you want to finish earlier (= decrease scheduled time) you should ... the effort ... .”
   - **Answer**: “If you want to finish earlier (= decrease scheduled time) you should increase the effort significantly.” In Putnam’s model, the relationship between time and effort is non-linear; reducing time increases the required effort disproportionately.

#### 7. Give three metrics for measuring size of a software product.
   - **Answer**: 
     - Lines of Code (LOC)
     - Function Points (FP)
     - Use Case Points (UCP)

#### 8. Discuss the main advantages and disadvantages of Function Points.
   - **Answer**: 
     - **Advantages**: Independent of programming language; focuses on functionality, which is relevant to clients; can be used early in the development cycle.
     - **Disadvantages**: Requires expert judgment and can be subjective; not automatically calculable; may not be as effective for non-data processing applications.

#### 9. What does it mean for a coupling metric not to satisfy the representation condition?
   - **Answer**: If a coupling metric does not satisfy the representation condition, it means the metric does not accurately represent the concept it is intended to measure. For example, a high coupling metric might not necessarily indicate poor design if the coupling is essential for functionality.

#### 10. Can you give 3 examples of impreciseness in Lines of Code measurements?
   - **Answer**: 
     - **Example 1**: Variations in coding styles can lead to different LOC for the same functionality.
     - **Example 2**: LOC does not account for the complexity or quality of the code.
     - **Example 3**: LOC is language-dependent; more verbose languages will naturally have higher LOC for the same functionality.

### Answers to Summary (ii) Questions

#### 1. During which phases in a software project would you use metrics?
   - **Answer**: Metrics can be used in various phases of a software project, including:
     - **Requirements Phase**: for estimating size and complexity of the project.
     - **Design and Development Phase**: for tracking progress, code quality, and adherence to standards.
     - **Testing Phase**: for measuring defect density and identifying areas needing improvement.
     - **Maintenance Phase**: for assessing the impact of changes and the maintainability of the software.

#### 2. Why is it so important to have “good” product size metrics?
   - **Answer**: Good product size metrics are crucial as they provide a basis for estimating effort, cost, and time requirements, help in tracking and improving productivity, and facilitate better project planning and resource allocation.

#### 3. Can you explain the two levels of calibration in COCOMO (i.e., C & S vs. M)? How can you derive actual values for these parameters?
   - **Answer**: COCOMO involves two levels of calibration:
     - **C & S**: These are project-independent parameters determined through regression analysis of historical project data, reflecting typical project characteristics.
     - **M**: This is the project-specific calibration factor adjusted for each project based on its specific attributes and constraints.
     - To derive actual values, analyze past project data or industry benchmarks and adjust based on specific project factors.

#### 4. Can you motivate why in software engineering productivity depends on the scheduled time? Do you have an explanation for it?
   - **Answer**: In software engineering, productivity depends on scheduled time due to the non-linear relationship between time and effort. Reducing time increases the required effort disproportionately, impacting productivity. This relationship is explained by models like Putnam’s model.

#### 5. Can you explain the cone of uncertainty? And why is it so relevant to cost estimation in software projects?
   - **Answer**: The cone of uncertainty represents the evolution of uncertainty in a project. It decreases as the project progresses and more information becomes available. It's relevant for cost estimation as it illustrates the risks and uncertainties involved in early estimates, guiding more accurate forecasting as the project advances.

#### 6. How can you decrease the uncertainty of a project bid using Putnam’s model?
   - **Answer**: To decrease the uncertainty in a project bid using Putnam’s model, one should gather as much detailed and accurate information as possible about the project's scope, complexity, and constraints. Adjusting the calibration factor based on this information can lead to more accurate estimates.

#### 7. Why do we prefer measuring Internal Product Attributes instead of External Product Attributes during Quality Control? What is the main disadvantage of doing that?
   - **Answer**: Internal Product Attributes are preferred during Quality Control because they are directly controllable and measurable by the development team. However, the main disadvantage is that they may not fully represent the user perspective or the external quality experienced by users.

#### 8. You are a project manager and you want to convince your project team to apply algorithmic cost modeling. How would you explain the technique?
   - **Answer**: Algorithmic cost modeling uses mathematical models to estimate project costs based on various project factors like size, complexity, team skill, and technology. It provides a systematic, data-driven approach for effort and cost estimation, allowing for more accurate planning and budgeting.

#### 9. Where would you fit coupling/cohesion metrics in a hierarchical quality model like ISO 9126?
   - **Answer**: In the ISO 9126 hierarchical quality model, coupling/cohesion metrics would fit under the 'Maintainability' characteristic. These metrics assess the interdependence of modules (coupling) and the unity of operations within a module (cohesion), which are crucial for maintainability.

#### 10. Why are coupling/cohesion metrics important? Why then are they so rarely used?
   - **Answer**: Coupling/cohesion metrics are important as they give insight into the software structure, affecting maintainability and flexibility. However, they are rarely used due to their complexity in measurement and interpretation, and the difficulty in defining universal standards applicable across different projects.

#### 11. Do you believe that “defect density” says something about the correctness of a program? Motivate your answer.
   - **Answer**: Defect density does provide some indication of a program's correctness, as it measures the number of defects relative to the size of the software. A higher defect density may suggest lower correctness. However, it should be interpreted cautiously, as it depends on the thoroughness of testing and defect discovery processes.

### Probable Answers to Given Tasks

#### Task 1 : Two classes A & B have a common parent class X. Class A defines a method a() and class B a method b() and there is a large portion of duplicated code between the two methods. Give a sequence of refactorings that moves the duplicated code in a separate method x() defined on the common superclass X.

1. **Identify and Extract Duplicated Code**:
   - Review the methods `a()` in class A and `b()` in class B to identify the duplicated code.

2. **Create a New Method in Class X**:
   - Create a new method `x()` in the common parent class X.

3. **Move Duplicated Code to the New Method**:
   - Move the duplicated code from both `a()` and `b()` into `x()`.

4. **Replace Duplicated Code with Method Call**:
   - Replace the original duplicated code in `a()` and `b()` with a call to the new method `x()`.

5. **Test the Changes**:
   - Test classes A and B to ensure that they still function correctly after the refactoring.

#### Task 2: What would you do in the above situation if the duplicated code in the methods a() and b() are the same except for the name and type of a third object which they delegate responsibilities too?

1. **Identify the Variation**:
   - Identify the differing object names and types in the duplicated code within methods `a()` and `b()`.

2. **Create an Abstract Method in Class X**:
   - Define an abstract method in class X, say `delegateMethod()`, that handles the varying part.

3. **Implement the Abstract Method in A & B**:
   - Implement `delegateMethod()` in both classes A and B, each handling the object specific to their method (`a()` or `b()`).

4. **Refactor Methods a() and b()**:
   - Extract the common duplicated code into a new method `x()` in class X, replacing the varying parts with calls to `delegateMethod()`.

5. **Replace Duplicated Code in a() and b()**:
   - Replace the original duplicated code in `a()` and `b()` with calls to `x()`.

6. **Test the Changes**:
   - Test classes A and B to ensure the refactoring has not altered the intended behavior of methods `a()` and `b()`.

These steps would allow the duplicated code to be centralized in the superclass while handling variations through polymorphic methods in the subclasses.
