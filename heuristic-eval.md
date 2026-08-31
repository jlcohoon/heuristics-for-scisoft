# Product & version evaluated: [your tool here]
### Feature or workflow evaluated: [which component of your tool did you focus on?]

### Summary of evaluation: 
[when done, summarize your major findings here]

## 1 - Visibility of System’s Current Status
Your product should always keep users informed about what is going on, through appropriate feedback within a reasonable amount of time. Information about the code's status as well as what the system is doing while in use should be available.
- Does the tool clearly communicate its state, including during “processing”  or “thinking” periods or when a timeout error occurs? 
- Is feedback presented quickly after user actions?
- When an action is cancelled, is it clear what the new system status is?
- Are release notes available to users?
- Is it clear which branch is stable?

**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]

## 2 - Match Between System and Prior Expectations
The system should reflect norms that its users are already familiar with so that the tool behaves as they expect. The tool should speak the users' language (whether that's a scientific domain or software engineering terminology) rather than use internal jargon. Follow conventions your anticipated users will be familiar with.
- Will users be familiar with the terminology used in the interface or commands? 
- Do the tool’s controls follow conventions and workflows users will already know?
- Are the system outputs in a form the user can directly leverage for subsequent tasks?
- Are settings located where users will easily find them?
- Are your docs organized into standard sections, including information on install and dependencies up front?

**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
## 3 - Internal Consistency
Maintain consistent patterns so that users can easily learn to use and navigate your product. Users should not have to wonder whether different words, situations, or actions mean the same thing. Use intuitive, predictable patterns and consistent naming conventions to ensure commands are easily remembered. 
- Is care taken to avoid calling the same thing by multiple names?
- Are visual treatments used consistently throughout?
- Do command-line flags, arguments, and naming conventions follow a predictable pattern throughout the tool?
- Are the "exit" or "cancel" paths consistent across all workflows?
- Do similar actions produce similar results (e.g., If "Delete" asks for confirmation in one menu, does it also ask for it in another?)

**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]

## 4 - User Control and Freedom
Users should be able to easily perform actions and undo them. Users often perform actions by mistake. They need a clearly marked "emergency exit" to leave the unwanted action without having to go through an extended process. 
- Are available options obvious to users?
- Does the tool allow users to go back a step in the process? 
- Are exits easily discoverable to new users? 
- Can users easily cancel an action? 
- Is Undo and Redo supported?
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
            
## 5 - Recognition Rather Than Recall
Minimize the user's memory load by making elements, actions, and options visible. The user should not have to remember information from one part of the interface to another. Information required to use the product (e.g. field labels or menu items) should be visible or easily retrievable when needed. 
- Does the tool keep important information visible, so that users do not have to memorize it? 
- Does the tool offer help in-context? 
- Is it clear to a user where they are in the system or workflow?
- Are interactive commands used to help new users of CLI tools gain familiarity with the system and available flags?
- Are steps requiring copying and pasting from one place to another minimized?
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
## 6 - Flexibility and Efficiency of Use
Ensure your tool adapts to the full range of user needs, scales, and skill levels you anticipate, providing a flexible experience that remains efficient as users grow in expertise and work becomes more complicated. There are two general forms of flexibility: for the user and for heterogenous data and work. Users may be novices or advanced, the latter being capable of using advanced shortcuts. Data and work may be big or small, complex or simple, with long or no histories.

*User flexibility:*
- Does the tool provide accelerators like keyboard shortcuts and touch gestures? 
- Is content and functionality personalized or customized for individual users so they more quickly get to what they want?
- Are users able to automate their workflow?

*Data and work flexibility:*
- Does the interface work well for both small and large workloads?
- Does the interface work well for both big and small data?
- Is it easy to construct both a simple and complex workflows?
- Does the interface make sense when a user logs in for the very first time?

  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
## 7 - Direct Attention Judiciously
Interfaces should not contain information that is irrelevant or rarely needed. Every extra unit of information in an interface competes with the relevant units of information and diminishes their relative visibility. Visual design should be consistent, not distracting, and used to focus users' attention where it is most needed.
- Have all distracting, unnecessary elements been removed? 
- Are symbols and images used to convey meaning and not just decorate?
- Is the visual design and content focused on the essentials?
- Do you use size, contrast, and proximity to focus users' attention on the most important content?
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]

## 8 - Guardrails for Error Prevention
Support for recovering from errors is important, but the best tools help users avoid committing errors in the first place. Eliminate error-prone conditions or check for them and present users with a confirmation option before they commit to the action. Shepherd users through complex actions step-by-step so they don't make mistakes.
- Does the tool prevent slips by using helpful constraints? 
- Does the tool warn users or introduce useful friction before they perform risky actions?
- Are appropriate defaults selected?
- Are there appropriate guardrails in place to ensure a user only works “dangerously” when it is safe to do so?
- Is input validation used when possible?
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
## 9 - Help Users Recognize, Diagnose, and Recover from Errors
Error messages should be expressed in plain language (no error codes), precisely indicate the problem, and constructively suggest a solution. 
- Does the tool use traditional error message visuals, like bold, red text? 
- Does the tool or documentation offer a direct solution to solve the error or debugging techniques?
- Is there a way to monitor ongoing processes?
- Are log files available for reviewing issues?
- Is it clear when an issue is related to a third-party?
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
## 10 - Help and Documentation
Documentation helps users understand how to complete their tasks and reproduce workflows later; it is also useful for AI agents seeking information about your product.
- Is help documentation easy to search? 
- Is help provided in context right at the moment when the user requires it? 
- Are there examples of the most popular workflows?
- Are appropriate markdown files provided to LLMs and agents?
- Does the documentation describe both simple and advanced workflows?
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
