# Knowledgebase Fixes Required - Staging Branch

This document lists all spelling, grammar, and formatting issues found in the staging branch of the knowledgebase, along with the exact changes needed to fix them.

---

## 1. docs.json

### Issue 1: Typo in navigation
**Line:** 103
**Current:**
```json
"group": "Agent Guildelines"
```
**Change to:**
```json
"group": "Agent Guidelines"
```

### Issue 2: Extra space in navigation
**Line:** 145
**Current:**
```json
"group": " AGENT KNOWLEDGEBASE"
```
**Change to:**
```json
"group": "AGENT KNOWLEDGEBASE"
```

---

## 2. get-started/overview.mdx

### Issue: Typo in description
**Line:** 3
**Current:**
```yaml
description: "Phonel is a voice AI platform that allows you to build, deploy, and manage AI-powered voice agents."
```
**Change to:**
```yaml
description: "Phonely is a voice AI platform that allows you to build, deploy, and manage AI-powered voice agents."
```

---

## 3. get-started/quick-start.mdx

### Issue: Spelling error
**Line:** 6
**Current:**
```
Building voice AI agents has never been easier. Get started in just a few simple steps to build the AI that can automate anything, repeatibly, every single time.
```
**Change to:**
```
Building voice AI agents has never been easier. Get started in just a few simple steps to build the AI that can automate anything, repeatedly, every single time.
```

---

## 4. get-started/dashboard-overview.mdx

### Issue: Incorrect word usage
**Line:** 49
**Current:**
```
- A sudden drop in bound calls
```
**Change to:**
```
- A sudden drop in outbound calls
```

---

## 5. key-concepts/flows.mdx

### Issue 1: Excessive spacing
**Line:** 23
**Current:**
```
- Collecting information (Collect).                                                                                                     
```
**Change to:**
```
- Collecting information (Collect).
```

### Issue 2: Spelling error
**Line:** 25
**Current:**
```
- Handling trasnfers (Transfer).
```
**Change to:**
```
- Handling transfers (Transfer).
```

---

## 6. key-concepts/variables.mdx

### Issue: Missing capital letter
**Line:** 73
**Current:**
```
### ive vs. post-call actions
```
**Change to:**
```
### Live vs. post-call actions
```

---

## 7. outboundcalling/createaoutboundcallingcampaign.mdx

### Issue 1: Inappropriate callout type
**Line:** 17-19
**Current:**
```mdx
<Danger>
  Campaigns support both batch calling for large lead uploads and \*\*continuous \*\*mode for real-time outreach as new leads sync from your CRM.
</Danger>
```
**Change to:**
```mdx
<Info>
  Campaigns support both **batch** calling for large lead uploads and **continuous** mode for real-time outreach as new leads sync from your CRM.
</Info>
```

### Issue 2: Excessive trailing spaces
**Line:** 21
**Current:**
```
Once configured, the system can automatically call new leads as they appear or process static lists of contacts in defined batches. The campaign setup process is divided into structured steps to ensure accuracy and compliance.                     
```
**Change to:**
```
Once configured, the system can automatically call new leads as they appear or process static lists of contacts in defined batches. The campaign setup process is divided into structured steps to ensure accuracy and compliance.
```

### Issue 3: Excessive bold formatting in headers
**Line:** 27
**Current:**
```markdown
### **Campaign Name**
```
**Change to:**
```markdown
### Campaign Name
```

### Issue 4: Excessive bold formatting in headers
**Line:** 35
**Current:**
```markdown
### **Campaign Use Cases**
```
**Change to:**
```markdown
### Campaign Use Cases
```

### Issue 5: Excessive bold formatting in headers
**Line:** 53
**Current:**
```markdown
### **Connecting Twilio**
```
**Change to:**
```markdown
### Connecting Twilio
```

### Issue 6: Excessive trailing spaces
**Line:** 73
**Current:**
```
3. **Country-Based Routing** – Used for international outreach.\
   Calls are routed through numbers assigned to the recipient's country, preserving a local presence and helping with compliance in regions where cross-border calls may be restricted.     \
   As with state-based routing, if no local number exists, Phonely falls back to a random enabled number.
```
**Change to:**
```
3. **Country-Based Routing** – Used for international outreach.\
   Calls are routed through numbers assigned to the recipient's country, preserving a local presence and helping with compliance in regions where cross-border calls may be restricted.\
   As with state-based routing, if no local number exists, Phonely falls back to a random enabled number.
```

