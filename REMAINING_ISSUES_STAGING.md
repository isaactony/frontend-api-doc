# Remaining Issues in Staging Branch

After reviewing the current state of the staging branch, here are the issues that still need to be fixed:

---

## 1. docs.json

### ✅ FIXED: "Agent Guildelines" → "Agent Guidelines"
### ✅ FIXED: Extra space before "AGENT KNOWLEDGEBASE"

**Status:** All issues in docs.json have been fixed.

---

## 2. get-started/overview.mdx

### ✅ FIXED: "Phonel" → "Phonely" in description

**Status:** All issues fixed.

---

## 3. get-started/quick-start.mdx

### ✅ FIXED: "repeatibly" → "repeatedly"
### ✅ FIXED: Excessive trailing spaces

**Status:** All issues fixed.

---

## 4. get-started/dashboard-overview.mdx

### ❌ STILL NEEDS FIX: Line 96
**Current:**
```markdown
- A sudden drop in bound calls might indicate routing issues or downtime.
```

**Should be:**
```markdown
- A sudden drop in outbound calls might indicate routing issues or downtime.
```

**Issue:** Missing "out" prefix - should be "outbound calls" not "bound calls"

---

## 5. key-concepts/flows.mdx

### ✅ FIXED: Excessive spacing and periods
### ✅ FIXED: Escape characters in plus signs
### ✅ FIXED: "trasnfers" → "transfers"

**Status:** All issues fixed.

---

## 6. key-concepts/variables.mdx

### ✅ FIXED: "ive vs. post-call actions" → "Live vs. post-call actions"

**Status:** All issues fixed.

---

## 7. outboundcalling/createaoutboundcallingcampaign.mdx

### ❌ STILL NEEDS FIX: Line 17-19 - Inappropriate callout type
**Current:**
```mdx
<Danger>
  Campaigns support both batch calling for large lead uploads and \*\*continuous \*\*mode for real-time outreach as new leads sync from your CRM.
</Danger>
```

**Should be:**
```mdx
<Info>
  Campaigns support both **batch** calling for large lead uploads and **continuous** mode for real-time outreach as new leads sync from your CRM.
</Info>
```

**Issues:** 
- Using `<Danger>` for informational content (should be `<Info>`)
- Extra spaces in bold formatting: `\*\*continuous \*\*` should be `**continuous**`

---

### ❌ STILL NEEDS FIX: Line 21 - Excessive trailing spaces
**Current:**
```markdown
Once configured, the system can automatically call new leads as they appear or process static lists of contacts in defined batches. The campaign setup process is divided into structured steps to ensure accuracy and compliance.                     
```

**Should be:**
```markdown
Once configured, the system can automatically call new leads as they appear or process static lists of contacts in defined batches. The campaign setup process is divided into structured steps to ensure accuracy and compliance.
```

**Issue:** 21 excessive trailing spaces at end of line

---

### ❌ STILL NEEDS FIX: Line 27 - Excessive bold formatting
**Current:**
```markdown
### **Campaign Name**
```

**Should be:**
```markdown
### Campaign Name
```

**Issue:** Unnecessary bold formatting on header

---

### ❌ STILL NEEDS FIX: Line 35 - Excessive bold formatting
**Current:**
```markdown
### **Campaign Use Cases**
```

**Should be:**
```markdown
### Campaign Use Cases
```

**Issue:** Unnecessary bold formatting on header

---

### ❌ STILL NEEDS FIX: Line 53 - Excessive bold formatting
**Current:**
```markdown
### **Connecting Twilio**
```

**Should be:**
```markdown
### Connecting Twilio
```

**Issue:** Unnecessary bold formatting on header

---

### ❌ STILL NEEDS FIX: Line 73 - Excessive trailing spaces
**Current:**
```markdown
3. **Country-Based Routing** – Used for international outreach.\
   Calls are routed through numbers assigned to the recipient's country, preserving a local presence and helping with compliance in regions where cross-border calls may be restricted.     \
   As with state-based routing, if no local number exists, Phonely falls back to a random enabled number.
```

