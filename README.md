# exam_microservices

Part 2: Microservices Architecture
Answer the following questions with your own words.
Write your answers to a Markdown file, and add it to the same git project.


• Q1: Define what is a Microservices architecture and how does it differ
from a Monolithic application.

A microservices architecture is when all modules have their own process.
In comparaison, for a monolith architecture is when there is a same process for all modules.
The microservices architecture is more complex but you have more control on our application.

---------------------------------------------------------------------------------

• Q2: Compare Microservices and Monolithic architectures by listing their
respective pros and cons.

Pros for microservices:
    - Graceful degradation
    - Deployed independently

Cons for microservices:
    - Complex
    - Higher chance failure (network)
    - Eventual consitency
    - Operational complexity

Pros for monolith:
    - Simple
    - Consitency

Cons for monolith:
    - Deployed one
    - The app will go down if something is wrong

---------------------------------------------------------------------------------

• Q3: In a Microservices architecture, explain how should the application be
split and why.


The application should be split according the teams working on it. 
The application has to be divided depending fonctionnalities and not technologies (langages used)
This is the communication of the team which defines the architecture of the application.


---------------------------------------------------------------------------------

• Q4: Briefly explain the CAP theorem and its relevance to distributed
systems and Microservices.

This theorem try to prove that in a distributed system, Consistency, Availability, and Partition Tolerance cannot all be achieved at the same time. 
You have to "sacrifice" one of them to have two together.
Plus, with microservices, the CAP theorem seems to pose a unsolvable problem.

Mostly in microservices architectures choose Partition Tolerance with High Availability and follow Eventual Consistency for data consistency.


---------------------------------------------------------------------------------

• Q5: What consequences on the architecture ?

In microservices architecture, you have to choose carefully between the three factors.

---------------------------------------------------------------------------------

• Q6: Provide an example of how microservices can enhance scalability in
a cloud environment.

In a cloud-based e-commerce microservices setup, consider the payment processing microservice. During a sale event, it can scale independently to handle a surge in transaction volume, ensuring efficient payment processing without affecting other services. This independent scalability allows for resource optimization, fault isolation, and improved performance during high-demand periods, contributing to an overall responsive and resilient system.


---------------------------------------------------------------------------------

• Q7: What is statelessness and why is it important in microservices archi-
tecture ?


Statelessness is crucial in microservices architecture because it enhances scalability, fault tolerance, and flexibility. By avoiding the storage of state information, microservices can be easily scaled, deployed, and updated, contributing to a more resilient and agile system.


---------------------------------------------------------------------------------

• Q8: What purposes does an API Gateway serve ?

 An API Gateway is one entity where you concentrate all your APIs, all the traffic goes through your API Gateway. It is one way to orchestrate microservices (there are also using a directory and using the service-mesh)