### Issue 7: Excessive bold formatting in headers
**Line:** 86
**Current:**
```markdown
**Calls per Hour**
```
**Change to:**
```markdown
### Calls per Hour
```

### Issue 8: Excessive bold formatting in headers
**Line:** 98
**Current:**
```markdown
**Campaign Type: Continuous vs Batch**
```
**Change to:**
```markdown
### Campaign Type: Continuous vs Batch
```

### Issue 9: Excessive bold formatting in headers
**Line:** 108
**Current:**
```markdown
### **Trigger Sources**
```
**Change to:**
```markdown
### Trigger Sources
```

### Issue 10: Excessive bold formatting in headers
**Line:** 169
**Current:**
```markdown
### **Selecting or Editing a Flow**
```
**Change to:**
```markdown
### Selecting or Editing a Flow
```

### Issue 11: Excessive bold formatting in headers
**Line:** 175
**Current:**
```markdown
### **Mapping Variables**
```
**Change to:**
```markdown
### Mapping Variables
```

---

## 8. agent-design/voice/voice-and-personality.mdx

### Issue 1: Spelling error in description
**Line:** 3
**Current:**
```yaml
description: "Learn on how to configure personality for your voice agent, add office noise and humanize coversations"
```
**Change to:**
```yaml
description: "Learn on how to configure personality for your voice agent, add office noise and humanize conversations"
```

### Issue 2: Excessive trailing spaces
**Line:** 18
**Current:**
```
This feature adds light background sound to mimic a real-world environment, making your agent's voice sound more authentic and less "studio-perfect." It's useful when you want your conversations to feel natural and comfortable for the caller.       
```
**Change to:**
```
This feature adds light background sound to mimic a real-world environment, making your agent's voice sound more authentic and less "studio-perfect." It's useful when you want your conversations to feel natural and comfortable for the caller.
```

### Issue 3: Excessive trailing spaces
**Line:** 30
**Current:**
```
- **Soft Office Space:** Adds a gentler ambient noise for a natural but calm tone.      \
  Best for relaxed or friendly interactions like onboarding or sales calls.
```
**Change to:**
```
- **Soft Office Space:** Adds a gentler ambient noise for a natural but calm tone.\
  Best for relaxed or friendly interactions like onboarding or sales calls.
```

### Issue 4: Excessive trailing spaces
**Line:** 82
**Current:**
```
You define how a word should be pronounced using phonemes (sound-based syllables).   \
Phonely supports standard phonetic notation systems, such as MFA (Montreal Forced Aligner).
```
**Change to:**
```
You define how a word should be pronounced using phonemes (sound-based syllables).\
Phonely supports standard phonetic notation systems, such as MFA (Montreal Forced Aligner).
```

---

## 9. blocks/live-call-actions/api-request.mdx

### Issue 1: Excessive trailing spaces
**Line:** 17
**Current:**
```
You can connect it to any REST API using a cURL command or manual setup.       
```
**Change to:**
```
You can connect it to any REST API using a cURL command or manual setup.
```

### Issue 2: Excessive trailing spaces
**Line:** 27-29
**Current:**
```
2. In your Flow Editor, locate the block where the API call should occur, then click the ➕ (plus) icon directly beneath or next to it.       
3. In the popup menu, look under Live Call Actions.   
4. Select **API Request**. You'll see a new block added to your canvas labeled **API Request**.         
```
**Change to:**
```
2. In your Flow Editor, locate the block where the API call should occur, then click the ➕ (plus) icon directly beneath or next to it.
3. In the popup menu, look under Live Call Actions.
4. Select **API Request**. You'll see a new block added to your canvas labeled **API Request**.
```

### Issue 3: Excessive trailing spaces
**Line:** 60
**Current:**
```
If you don't have a cURL command, click **Build Manually**.                  \
You'll then define all settings step by step in the **Configure** tab.     
```
**Change to:**
```
If you don't have a cURL command, click **Build Manually**.\
You'll then define all settings step by step in the **Configure** tab.
```

