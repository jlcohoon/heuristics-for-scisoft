# An Approach to Heuristic Evaluation for Scientific Software
Jakob Nielsen's presents [10 general principles for interaction design](https://www.nngroup.com/articles/ten-usability-heuristics/). These principles, also called heuristics, define best practices for implementing good user experiences. Scientific software developers often find these heuristics difficult to apply to their work, frequently because their software requires complex interfaces or has no GUI. The [PESO project](https://pesoproject.org/) and [CASS](https://cass.community/) have adapted Nielsen's heuristics so that they are more easily applied to scientific software. Use this repo to learn the heuristics and conduct an evaluation of a software tool.

## Why heuristic evaluation
Conducting a heuristic evaluation allows you to systematically identify usability issues in your product. By reviewing your own tool in light of Nielsen’s principles, you may notice details that went unseen previously or violations of best practices you were unaware of. A heuristic evaluation like this can be applied to any user interface, meaning any digital product that a user interacts with: a website, an app, a command line tool, a software library, etc.

## How to use this tool
**General Process:**
1. Review all of the heuristics and their prompt questions. Some prompt questions may not apply to your type of software—that's okay, they're just there to inspire you and clarify the meaning of the heuristic.
2. Read the FAQs below if you haven't already.
3. Quickly re-familiarize yourself with the workflow or feature you will evaluate. Depending on the tool, it may be feasible for you to conduct a full review, but heuristic evaluation can be time consuming, taking several hours. We recommend focusing on a workflow or feature so that you do not become overwhelmed. Record, in the provided space, which tool and feature or workflow you are evaluating.
4. Re-review the workflow or feature, this time more slowly, walking through a typical user journey (i.e. the usual steps a user would follow) and assigning issues to the relevant heuristics in whatever order you encounter them. Replace the placeholder text with a description of the problem you see.
    1. Include screenshots and examples as needed for clarity.
    2. You may choose to make a recommendation on how to address the issue, though there are often many ways to resolve problems and you might benefit from a group discussion before asserting a solution.
    3. You may choose to include a severity ranking. See below for how to do this.
5. Before completing your work, read through the heuristics one by one, adding any issues you may have missed and recategorizing issues as you see fit.
6. At the top of the document, summarize the major issues you found or general trends you see.
7. If there is a development team to share your review with, we recommend you share your documented work and then discuss to prioritize issues, determine the level of effort to address them, and develop solutions. Otherwise, do this prioritization and solutioning on your own.

**Assigning severity rankings:**

You may choose to assign a severity to the issues you identify. You can use your own system for this, or ours:
- **Critical:** Prevents users from completing a task (e.g., broken functionality or unclear instructions) or has significant impact on the product’s ability to deliver its value proposition
- **Moderate:** Slows users down or causes frustration but doesn’t prevent task completion or impact delivery of value proposition
- **Minor:** Small mistakes with minimal impact on task completion or delivery of the tool's value proposition
  
We further recommend noting how often users are likely to be affected by the issue. You can use this scale as a rough guide:
- **Often:** A substantial proportion of your users are likely to encounter the issue *or* those who do encounter it do so very frequently
- **Sometimes:** A moderate proportion of your users are likely to encounter the issue *or* those who do encounter it do so occasionally
- **Rarely:** A small of your users are likely to encounter the issue *or* those who do encounter it do so rarely


### Example: Evaluating a Data Catalog

***Heuristic #4 - Consistency and Standards***
- Empty fields are denoted in multiple ways and with different text formatting, for example: “No data available.” “No data found” “-” “--” “No Tags added” “No Description” “No description”
    - *Severity:* minor, often
    - *Recommendation:* Apply a consistent scheme for indicating a lack of information, including punctuation and capitalization. 
Ensure that it is clear whether the data cannot be retrieved or if it was never provided.


### Example: Evaluating an AI agent with chat interface

***Heuristic #1 - Visibility of System Status***
- Queries are not named/IDed but previous queries are discussed by the agent, making it ambiguous what is the object of discussion. For example: The agent says, “Let me check what went wrong with the query,” and “Let me wait and check the status,” but doesn’t say which query is being checked.
    - *Severity:* moderate, often
    - *Recommendation:* Provide IDs for queries so that they can be explicitly referenced.

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

## How we adapted the heuristics
The [STRUDEL](https://strudel.science/) team [first adapted](https://zenodo.org/records/20517042) Nielsen's heuristics, adding additional prompt questions and creating a workbook for people to document issues in. [PESO](https://pesoproject.org/) and [CASS](https://cass.community/) then worked with five scientific software developers to further improve the usability of this tool. PESO and CASS asked the developers to conduct evaluations with the STRUDEL workbook and interviewed them about their experiences afterward. Common issues were noted and revisions were subsequently made. Some notable findings were:

- People valued the examples, prompt questions, and [link to Nielsen's](https://www.nngroup.com/articles/ten-usability-heuristics/) own description of the heuristics
- Many heuristics and prompt questions felt too oriented toward GUIs
- The developers sometimes misunderstood the meaning of a heuristic, sometimes because they have their own associations with certain language (e.g., errors)
- The Google Doc format and layout of the content could be improved
- People were uncertain about how to evaluate severity, how much time to spend, and exactly what order they should work in
- There was uncertainty about how to keep things simple for users and provide needed complexity; the developers were unsure how accessible they should be making their tool

Based on these findings and the examples produced by the five developers, we updated the instructions and FAQs, reworded the titles and descriptions of some heuristics, revised prompt questions, and transitioned away from Google Docs to Github. 

## Contact
If you encounter issues with this documentation or during your heuristic evaluation, reach out to the [CASS User/Developer Experience working group](https://cass.community/working-groups/user-developer-experience.html) via email or during one of their regular discussion hours. You may also [open an issue](/../../issues).
