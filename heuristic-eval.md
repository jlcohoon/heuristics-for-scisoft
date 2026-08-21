# Product & version evaluated: [your tool here]
### Feature or workflow evaluated: [which component of your tool did you focus on?]

### Summary of evaluation: 
[when done, summarize your major findings here]

## 1 - Visibility of System’s Current Status
Your product should always keep users informed about what is going on, through appropriate feedback within a reasonable amount of time. 
- Does the tool clearly communicate its state, including during “processing”  or “thinking” periods or when a timeout error occurs? 
- Is feedback presented quickly after user actions?
- When an action is cancelled, is it clear what the new system status is?

**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]

## 2 - Match Between System and the Real World
The system should reflect norms that its users are already familiar with. The tool should speak the users' language. Use words, phrases, and concepts familiar to a new user, rather than internal jargon. Follow real-world conventions, making information appear in a natural and logical order. 
- Will users be familiar with the terminology used in the interface or commands? 
- Do the tool’s controls follow real-world conventions and workflows?
- Do commands follow similar patterns to those used by competing or related products?
- Are the system outputs in a form the user can directly leverage for subsequent tasks?

**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]

## 3 - User Control and Freedom
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
      
## 4 - Consistency and Standards
Users should not have to wonder whether different words, situations, or actions mean the same thing. Follow platform, industry, and disciplinary conventions. Place information where users have been trained to expect it. Use intuitive, predictable patterns and consistent naming conventions to ensure commands are easily remembered.
- Does the tool follow common conventions, including information organization norms? 
- Is care taken to avoid calling the same thing by multiple names?
- Are your docs organized into standard sections, including information on install and dependencies up front?
  
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
Offer efficiency tools that can be leveraged by users as they gain confidence. Shortcuts — hidden to not distract novice users — may speed up the interaction for the expert user. Allow users to tailor frequent actions. 
- Does the tool provide accelerators like keyboard shortcuts and touch gestures? 
- Is content and functionality personalized or customized for individual users so they more quickly get to what they want?
- Are users able to automate their workflow?
- Does the documentation describe both simple and advanced workflows?
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
## 7 - Aesthetic and Minimalist Design
Interfaces should not contain information that is irrelevant or rarely needed. Every extra unit of information in an interface competes with the relevant units of information and diminishes their relative visibility. Visual design should be consistent and not distracting.
- Is the visual design and content focused on the essentials? 
- Have all distracting, unnecessary elements been removed? 
- Are symbols and emojis used to convey meaning and not just decorate?
- Are visual treatments used consistently throughout?
  
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
- Does the tool offer a solution that solves the error immediately?
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
  
**Issues:**
- [your issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
- [another issue here, possibly including an example]
    -   *Severity:* [critical/moderate/minor, often/sometimes/rarely]
    -   *Recommendation:* [optional, your recommendation here]
      