### Issue 4: Excessive trailing spaces
**Line:** 66
**Current:**
```
The **Configure** tab is where you define what your API request should do.                            
```
**Change to:**
```
The **Configure** tab is where you define what your API request should do.
```

### Issue 5: Excessive trailing spaces
**Line:** 76-83
**Current:**
```
**1. API Method**

Select the type of request from the dropdown:                    

- `GET` – Retrieve data from a system.      
- `POST` – Send new data (most common).
- `PUT` or `PATCH` – Update an existing record.       
- `DELETE` – Remove a resource.

> Example: Choose **POST** when sending call data to an external app.        
```
**Change to:**
```
**1. API Method**

Select the type of request from the dropdown:

- `GET` – Retrieve data from a system.
- `POST` – Send new data (most common).
- `PUT` or `PATCH` – Update an existing record.
- `DELETE` – Remove a resource.

> Example: Choose **POST** when sending call data to an external app.
```

### Issue 6: Excessive trailing spaces
**Line:** 87
**Current:**
```
Enter the endpoint where the request should go. This is the destination for your data.                
```
**Change to:**
```
Enter the endpoint where the request should go. This is the destination for your data.
```

### Issue 7: Excessive trailing spaces
**Line:** 91
**Current:**
```
Headers define metadata or authentication details for your API call.                                                         Click **\+ Add** to add key-value pairs such as:                                                                                                 
```
**Change to:**
```
Headers define metadata or authentication details for your API call. Click **+ Add** to add key-value pairs such as:
```

### Issue 8: Excessive trailing spaces
**Line:** 106
**Current:**
```
Use this if your API uses query strings in the URL (e.g., filtering or pagination).

Example:    
```
**Change to:**
```
Use this if your API uses query strings in the URL (e.g., filtering or pagination).

Example:
```

### Issue 9: Excessive trailing spaces
**Line:** 117
**Current:**
```
Define what data will be sent.Switch between **Code** (for JSON) and **Raw** (for plain text).                     Example:      
```
**Change to:**
```
Define what data will be sent. Switch between **Code** (for JSON) and **Raw** (for plain text). Example:
```

### Issue 10: Excessive trailing spaces
**Line:** 133
**Current:**
```
Click to expand this section. These options help control the flow behavior during API communication.    
```
**Change to:**
```
Click to expand this section. These options help control the flow behavior during API communication.
```

### Issue 11: Excessive trailing spaces
**Line:** 150
**Current:**
```
Click **Continue** to save and move on to the **Test** step.     
```
**Change to:**
```
Click **Continue** to save and move on to the **Test** step.
```

### Issue 12: Excessive trailing spaces
**Line:** 156-158
**Current:**
```
1. Click **Test**.                 \
   Phonely will send the request exactly as you configured.    
2. The response will display instantly, showing whether it succeeded or failed.    
```
**Change to:**
```
1. Click **Test**.\
   Phonely will send the request exactly as you configured.
2. The response will display instantly, showing whether it succeeded or failed.
```

### Issue 13: Excessive trailing spaces
**Line:** 170
**Current:**
```
If failed, you'll get an error message explaining what went wrong (e.g., invalid URL, authentication error, or timeout).           
```
**Change to:**
```
If failed, you'll get an error message explaining what went wrong (e.g., invalid URL, authentication error, or timeout).
```

### Issue 14: Spelling error
**Line:** 172
**Current:**
```markdown
## Usecases for API Requests
```
**Change to:**
```markdown
## Use cases for API Requests
```

---

## 10. blocks/post-call-actions/post-call-overview.mdx

### Issue 1: Missing comma (grammar)
**Line:** 6
**Current:**
```
Post Call Actions are a powerful type of block that trigger specific automations after a phone conversation has concluded. Unlike Live Call Actions which happen in real-time during the call, Post Call Actions are designed to process and pass information once the call has finished.
```
**Change to:**
```
Post Call Actions are a powerful type of block that trigger specific automations after a phone conversation has concluded. Unlike Live Call Actions, which happen in real-time during the call, Post Call Actions are designed to process and pass information once the call has finished.
```

