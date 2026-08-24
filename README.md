# An Approach to Heuristic Evaluation for Scientific Software
Jakob Nielsen, a leading authority on usability, established [10 general principles for interaction design](https://www.nngroup.com/articles/ten-usability-heuristics/). These *heuristics* define best practices for implementing intuitive user experiences. However, scientific software developers often struggle to apply these heuristics to their work, as their software may requires complex interfaces or have no GUI. To bridge this gap, the [PESO project](https://pesoproject.org/) and [CASS](https://cass.community/) have adapted Nielsen's heuristics for scientific software. Use this repo to learn the heuristics and conduct an evaluation of your own software tool.

Quick link to the heuristics and evaluation template: [heuristic-eval.md](/heuristic-eval.md)

## Table of Contents
1. [Why heuristic evaluation](#why-heuristic-evaluation)
2. [How to use this tool](#how-to-use-this-tool)
4. [Examples](#examples)
5. [FAQ](#faq)
6. [How we adapted the heuristics](#how-we-adapted-the-heuristics)
7. [Contact and Get Involved](#contact-and-get-involved)

## Why heuristic evaluation
Conducting a heuristic evaluation allows you to systematically identify usability issues in your product. By reviewing your own tool in light of these heuristics, you may notice details that went unseen previously or violations of best practices you were unaware of. A heuristic evaluation like this can be applied to any user interface, meaning any digital product that a user interacts with: a website, an app, a command line tool, a software library, etc.

## How to use this tool
Heuristic evaluation is an exercise that helps you step out of your usual perspective as a developer and focus more on how users actualy perceive your product. Because these heuristics are broad guidelines, applying them effectively requires critical thinking; it is normal to encounter a learning curve at first. By completing this evaluation, you will be better equipped to make informed design and development decisions.

**General Process:**
1. Create a fork of this repo for you to work in.
2. Review all of the heuristics in [heuristic-eval.md](/heuristic-eval.md) and their prompt questions. Some prompt questions may not apply to your type of software—that's okay, they're just there to inspire you and clarify the meaning of the heuristic.
3. Quickly re-familiarize yourself with the workflow or feature you will evaluate. Depending on the tool, it may be feasible for you to conduct a full review, but heuristic evaluation can be time consuming, taking several hours. We recommend focusing on a workflow or feature so that you do not become overwhelmed. Record, in the provided space at the top of [heuristic-eval.md](/heuristic-eval.md), which tool and feature or workflow you are evaluating.
4. Re-review the workflow or feature, this time more slowly, walking through a typical user journey (i.e. the usual steps a user would follow) and assigning issues to the relevant heuristics in whatever order you encounter them. Do this assignment in [heuristic-eval.md](/heuristic-eval.md). Replace the placeholder text with a description of the problem you see.
    1. Include screenshots and examples as needed for clarity.
    2. You may choose to make a recommendation on how to address the issue, though there are often many ways to resolve problems and you might benefit from a group discussion before asserting a solution.
    3. You may choose to include a severity ranking. See below for how to do this.
5. Before completing your work, read through the heuristics one by one, adding any issues you may have missed and recategorizing issues as you see fit.
6. At the top of the document, summarize the major issues you found or general trends you see.
7. If there is a development team to share your review with, we recommend you share your documented work and then discuss to prioritize issues, determine the level of effort to address them, and develop solutions. Otherwise, do this prioritization and solutioning on your own.

You can repeat this heuristic evaluation exercise at regular intervals, ensuring that as your product evolves, you continue to deliver good user experiences.

**Assigning severity rankings:**

You may choose to assign a severity to the issues you identify. You can use your own system for this, or ours:
- **Critical:** Prevents users from completing a task (e.g., broken functionality or unclear instructions) or has significant impact on the product’s ability to deliver its value proposition
- **Moderate:** Slows users down or causes frustration but doesn’t prevent task completion or impact delivery of value proposition
- **Minor:** Small mistakes with minimal impact on task completion or delivery of the tool's value proposition
  
We further recommend noting how often users are likely to be affected by the issue. You can use this scale as a rough guide:
- **Often:** A substantial proportion of your users are likely to encounter the issue *or* those who do encounter it do so very frequently
- **Sometimes:** A moderate proportion of your users are likely to encounter the issue *or* those who do encounter it do so occasionally
- **Rarely:** A small of your users are likely to encounter the issue *or* those who do encounter it do so rarely

## Examples
### Example: Evaluating an AI agent with chat interface
***Heuristic #1 - Visibility of System Status***
- Queries are not named/IDed but previous queries are discussed by the agent, making it ambiguous what is the object of discussion. For example: The agent says, “Let me check what went wrong with the query,” and “Let me wait and check the status,” but doesn’t say which query is being checked.
    - *Severity:* moderate, often
    - *Recommendation:* Provide IDs for queries so that they can be explicitly referenced.

### Example: Evaluating a math library
***Heuristic #2 - Match Between System and Prior Expectations***
- The initial design used the word “evaluate” to mean “compute the value of”, when related to the sparse grid surrogate. However, with the more recent introduction of neural network models, the word “evaluate” now has a different meaning in the context of surrogate modeling.
    - *Severity:* minor, often
    - *Recommendation:* Keep the existing evaluate method for backwards compatibility but also add a new method with a more appropriate name, e.g., “compute” or “simulate” or “value at” 

### Example: Evaluating a data catalog
***Heuristic #3 - Internal Consistency***
- Empty fields are denoted in multiple ways and with different text formatting, for example: “No data available.” “No data found” “-” “--” “No Tags added” “No Description” “No description”
    - *Severity:* minor, often
    - *Recommendation:* Apply a consistent scheme for indicating a lack of information, including punctuation and capitalization. Ensure that it is clear whether the data cannot be retrieved or if it was never provided.

### Example: Evaluating a container tool
***Heuristic #4 - User Control and Freedom***
- The users can generally use “Ctrl+C” to stop the process. However, this assumes the users are familiar with basic linux commands.
    - *Severity:* moderate, sometimes
    - *Recommendation:* Before the actual runnings, information/tips about checking/changing the running status can be printed on the screen so users know what to do after running.

### Example: Evaluating a math library
***Heuristic #5 - Recognition Rather Than Recall***
- The sparse grid class has multiple modes (e.g., local vs. global basis, batch-adaptive vs. dynamic construction) of operations and MANY methods. Some methods are only usable/accessible in some modes. While objects can always be thoroughly queried, the documentation can benefit better clarification on the categories.
    - *Severity:* moderate, sometimes
    - *Recommendation:* Improve the documentation for people that are not familiar with the intricacies of math theory of sparse grids and hence may struggle to understand why some methods are disabled or throw exceptions. Make clearer what methods are available under what circumstances

### Example: Evaluating a data catalog
***Heuristic #6 - Flexibility and Efficiency of Use***
- Users have no way of quickly getting to their most important datasets—they have to search or scroll through all of their datasets to find the ones they are looking for, even if they visit it daily.
    - *Severity:* moderate, often
    - *Recommendation:* Allow users to bookmark datasets and display those prominently so they can be accessed very quickly

### Example: Evaluating a data catalog
***Heuristic #7 - Direct Attention Judiciously***
- Badges showing schema types (e.g. string) have a color not used elsewhere (purple), drawing the eye to a relatively unimportant GUI component.
    - *Severity:* minor, often
    - *Recommendation:* Use accenting colors only for high priority information. Make type badges blue or grey like other badges.

### Example: Evaluating a container tool
***Heuristic #8 - Guardrails for Error Prevention***
- By default, the image files are saved on the login node. This should be combined with the migrate command to avoid wasted spaces and losing tracking of built images. However, users may not know this and forget the second step.
    - *Severity:* moderate, sometimes
    - *Recommendation:* Add a constraint to users while building the images and ask them whether to “migrate” the images before they leave the session, warning them of the consequences of not doing so. The default should be set to a safer choice which is doing the “migrate”.

### Example: Evaluating a modeling code
***Heuristic #9 - Help Users Recognize, Diagnose, and Recover from Errors***
- There are multiple occasions where the code aborts with no helpful information
    - *Severity:* critical, sometimes
    - *Recommendation:* Continue to add checks that will generate useful print output rather than just crashes

### Example: Evaluating an AI agent with chat interface
***Heuristic #10 - Help and Documentation***
- Some terms the agent uses in chat may be jargon to novice users but getting them defined would require interrupting the current query or leaving the interface.
    - *Severity:* minor, sometimes
    - *Recommendation:* Identify key terms of art and ensure that when used by the agent, a definition is provided within the interface.

## FAQ
**Isn’t this subjective?**
Yes, but heuristics offer rules of thumb that are known to improve usability of a given tool. If you see an instance where your tool seems to violate one of these heuristics, it is likely that other people will too. If you don’t catch all the issues, what you do find can still meaningfully improve usability.

**I’m not a UX expert, can I still do this?**
Yes, there is no special language you need to know or outside knowledge you need to have that is not included in this template. Just describe the issues you see in your own words and provide examples to help ensure any collaborators understand as well. If you need more support, reach out to the [CASS User/Developer Experience working group](https://cass.community/working-groups/user-developer-experience.html) via email or during one of their regular discussion hours. 

**What type of user should I be thinking about?**
Often, usability advice will encourage you to ensure broad accessibility, and this may make you think that it's recommended that *anyone* should be able to use your tool. That isn't necessarily true. Consider who could gain value from using your tool and the knowledge those people might have. When conducting your heuristic evaluation, evaluate the user experience from the perspectives of both novice and expert users, keeping in mind that even a novice user will have some background knowledge.

**I thought my issue belonged in one category but then later I thought it belonged to another. What do I do?**
Many times an issue will span multiple heuristics. Choose the option that best summarizes the problem you perceive.

**I didn't have an issue for every heuristic. Is that okay?**
Yes, you may not find problems associated with every heuristic. Sometimes this is because of the nature of your tool, other times it's because there just aren't problems of that type. You do not need to find something for every heuristic.

**Can this be a team exercise?**
Yes! This can ensure better coverage, though it should be noted that heuristic evaluation is like using a fine toothed comb and not all issues you identify may have a meaningful impact on usability. We recommend that individuals conduct their own reviews and then discuss the issues they found together so you can see which were most prominent among you and how you perceived their severity. 

**How do I do this more quickly?**
To cut down on time spent on a heuristic evaluation, avoid making recommendations or ranking the severity of an issue. You can also make just a single pass through the heuristics, rather than going back through and looking for missed issues. Don't fuss too much over which heuristic you've categorized an issue under—the key is that you adopted a user-centered perspective and have identified an issue.

## How we adapted the heuristics
The [STRUDEL](https://strudel.science/) team [first adapted](https://zenodo.org/records/20517042) Nielsen's heuristics, adding additional prompt questions and creating a workbook for people to document issues in. [PESO](https://pesoproject.org/) and [CASS](https://cass.community/) then worked with five scientific software developers to further improve the usability of this tool. PESO and CASS asked the developers to conduct evaluations with the STRUDEL workbook and interviewed them about their experiences afterward. Common issues were noted and revisions were subsequently made. Some notable findings were:

- People valued the examples, prompt questions, and [link to Nielsen's](https://www.nngroup.com/articles/ten-usability-heuristics/) own description of the heuristics
- Many heuristics and prompt questions felt too oriented toward GUIs
- The developers sometimes misunderstood the meaning of a heuristic, sometimes because they have their own associations with certain language (e.g., errors)
- The Google Doc format and layout of the content could be improved
- People were uncertain about how to evaluate severity, how much time to spend, and exactly what order they should work in
- There was uncertainty about how to keep things simple for users and provide needed complexity; the developers were unsure how accessible they should be making their tool

Based on these findings and the examples produced by the five developers, we updated the instructions and FAQs, reworded the titles and descriptions of some heuristics, revised prompt questions, and transitioned away from Google Docs to Github. 

## Contact and Get Involved
If you encounter issues with this documentation or during your heuristic evaluation, reach out to the [CASS User/Developer Experience working group](https://cass.community/working-groups/user-developer-experience.html) via email or during one of their regular discussion hours. You may also [open an issue](/../../issues).

We are seeking more examples of how people have applied the heuristic evaluation process to their software. Please get in touch or open a pull request to share your example. You can add a small one to the list above or we can link to your full evaluation.