**Should be:**
```markdown
3. **Country-Based Routing** – Used for international outreach.\
   Calls are routed through numbers assigned to the recipient's country, preserving a local presence and helping with compliance in regions where cross-border calls may be restricted.\
   As with state-based routing, if no local number exists, Phonely falls back to a random enabled number.
```

**Issue:** 5 excessive trailing spaces before line break

---

### ❌ STILL NEEDS FIX: Multiple headers with excessive bold formatting

**Lines with issues:**
- Line 86: `**Calls per Hour**` → should be `### Calls per Hour`
- Line 98: `**Campaign Type: Continuous vs Batch**` → should be `### Campaign Type: Continuous vs Batch`
- Line 108: `### **Trigger Sources**` → should be `### Trigger Sources`
- Line 169: `### **Selecting or Editing a Flow**` → should be `### Selecting or Editing a Flow`
- Line 175: `### **Mapping Variables**` → should be `### Mapping Variables`

---

## 8. agent-design/voice/voice-and-personality.mdx

### ✅ FIXED: "coversations" → "conversations" in description

### ❌ STILL NEEDS FIX: Line 60 - Excessive trailing spaces
**Current:**
```markdown
- **Soft Office Space:** Adds a gentler ambient noise for a natural but calm tone.      \
  Best for relaxed or friendly interactions like onboarding or sales calls.
```

**Should be:**
```markdown
- **Soft Office Space:** Adds a gentler ambient noise for a natural but calm tone.\
  Best for relaxed or friendly interactions like onboarding or sales calls.
```

**Issue:** 6 excessive trailing spaces before line break

---

### ❌ STILL NEEDS FIX: Line 82 - Excessive trailing spaces
**Current:**
```markdown
You define how a word should be pronounced using phonemes (sound-based syllables).   \
Phonely supports standard phonetic notation systems, such as MFA (Montreal Forced Aligner).
```

**Should be:**
```markdown
You define how a word should be pronounced using phonemes (sound-based syllables).\
Phonely supports standard phonetic notation systems, such as MFA (Montreal Forced Aligner).
```

**Issue:** 3 excessive trailing spaces before line break

---

## 9. blocks/live-call-actions/api-request.mdx

### ❌ STILL NEEDS FIX: Line 69 - Excessive trailing spaces and missing space
**Current:**
```markdown
Headers define metadata or authentication details for your API call.                                                         Click **\+ Add** to add key-value pairs such as:
```

**Should be:**
```markdown
Headers define metadata or authentication details for your API call. Click **+ Add** to add key-value pairs such as:
```

**Issues:** 
- 57 excessive trailing spaces between sentences
- Escape character in `\+` should be just `+`

---

### ❌ STILL NEEDS FIX: Line 90 - Missing space and excessive trailing spaces
**Current:**
```markdown
Define what data will be sent.Switch between **Code** (for JSON) and **Raw** (for plain text).                     Example:
```

**Should be:**
```markdown
Define what data will be sent. Switch between **Code** (for JSON) and **Raw** (for plain text). Example:
```

**Issues:**
- Missing space after period: "sent.Switch" should be "sent. Switch"
- 21 excessive trailing spaces before "Example:"

---

### ❌ STILL NEEDS FIX: Line 135 - Spelling/Capitalization Error
**Current:**
```markdown
## Use cases for API Requests
```

**Should be:**
```markdown
## Use cases for API Requests
```

**Issue:** "Usecases" should be two words "Use cases" (appears to be fixed already based on reading)

---

## 10. blocks/post-call-actions/post-call-overview.mdx

### ✅ FIXED: Missing comma in "Unlike Live Call Actions, which happen"
### ✅ FIXED: Excessive trailing spaces

**Status:** All issues fixed.

---

## 11. testing/ab-testing.mdx

### ❌ STILL NEEDS FIX: Line 3 - Spelling error in description
**Current:**
```yaml
description: "Description of your new file."
```