### Issue 2: Excessive trailing spaces
**Line:** 10
**Current:**
```
Post Call Actions are actions that are taken after a phone conversation is complete, and are extremely valuable for automating follow-ups, capturing comprehensive call data, and integrating with other systems without interrupting the live conversation.    
```
**Change to:**
```
Post Call Actions are actions that are taken after a phone conversation is complete, and are extremely valuable for automating follow-ups, capturing comprehensive call data, and integrating with other systems without interrupting the live conversation.
```

### Issue 3: Excessive trailing spaces
**Line:** 48-51
**Current:**
```
  <Step title="Select Action">
    A menu will pop up with a series of pre-built Post Call Action blocks (e.g., \"Send Email,\" \"Send Text Message,\" \"Zapier\"). Select the desired action.        
  </Step>
  <Step title="Configure & Connect:">
    Once added, configure the settings of the Post Call Action block and ensure it is connected to the appropriate node in your workflow. You will know that your Post Call Action has successfully connected if there is a dotted line connected to your previous block.     
```
**Change to:**
```
  <Step title="Select Action">
    A menu will pop up with a series of pre-built Post Call Action blocks (e.g., "Send Email," "Send Text Message," "Zapier"). Select the desired action.
  </Step>
  <Step title="Configure & Connect:">
    Once added, configure the settings of the Post Call Action block and ensure it is connected to the appropriate node in your workflow. You will know that your Post Call Action has successfully connected if there is a dotted line connected to your previous block.
```

### Issue 4: Excessive trailing spaces and formatting
**Line:** 61-63
**Current:**
```
**A Post Call Action is only triggered if the conversation successfully reaches the specific node to which that Post Call Action is attached.       **

**Example**: If you have a Post Call \"Send Text Message\" connected to a specific \"Appointment Confirmed\" block, the text message will only be sent after the call finishes AND the caller successfully navigated to and completed the \"Appointment Confirmed\" block.    
```
**Change to:**
```
**A Post Call Action is only triggered if the conversation successfully reaches the specific node to which that Post Call Action is attached.**

**Example**: If you have a Post Call "Send Text Message" connected to a specific "Appointment Confirmed" block, the text message will only be sent after the call finishes AND the caller successfully navigated to and completed the "Appointment Confirmed" block.
```

---

## 11. testing/ab-testing.mdx

### Issue 1: Multiple spelling errors
**Line:** 3
**Current:**
```yaml
description: "Learn how to run perfomance tests on your voice agents"
```
**Change to:**
```yaml
description: "Learn how to run performance tests on your voice agents"
```

### Issue 2: Spelling error
**Line:** 6
**Current:**
```
A/B testing (also called split testing) allows you to compare two versions of your voice agent to see which one perfoms better in the real worl.
```
**Change to:**
```
A/B testing (also called split testing) allows you to compare two versions of your voice agent to see which one performs better in the real world.
```

### Issue 3: Spelling error
**Line:** 31
**Current:**
```
- **Test Name:** Give your test a descrptive name that identifies what you're testing.\
```
**Change to:**
```
- **Test Name:** Give your test a descriptive name that identifies what you're testing.\
```

### Issue 4: Spelling error
**Line:** 33
**Current:**
```
- **Description:** Explain your test goal.\
  _Example:_ \"Evaluate whether a friendly voice style improves appointment confirmations.\"
```
**Change to:**
```
- **Description:** Explain your test goal.\
  _Example:_ "Evaluate whether a friendly voice style improves appointment confirmations."
```

### Issue 5: Excessive backslashes
**Line:** 31-34
**Current:**
```
- **Test Name:** Give your test a descrptive name that identifies what you're testing.\\\\\\\\\\\\n
  _Example:_ \"Friendly Voice vs Formal Voice – Support Line.\"
- **Description:** Explain your test goal.\\\\\\\\\\\\n
  _Example:_ \"Evaluate whether a friendly voice style improves appointment confirmations.\"
```
**Change to:**
```
- **Test Name:** Give your test a descriptive name that identifies what you're testing.\
  _Example:_ "Friendly Voice vs Formal Voice – Support Line."
- **Description:** Explain your test goal.\
  _Example:_ "Evaluate whether a friendly voice style improves appointment confirmations."
```

