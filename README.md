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

