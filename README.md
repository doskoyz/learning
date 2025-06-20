# learning as a software engineer for 10 years
Hello, my name is Dios. I've been working as a software engineer for 10 years. Here is a summary of my experiences and challenges: 
  * Binus University (Education, Platform) (3 years)
    * Research Team
      Challenges: How do we face the new technology and think about how it can help us?
    * Binusmaya Team:
      Challenges: How to match the lecturer's schedule with the students' and manage class absences until the lecturer receives an honorarium.
  * Traveloka (Travel Platform) (2.5 years)
    * Bus and Train Team:
      Challenges: How to maintain the stability of the system, even though the provider is not stable?
  * Gudangada (Commerce Platform) (2.5 years)
    * Payment & Finance Team: How to manage the payment in/out with precision and create the journal for each detailed transaction?
  * Blibli (Commerce Platform) (2+ years)
    * Return Team: How to manage the flow that has so many dependencies (order, finance, logistics, insurance, etc)?

There are so many challenges that I have faced in 10 years, and I want to share my experience so that you can learn.
## Programming Language/Tools
* I code with different programming languages at each company, focusing on the principles of programming languages, not the language itself (When I used Java 21, it was so different with the java7), so there is no point in thinking about the syntax and framework. Better try to think about how this language works, like the memory management (garbage collector), thread management, observability, etc.
* When I interview a candidate, I always ask, What is your experience? The majority of junior candidates tell me the tools that they used before, and then when I ask the reason why they chose that, some of them said it is a legacy from the company. They focus on the reason why they use the tools, not the problem that the tools can solve the problem, and their company chooses the tools. From my perspective, it is better to know what the problem is that we need to solve than we decide the tools to solve the problem, because the tools always evolve. So it is the fundamental thinking when we need to migrate to a new tool or just use the old tool, even though it is already old.
## Prioritization
<img src="https://github.com/user-attachments/assets/82b8e86a-32f6-45f7-a491-17b085c85578" width="300" height="200" />
* I love to share the Eisenhower matrix, because in reality, we often face the issue of deciding urgent and non-urgent. From my perspective, it is easier to decide what is important and non-important instead of deciding what is urgent and non-urgent. Based on my experience, we are sorting the urgent ones in the backlog and hope no re-prioritization that pending for the important non-urgent. So, this is crucial that we *must* set the real timeline to schedule the important non-urgent and put a hard rule not to reschedule the timeline. The real case: we need to refactor the flow, the result of some of the API is unused. From my perspective, the unused API/flow is important to delete. Why? Because when we don't delete it, we need to maintain it. Based on APOSD: "the more information a developer needs to have, the harder it will be for them to work on the system". So it is important to remove the unused information/context before it is bloated in the future.
## Naming Convention
* Some people think naming is not important. Imagine we have a super big warehouse, and we just put the index name of the block as initial names A,B,X,Z. The operator should know where the item is in what block. After that, imagine if there is a new operator or if there is a new item, we need time to transfer knowledge and think whether this item should be on block B or C, it will be a repetitive task that consumes a lot of time (it will be worse if the new operator asking why the naming like this and the old operator just tell the reason it is from legacy, it will be 5 monkeys and a banana experiment) and we can remove this when the naming convention is already proper. So, naming convention must be clear the first time we build something, but this time I will not tell you how to decide a good naming convention, because a good naming convention comes from needs and the team agreement, but I only recommend being more focused on consistency about deciding the naming convention and can be accepted with the team with no hesistation for each person, it is worth to be debatable in the first time and better than will be chaos in the future.
## YAGNI
* From my perspective, YAGNI is not easy, //TODO
## Automatic rules
* Sonar etc
## Code Documentation
* IAAC, PlantUml, Migration, Production Support
## Problem and Goals
* Don't bias


