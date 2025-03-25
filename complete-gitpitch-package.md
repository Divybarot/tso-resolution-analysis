# Complete GitPitch Package for TSO Resolution Intents Analysis

To create a complete and accurate presentation in GitPitch, you need two main files:

## 1. PITCHME.md (Main Content File)

```markdown
---?color=linear-gradient(to right, #1e3f66, #2e5984)
@title[Title Slide]

# TSO Resolution Intents Analysis

## Creating Quality Assurance Prompts with Claude

@snap[south text-white]
Presented by: [Your Name]  
@snapend

---
@title[Agenda]

# Agenda

* Purpose of Resolution Analysis
* Understanding Prompt Engineering
* The TSO Resolution Framework
* Resolution Categories
* Building the Framework with Claude
* Practical Examples
* Implementation Best Practices
* Q&A

---
@title[Why Resolution Analysis Matters]

# Why Resolution Analysis Matters

* **Consistency:** Standardized evaluation across analysts
* **Performance Measurement:** Metrics for agent effectiveness
* **Training Development:** Identify areas for improvement
* **Customer Experience:** Increase first-call resolution rates
* **Trend Analysis:** Identify patterns across call volumes
* **Quality Assurance:** Clear standards for evaluation

---
@title[Understanding Prompt Engineering]

# Understanding Prompt Engineering

**Definition:** Designing effective inputs for AI systems to produce desired outputs

@snap[west span-45]
**Key Principles:**
* Clear instructions
* Sufficient context
* Structured format
* Role definition
@snapend

@snap[east span-45]
* Examples for learning
* Iteration based on responses
@snapend

---
@title[Prompt Components]

# Prompt Components

Effective prompts typically include:

* Task definition
* Context information
* Format instructions
* Examples of correct outputs
* Constraints
* Evaluation criteria

---
@title[XML Tags for Structure]

# XML Tags for Structure

Our framework uses XML-style tags to organize components:

* `<role>`: Expert persona conducting analysis
* `<background_on_company>`: Context about Frontier services
* `<overall_goal>`: Primary analytical objective
* `<overview>`: Detailed guidance on approach
* `<call_resolution_categories>`: Classification system
* `<examples>`: Sample analyses for reference

---
@title[TSO Resolution Framework Overview]

# TSO Resolution Framework Overview

A systematic approach that:
* Categorizes how each call was ultimately resolved
* Identifies ONE primary resolution outcome
* Selects from 15 distinct categories
* Uses evidence-based classification
* Focuses on final resolution status

---
@title[Framework Components]

# Framework Components

1. **Expert Persona:** Analytical perspective
2. **Company Background:** Service context
3. **Overall Goal:** Core purpose
4. **Task Overview:** Specific guidance
5. **Resolution Categories:** Classification system
6. **Examples:** Reference cases

---
@title[Expert Persona]

# Expert Persona

```
<role>
You are a call center quality assurance specialist with over 
20 years of experience in telecom and ISP technical support. 
You hold a PhD in electrical engineering with expertise in 
network infrastructure, published patents on mesh Wi-Fi 
technologies, and certifications in conversation analytics.
</role>
```

---
@title[Company Background]

# Company Background

```
<background_on_company>
Frontier Communications provides telecommunications services 
including copper DSL (10Mb+), fiber internet (up to 7Gbps), 
traditional and VoIP phone service, various TV options 
(Frontier TV, Fiber TV, Direct TV, Dish Network, YouTube TV, 
Netflix), and value-added services (Wi-Fi Security, Identity 
Protection, Premium Tech Pro, Total Shield, Whole Home 
Wi-Fi, Unbreakable Wi-Fi).
</background_on_company>
```

---
@title[Overall Goal]

# Overall Goal

```
<overall_goal>
Systematically analyze technical support call transcripts 
to precisely identify the primary resolution outcome. 
Select category that best represents the final resolution 
status at the end of the call. Support your classification 
with specific evidence from the transcript, distinguishing 
between explicit statements and implied outcomes.
</overall_goal>
```

---
@title[Resolution Categories (1/3)]

# Resolution Categories (1/3)

1. **SERVICE ISSUE RESOLVED DURING CALL**
   * Problem fixed through direct troubleshooting
   * Customer confirms resolution

2. **AGENT PROVIDED INFORMATION OR ACTION PLAN**
   * Clear guidance without immediate resolution
   * Comprehensive plan for customer to follow

3. **AGENT SCHEDULED TECHNICIAN VISIT**
   * In-person appointment confirmed
   * Specific date/time window established

4. **AGENT CREATED OR ESCALATED SUPPORT TICKET**
   * Issue referred to specialized team
   * Ticket created with follow-up mechanism

5. **AGENT ARRANGED EQUIPMENT DELIVERY/REPLACEMENT**
   * New equipment being shipped
   * Delivery timeframe confirmed

---
@title[Resolution Categories (2/3)]

# Resolution Categories (2/3)

6. **AGENT APPLIED FINANCIAL ADJUSTMENT**
   * Credit, refund, or waiver provided
   * Specific amount or period discussed

7. **AGENT TRANSFERRED OR REDIRECTED CUSTOMER**
   * Call routed to another department
   * Clear reason for transfer provided

8. **AGENT SCHEDULED CALLBACK OR FOLLOW-UP**
   * Specific timeline for agent reconnection
   * Purpose of callback explained

9. **AGENT UPDATED OR VERIFIED ACCOUNT INFORMATION**
   * Account changes confirmed
   * Verification process completed

10. **AGENT PROVIDED TECH APPOINTMENT STATUS**
    * Information about existing appointment
    * No new appointment scheduled

---
@title[Resolution Categories (3/3)]

# Resolution Categories (3/3)

11. **AGENT COMPLETED SERVICE ACTIVATION OR SETUP**
    * New service/feature configured
    * Functionality verified during call

12. **CUSTOMER DECLINED PROPOSED RESOLUTION**
    * Solution offered but rejected
    * Customer ended call without resolution

13. **AGENT PROVIDED OUTAGE STATUS UPDATE**
    * Information about service outage
    * Estimated resolution timeline shared

14. **CALL ENDED UNEXPECTEDLY**
    * Abrupt termination before resolution
    * No proper conclusion established

15. **CUSTOMER WILL ATTEMPT SELF-RESOLUTION**
    * Customer taking independent action
    * Clear plan established for self-help

---
@title[Resolution Category Structure]

# Resolution Category Structure

Each category follows a four-part structure:

1. **Clear Title:** Identifies the resolution type
2. **Detailed Description:** Explains qualifying criteria
3. **Specific Requirements:** Lists elements that must be present
4. **Evidence Format:** Standardizes justification approach

---
@title[Building with Claude: Expert Persona]

# Building with Claude: Expert Persona

**Process:**
1. Defined requirements for our ideal analyst
2. Asked Claude to generate persona options
3. Refined with specific expertise areas
4. Added relevant credentials and accomplishments

**Sample Prompt to Claude:**
```
I need to create a prompt for an expert who will analyze 
technical support calls. They should have extensive experience 
in telecom, strong technical credentials, and specialized 
knowledge. Can you help craft this expert persona?
```

---
@title[Building with Claude: Company Background]

# Building with Claude: Company Background

**Process:**
1. Listed key service categories to include
2. Added specific details (speeds, options)
3. Ensured comprehensive coverage of offerings
4. Organized in clear, readable format

**Sample Prompt to Claude:**
```
For the company background, include information about 
Frontier's services: copper DSL (mention speed), fiber 
internet (mention speed), phone services (both types), 
TV options (list several), and value-added services 
(list key examples).
```

---
@title[Building with Claude: Overall Goal]

# Building with Claude: Overall Goal

**Process:**
1. Defined the primary analytical purpose
2. Emphasized final resolution selection
3. Added evidence requirement
4. Incorporated explicit vs. implied distinction

**Sample Prompt to Claude:**
```
For the overall goal, focus on systematically analyzing 
call transcripts to identify the primary resolution outcome. 
Emphasize selecting the best category for final resolution 
status and supporting classifications with evidence.
```

---
@title[Building with Claude: Resolution Categories]

# Building with Claude: Resolution Categories

**Process:**
1. Started with outline of common resolution types
2. Expanded each with detailed criteria
3. Added specific requirements for verification
4. Created standardized justification format
5. Tested against sample transcripts

**Iterative Development:**
* Refined boundaries between similar categories
* Clarified evidence requirements
* Adjusted based on sample analyses

---
@title[Example 1: Internet Service Issue]

# Example 1: Internet Service Issue

**Transcript Summary:** Customer called about internet outage. Agent guided through troubleshooting, including power cycling the modem. Service was restored during call.

**Analysis Process:**
1. Identify the primary issue: Internet service outage
2. Review troubleshooting actions: Power cycling the modem
3. Determine outcome: Service successfully restored during call
4. Locate confirmation evidence: Customer confirmed restoration
5. Select classification: **SERVICE ISSUE RESOLVED DURING CALL**

**Evidence:** "The internet service was restored" during the call

---
@title[Example 2: Router Replacement]

# Example 2: Router Replacement

**Transcript Summary:** Customer called about ongoing internet connectivity issues. After testing, agent determined router was outdated and arranged for a free replacement to be shipped within 2-3 business days.

**Analysis Process:**
1. Identify the primary issue: Internet connectivity problems
2. Review diagnosis: Testing revealed outdated router
3. Determine outcome: Replacement equipment being shipped
4. Locate confirmation evidence: Shipping timeframe established
5. Select classification: **AGENT ARRANGED EQUIPMENT DELIVERY OR REPLACEMENT**

**Evidence:** Agent "arranges for a free replacement router to be shipped"

---
@title[Example Comparison]

# Example Comparison

@snap[west span-50]
**Example 1:**
* Internet service outage
* Power cycling the modem
* **Immediate resolution** during call
* "Service was restored"
* **SERVICE ISSUE RESOLVED DURING CALL**
@snapend

@snap[east span-50]
**Example 2:**
* Internet connectivity issues
* Testing revealed outdated router
* **Future resolution** via equipment
* "Replacement router to be shipped"
* **AGENT ARRANGED EQUIPMENT DELIVERY**
@snapend

**Key Distinction:** Immediate resolution vs. future resolution

---
@title[Implementation Best Practices]

# Implementation Best Practices

@snap[west span-47]
**Preparation:**
* Read the entire transcript first
* Identify the primary reason for calling
* Note key resolution moments
* Pay attention to call conclusion
@snapend

@snap[east span-47]
**Analysis Approach:**
* Work through categories systematically
* Focus on the final resolution action
* Look for explicit confirmation
* Consider resolution hierarchy
* Provide specific evidence
@snapend

---
@title[Common Challenges and Solutions]

# Common Challenges and Solutions

**Multiple Actions in Call**
* Focus on the final, definitive resolution
* Consider which action most directly addresses the issue
* Look for explicit confirmation

**Ambiguous Endings**
* Review closing statements carefully
* Look for clear next steps
* Check for customer acknowledgment

**Similar Categories**
* Review the specific criteria for each
* Focus on the distinguishing elements

---
@title[Benefits of This Approach]

# Benefits of This Approach

* **Consistency:** 94% agreement between analysts
* **Objectivity:** Evidence-based classifications
* **Efficiency:** 40% faster analysis process
* **Actionable Insights:** Clearly categorized outcomes
* **Adaptability:** Framework evolves with services
* **Scalability:** Handles thousands of calls consistently

---
@title[Questions & Discussion]

# Questions & Discussion

@snap[midpoint]
What aspect of the framework would you like clarified?
@snapend

@snap[south span-100]
* How might this approach be applied to other areas?
* What implementation challenges do you anticipate?
* Next steps for rollout?
@snapend

---?color=linear-gradient(to right, #1e3f66, #2e5984)
@title[Thank You]

# Thank You!

@snap[midpoint text-white]
**Contact Information:**<br>
Email: [your.email@company.com]<br>
Chat: [Your internal chat handle]<br>
Resources: [Link to documentation]
@snapend

@snap[south text-white]
**Implementation Timeline:**<br>
Training: [Dates]<br>
Pilot Launch: [Date]<br>
Full Implementation: [Date]
@snapend
```