### Issue 6: Excessive backslashes
**Line:** 48-50
**Current:**
```
- **By Number of Calls:** Ends after a set number of test calls.\\\\\\\\\\\\n
  _Example:_ Stop after 1,000 calls routed to the test version.
```
**Change to:**
```
- **By Number of Calls:** Ends after a set number of test calls.\
  _Example:_ Stop after 1,000 calls routed to the test version.
```

### Issue 7: Spelling error
**Line:** 67
**Current:**
```
Evaluates success based on how the call ended.\\\\\\\\\\\\nUse this if you care about the _technical or behavioral outcome_ of the call.
```
**Change to:**
```
Evaluates success based on how the call ended.\
Use this if you care about the _technical or behavioral outcome_ of the call.
```

### Issue 8: Spelling error
**Line:** 82
**Current:**
```
- **Caller Responsed Positively** – Caller confirmed, agreed, or expressed satisfaction.
```
**Change to:**
```
- **Caller Responded Positively** – Caller confirmed, agreed, or expressed satisfaction.
```

### Issue 9: Spelling error
**Line:** 86
**Current:**
```
- **Caller Provided Knowlesdge** – Caller shared useful information (e.g., feedback, preferences).
```
**Change to:**
```
- **Caller Provided Knowledge** – Caller shared useful information (e.g., feedback, preferences).
```

### Issue 10: Spelling error
**Line:** 96
**Current:**
```
- **Call Endedded by Caller** – Caller hung up first.
```
**Change to:**
```
- **Call Ended by Caller** – Caller hung up first.
```

### Issue 11: Excessive backslashes
**Line:** 108
**Current:**
```
After setup, Phonely automatically duplicates your base agent into a **Test Agent**.\\\\\\\\\\\\nYou'll see a banner:
```
**Change to:**
```
After setup, Phonely automatically duplicates your base agent into a **Test Agent**.\
You'll see a banner:
```

### Issue 12: Spelling error
**Line:** 120
**Current:**
```
If you want to edit the exisiting Base Agent (the control version), select this option.
```
**Change to:**
```
If you want to edit the existing Base Agent (the control version), select this option.
```

### Issue 13: Excessive backslashes
**Line:** 126
**Current:**
```
Selecting this option opens the **Test Agent**, which is the duplicate created during setup.\\\\\\\\\\\\nYou'll see a banner reminding you:
```
**Change to:**
```
Selecting this option opens the **Test Agent**, which is the duplicate created during setup.\
You'll see a banner reminding you:
```

### Issue 14: Excessive backslashes
**Line:** 134
**Current:**
```
Only modify the specific variables you want to test.\\\\\\\\\\\\nAll other settings should remain identical to your Base Agent to ensure fair and reliable results.
```
**Change to:**
```
Only modify the specific variables you want to test.\
All other settings should remain identical to your Base Agent to ensure fair and reliable results.
```

### Issue 15: Excessive backslashes
**Line:** 154
**Current:**
```
If you want to remove a planned or completed test entirely, choose **Delete Test**.\\\\\\\\\\\\n(Tests already running cannot be deleted until they finish.)
```
**Change to:**
```
If you want to remove a planned or completed test entirely, choose **Delete Test**.\
(Tests already running cannot be deleted until they finish.)
```

---

## Summary Statistics

**Total Files with Issues:** 11
**Total Issues Found:** 60+

### Issue Breakdown:
- **Spelling Errors:** 15
- **Grammar Issues:** 3
- **Formatting Issues (excessive spaces/backslashes):** 35+
- **Unprofessional Elements:** 7

### Most Common Issues:
1. Excessive trailing spaces (appears in almost every file)
2. Excessive backslashes in markdown (testing/ab-testing.mdx)
3. Inappropriate bold formatting in headers (outboundcalling/createaoutboundcallingcampaign.mdx)
4. Spelling errors scattered throughout multiple files

---

## Recommended Action Plan

1. **High Priority:** Fix all spelling and grammar errors first
2. **Medium Priority:** Remove excessive trailing spaces and clean up formatting
3. **Low Priority:** Standardize header formatting (remove excessive bold)

All changes should be made in the **staging** branch of the repository.