**Should be:**
```yaml
description: "Learn how to run performance tests on your voice agents"
```

**Issue:** Generic placeholder description instead of proper description

---

### ❌ STILL NEEDS FIX: Line 6 - Multiple issues
**Current:**
```markdown
Phonely's A/B Testing tool helps you experiment, measure, and improve your voice AI's performance with real world data . It allows you to compare different versions of you AI agent such as Voice, workflow, conversation settings to determine which one performs best in live calls.
```

**Should be:**
```markdown
Phonely's A/B Testing tool helps you **experiment**, measure, and improve your voice AI's performance with real world data. It allows you to compare different versions of your AI agent such as Voice, workflow, conversation settings to determine which one performs best in live calls.
```

**Issues:**
- Missing bold on "experiment"
- Extra space before period: "data ." should be "data."
- "you AI" should be "your AI"

---

### ❌ STILL NEEDS FIX: Line 31 - Spelling error
**Current:**
```markdown
Give your test a descrptive name that identifies what you're testing.\
```

**Should be:**
```markdown
Give your test a descriptive name that identifies what you're testing.\
```

**Issue:** "descrptive" → "descriptive"

---

### ❌ STILL NEEDS FIX: Line 33 - Excessive trailing spaces
**Current:**
```markdown
Add a description to explain the goal of your test.                                                        \
```

**Should be:**
```markdown
Add a description to explain the goal of your test.\
```

**Issue:** 56 excessive trailing spaces before line break

---

### ❌ STILL NEEDS FIX: Line 55 - Spelling error
**Current:**
```markdown
| **Knowledge Base** | Tests different documentation sources                            | See which knowledge sources improve the accuracy of the the answers |
```

**Should be:**
```markdown
| **Knowledge Base** | Tests different documentation sources                            | See which knowledge sources improve the accuracy of the answers |
```

**Issue:** Duplicate word "the the" should be just "the"

---

### ❌ STILL NEEDS FIX: Line 82 - Spelling error
**Current:**
```markdown
Evaluates success based on how the call ended. Use this if you care about the technical or behavioral outcome of the call.
```

**Should be:**
```markdown
Evaluates success based on how the call ended.\
Use this if you care about the _technical or behavioral outcome_ of the call.
```

**Issue:** Should have line break and italics for consistency with other sections

---

### ❌ STILL NEEDS FIX: Line 102 - Spelling error
**Current:**
```markdown
  - Agent Endedded
```

**Should be:**
```markdown
  - Agent Ended
```

**Issue:** "Endedded" → "Ended"

---

## 12. blocks/flow-blocks/collect.mdx

### ✅ FIXED: "Setup  - Two Ways" → "Setup - Two Ways"

**Status:** All issues fixed.

---

## Summary of Remaining Issues

**Total Remaining Issues: 24**

### By File:
1. **get-started/dashboard-overview.mdx** - 1 issue
2. **outboundcalling/createaoutboundcallingcampaign.mdx** - 10 issues
3. **agent-design/voice/voice-and-personality.mdx** - 2 issues
4. **blocks/live-call-actions/api-request.mdx** - 3 issues
5. **testing/ab-testing.mdx** - 8 issues

### By Type:
- **Spelling errors:** 5
- **Grammar errors:** 2
- **Formatting issues (excessive spaces):** 8
- **Unprofessional elements (bold headers, wrong callouts):** 9

### Priority:
**HIGH PRIORITY (User-Facing):**
- Spelling errors in testing/ab-testing.mdx
- Wrong callout type in outboundcalling file
- "bound calls" → "outbound calls" in dashboard-overview.mdx

**MEDIUM PRIORITY (Formatting):**
- Excessive trailing spaces
- Excessive bold formatting in headers

---

## Files That Are Fully Fixed:
✅ docs.json
✅ get-started/overview.mdx
✅ get-started/quick-start.mdx
✅ key-concepts/flows.mdx
✅ key-concepts/variables.mdx
✅ blocks/post-call-actions/post-call-overview.mdx
✅ blocks/flow-blocks/collect.mdx