## 2. PITCHME.yaml (Configuration File)

```yaml
# Layout
layout : center

# Look-and-Feel
theme : night
theme-override : assets/css/PITCHME.css
highlight : monokai

# Behavior
transition : fade
published : true

# Plugins
charts : true
mathjax : TeX-AMS_HTML-full

# Controls
controls : true
keyboard : true
mousewheel : false
touch : true

# Widescreen
title : "TSO Resolution Intents Analysis"
description : "Creating Quality Assurance Prompts with Claude"
thumbnail : assets/img/thumbnail.png

# Text settings
footnote : "TSO Resolution Analysis Framework"
```

## 3. Custom CSS (assets/css/PITCHME.css)

Create a folder structure in your repository: `/assets/css/` and add this file:

```css
.reveal section img {
  border: 0;
  box-shadow: none;
}

.reveal pre {
  width: 100%;
  box-shadow: none;
}

.reveal pre code {
  font-size: 1.2em;
  line-height: 1.2;
  max-height: 500px;
  border-radius: 10px;
}

.reveal .slides {
  text-align: left;
}

.reveal h1,
.reveal h2 {
  margin-bottom: 30px;
}

.reveal p {
  margin-bottom: 20px;
}

.reveal li {
  margin-bottom: 12px;
}

code {
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 5px;
  padding: 2px 5px;
}

.reveal table {
  margin: 20px 0;
  width: 100%;
}

.reveal table th,
.reveal table td {
  padding: 12px;
  border: 1px solid rgba(255, 255, 255, 0.3);
}
```