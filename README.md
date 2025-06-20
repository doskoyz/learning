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
<img src="https://github.com/user-attachments/assets/82b8e86a-32f6-45f7-a491-17b085c85578" width="300" height="300" />

* I love to share the Eisenhower matrix, because in reality, we often face the issue of deciding urgent and non-urgent. From my perspective, it is easier to decide what is important and non-important instead of deciding what is urgent and non-urgent. Based on my experience, we are sorting the urgent ones in the backlog and hope no re-prioritization that pending for the important non-urgent. So, this is crucial that we *must* set the real timeline to schedule the important non-urgent and put a hard rule not to reschedule the timeline. The real case: we need to refactor the flow, the result of some of the API is unused. From my perspective, the unused API/flow is important to delete. Why? Because when we don't delete it, we need to maintain it. Based on APOSD: "the more information a developer needs to have, the harder it will be for them to work on the system". So it is important to remove the unused information/context before it is bloated in the future.
## Naming Convention
* Some people think naming is not important. Imagine we have a super big warehouse, and we just put the index name of the block as initial names A,B,X,Z. The operator should know where the item is in what block. After that, imagine if there is a new operator or if there is a new item, we need time to transfer knowledge and think whether this item should be on block B or C, it will be a repetitive task that consumes a lot of time (it will be worse if the new operator asking why the naming like this and the old operator just tell the reason it is from legacy, it will be 5 monkeys and a banana experiment) and we can remove this when the naming convention is already proper. So, naming convention must be clear the first time we build something, but this time I will not tell you how to decide a good naming convention, because a good naming convention comes from needs and the team agreement, but I only recommend being more focused on consistency about deciding the naming convention and can be accepted with the team with no hesistation for each person, it is worth to be debatable in the first time and better than will be chaos in the future.
## Design Principle
* Have you ever heard YAGNI, KISS, DRY principles? While we read the documentation, it is like simple terms, but in reality, it is not as easy as the documentation says. There is a lot of subjectivity when we need to prepare the future flow, and we need to make it simple-stupid. My suggestion, it is better to talk with the business/product team to see the future business unit (but it is still hard to predict the future), the second think about what the impact would be if we oversimplify or overengineer. Based on my experience better to make it a generic one for data layers (database), not to do the KISS in these layers, and do the YAGNI in the apps levels, since the data layers will be the biggest effort if there is a business change (atleast if we use the generic for single purpose in data layers it is still fits and readable in apps layers).
* I also learn from my mistakes. I have ever done the over-optimization that sacrifices the readability of code. But nowadays, memory is cheaper than before, so now I prefer to choose readability instead of doing the over-optimization that improves not insignificant performance. But I still agree that performance still matters, it is how you balance the performance and readability of the code. Let's say the traffic is low and less likely to change. Is it worth debating the micro-performance for that flow?
* Config vs Hardcode: it is also a frequently debatable subject, from my perspective, hardcode is not always bad design. Sometimes, hardcoding makes it easier to read the code. So if there is no need different value config across environments and we don't know when the config will be updated, I encourage you to hardcode instead of putting it into the config.
## Company Code Rules
* We used static code analysis to help us standardize the quality of our code (clean code, security, bugs), but some companies standardize the static code for the whole team in the company. It is challenging since it is so hard to create a silver bullet standard for the whole team, because each team can have a different culture. So if our team struggles with the non-sense rule, it will be better to recall why we use this static code? Does it make our code as clean as our standard, or just formalities? If it is just for formality and we agreed it is not relevant to the team, so it is time to start realigning the rule that fits with our culture. My perspective: "static code is to make it easier to read the code, not make it harder".
* The majority of you must be familiar with the code test, right? like integration test, unit test. Based on my experience in the complex flow that has many branches (more than 20), we often "hack" the test so that it can cover the whole branch due to company standard rules (min: 90% coverage). That makes our test not readable, and only God knows the test since it is already complicated. From my perspective:
  * If we use integration tests to test the end-to-end flow, like rest API or event listener, it is okay to create the unit test for the service/helper/util instead of forcing all the branches to be covered.
  * If we use unit tests, please rethink whether it is okay if there are so many branches in one function. If not, just refactor the code instead of "hacking" the test.
## Code Documentation
* IAAC, PlantUml, Migration, Production Support
## Problem and Goals
* Don't bias


