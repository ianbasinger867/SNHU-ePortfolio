# SNHU-ePortfolio
SNHU ePortfolio


# Self Assessment
Throughout the development and enhancement of my ePortfolio artifacts, I have demonstrated growth across multiple domains of computer science, including software engineering, algorithms, database design, and system-level thinking. Each milestone reflects not only technical skill development but also increasing confidence in evaluating and improving existing systems.

The Mobile Weight Tracking Application evolved from a functional academic assignment into a more refined, production style software solution. Enhancement One strengthened my understanding of modular architecture, maintainability, and separation of concerns. Enhancement Two expanded the system with algorithmic intelligence, integrating statistical techniques such as moving averages, exponential smoothing, and regression into a mobile application environment. Enhancement Three refined database performance, indexing strategy, and schema evolution, reinforcing the importance of long-term scalability and data integrity.

Across these enhancements, I demonstrated the ability to:

Apply algorithmic principles within real-world constraints

Select appropriate data structures and optimize for performance

Refactor and improve legacy code without breaking functionality

Design database schemas that balance efficiency and maintainability

Make informed trade-offs between computation in application logic and SQL

Maintain data privacy and integrity in a user-facing system

One of the most significant areas of growth for me was learning to work within constraints rather than redesigning systems from scratch. Real-world software development often requires adapting to existing architecture, preserving user data, and incrementally improving performance. These enhancements reflect my ability to operate within those constraints while still delivering meaningful improvements.

# Enhancement One
The artifact selected for this milestone is my Mobile Weight Tracking Application originally developed in CS 360. This application allows users to log daily weight entries, view trends, and manage historical records using a local database. It was originally created as part of a mobile application development project focused on Android Studio, Java, and SQLite integration.

 I selected this artifact because it demonstrates a complete, real world software solution that incorporates UI design, database integration, and business logic. For this enhancement, I improved the code structure by refactoring activities into clearer components, improving data validation, and enhancing UI responsiveness. These changes showcase the ability to apply software engineering to best practices such as modular design, separation of concerns, and maintainability.

 The enhancements directly support the course of outcomes related to designing and implementing computing solutions using appropriate practices and tools. I also strengthened outcome coverage related to delivering professional quality software and applying software engineering techniques. Compared to my original plan in Module One, I expanded my focus to include better user experience design and code readability, not just functional improvements.
 
 Enhancing this artifact helped me better understand how small design decisions affect scalability and long-term maintainability. One challenge was restructuring the data handling logic without breaking existing functionality, which required careful testing and iterative refactoring. Through this process, I gained confidence in modifying and improving existing codebases, a skill that is critical in development.

# Enhancement Two

For milestone three, this artifact was enhanced by introducing trend analysis and a forecasting module that performs incremental algorithmic computation on historical weight data. This was implemented using Java and integrated directly into the dashboard workflow.
Including this artifact in the ePortfolio is important because it demonstrates the application of core data structures and algorithmic principles within a realistic, user-facing application. Unlike isolated academic exercises, this weight tracker application operates on persisted, user-generated data and must have correctness, efficiency, and integration with existing architecture.
The enhancement showcases skills in data structure selection, using the fixed-size ring buffer, algorithm design by moving averages, exponential smoothing and linear regression, along with performance optimization via incremental computation versus full recompilation, and finally adapting an algorithm to a legacy data model.
This artifact was improved by extending beyond basic data storage and display into a system capable of continuous analytical computation, including a 7-day moving average using a running sum for O(1) updates, an exponential moving average to weigh recent entries more heavily, a linear regression over a sliding window to estimate weight trends, and forecasting logic to estimate time-to-goal based on observed slope. These enhancements transform the application from a simple tracker into an analytical tool.

## Course Outcome Alignment
This enhancement meets the planned course outcomes, particularly:

Design and evaluate computing solutions using algorithmic principles and computer science practices while managing trade-offs

The enhancement required selecting appropriate algorithms and data structures while considering time complexity, memory usage, and mobile performance constraints. Incremental updates were chosen over repeated full-dataset computation to reduce computational overhead.

Demonstrate the ability to use well-founded and innovative techniques, skills, and tools in computing practices

The implementation applies established statistical techniques (moving averages, exponential smoothing, regression) within a mobile application context, demonstrating the ability to translate mathematical concepts into working software logic.

## Reflection on Enhancement Process
Enhancing this artifact reinforced the importance of adapting algorithmic solutions to existing system constraints, rather than redesigning core components unnecessarily. One challenge I encountered was integrating new analytical logic with an immutable data model where weight values are stored as strings and domain objects required specific constructors. Rather than refactoring the data model, the enhancement was designed to parse and process values safely while preserving compatibility with the existing architecture.
By implementing a ring buffer with a running sum, the system avoids repeated re computation of averages, showing to me how small design decisions can significantly affect performance and scalability. I tested the enhancement through Logcat output to validate correctness of moving averages, exponential smoothing, trend slopes, and forecast estimates using real application data.

# Enhancement Three

For milestone four, the artifact was enhanced by refining the database layer to support performance optimization, analytical queries, safe schema evolution, all while preserving the existing SQLite architecture and user data.
This artifact was selected for inclusion in the ePortfolio because it demonstrates applied database design and skills within a realistic, production style application. Rather than focusing on database theory by itself, the Weight Tracker integrates query design, persistence, and performance considerations in a mobile environment where privacy, efficiency, and data integrity are important.
The database enhancement proves skills in:

Schema refinement and indexing
SQL aggregation and analytical query design
Migration and versioned schema upgrades
Balancing application logic vs database computation
    
The artifact improved by moving beyond simple CRUD operations to support analytics ready data access. Indexes were added to frequently queried columns to improve query performance, and new analytical SQL queries were introduced to compute weekly averages, minimum and maximum weights, and goal progress snapshots directly within the database. These enhancements reduce redundant application computation and enable more scalable data analysis as the dataset may grow.

## Course Outcome Alignment
The database enhancement meets course outcomes identified in Module One. It demonstrates progress toward:

Design and evaluate computing solutions while managing trade-offs

Design decisions were made to move aggregation and summary logic into SQL rather than recomputing values repeatedly in application code. This reflects an understanding of performance trade-offs between storage, computation, and maintainability.
well-founded techniques, skills, and tools to implement computing solutions

The enhancement applies standard database practices such as indexing, aggregation functions, and versioned upgrades to deliver measurable performance and analytical improvements without altering application behavior.
Develop a security and privacy mindset

All data remains stored locally on the device; schema changes preserve existing user data, and analytical queries operate only on the minimum required fields. This ensures that health-adjacent data is handled responsibly and securely.


## Reflection
Enhancing the database layer reinforced the importance of designing databases not only to store data, but also to support efficient analysis and future growth. One key learning outcome was recognizing when computation should occur in SQL versus application code. By shifting aggregation logic into database queries, the application becomes more efficient and easier to maintain overall.
A challenge for me was implementing schema improvements without disrupting existing users or data. This required some careful use of database versioning and upgrade logic to ensure that indexes could be added safely without requiring destructive migrations. Working within these constraints I feel closely mirrored real world scenarios where databases must evolve incrementally rather than being rebuilt from scratch.
Overall, this milestone strengthened understanding of how thoughtful database design contributes directly to application performance, scalability, and reliability, and how even small schema refinements can significantly improve the quality of a software system.



