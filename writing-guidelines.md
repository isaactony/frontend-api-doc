# Documentation Writing Guidelines

This guide provides essential patterns and best practices for creating effective Phonely documentation.

## Writing Style

### Voice and Tone
- **Conversational yet professional** - Write as if speaking to a knowledgeable colleague
- **Clear and direct** - Avoid jargon and complex sentences
- **Consistent terminology** - Use "workflow" not "flow" throughout

### Effective Openings
**✅ Use:**
- "In this guide, we'll introduce you to..."
- "The [Block Name] serves as a vital tool for..."
- Provide context and explain why the topic matters
- Use clear, accessible language

**❌ Don't:**
- Start with generic introductions without context
- Use overly technical language upfront

## Page Structure

### Title and Headlines
**✅ Start with introduction, then main content:**
```mdx
---
title: "Call History and Analytics"
description: "Brief description"
---

In this guide, we'll introduce you to...

The **Call History and Analytics** serves as a vital tool for...
```

**✅ Use clean titles without "in Phonely"** - It's redundant since all docs are about Phonely

### Headline Guidelines
- **H1**: Page title only (start content directly after introduction)
- **H2**: Main sections (2-5 per page)
- **H3**: Subsections (use sparingly - maximum 3-4 per page)
- **H4+**: Use bolded bullet points instead

**Headline Best Practices:**
- **Limit H1, H2 and H3 headlines** - Too many create clutter in the overview bar
- **Use lists instead** - Convert multiple related H3s to bullet points or Properties components
- **Group related content** - Combine similar subsections under single H2s

**✅ Headline Best Practices:**
- Don't repeat information from the page title or previous content
- Use action-oriented language when possible
- Focus on what the section covers, not what it's called
- Keep headlines descriptive and clear

**❌ Don't:**
- Repeat the page title as an H1 headline
- Use headlines beyond H3 (H4, H5, H6)
- Create headlines that repeat information already stated
- Include redundant information from the page context

**✅ Example:**
```mdx
## Main Section

**Key Point 1** - Description of the key point
**Key Point 2** - Another important point

1. **Step Title** - Description of the step
2. **Next Step** - Description of the next step
```

## Essential Components

### Cards
```mdx
<Card title="Title" icon="icon">
  Content
</Card>

<CardGroup cols={2}>
  <Card title="Title 1" icon="icon1">Content 1</Card>
  <Card title="Title 2" icon="icon2">Content 2</Card>
</CardGroup>
```

### Callouts
```mdx
<Callout type="info">
  Important information
</Callout>

<Tip>
  Helpful tip
</Tip>
```

### Steps
```mdx
<Steps>
  <Step stepNumber={1} title="Step Title">
    Step description
  </Step>
  <Step stepNumber={2} title="Next Step">
    Next step description
  </Step>
</Steps>
```

### Video Embeds
**Place videos right above the first ## headline, below the introductory paragraph:**
```mdx
In this guide, we'll introduce you to Phonely's powerful features that help you manage and optimize your call outcomes.

<div class="responsive-iframe-container">
  <iframe src="https://www.youtube.com/embed/VIDEO_ID" title="Video Title" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

## Key Features

Content starts here...
```

**❌ Don't:**
- Use direct YouTube links instead of embeds
- Place videos at the end of pages
- Create ## Introduction sections (jump straight into content)

### Properties
**❌ Avoid using Properties component** - It doesn't display properly in Mintlify. Use bold bullet points instead:

```mdx
**Property Name** (type) - Description of the property
```

**✅ Better format:**
```mdx
**variable_name** (string) - Description of the variable
- **another_property** (number) - Another property description
```

### Tabs
```mdx
<Tabs>
  <Tab title="Scenario 1">
    Content for scenario 1
  </Tab>
  <Tab title="Scenario 2">
    Content for scenario 2
  </Tab>
</Tabs>
```

## Formatting

### Bold Text
**✅ Use bold for UI elements and key concepts:**
```mdx
Click <b>Edit</b> to modify the settings
The <b>Send Email Block</b> is a vital tool
```

### Lists
**✅ Numbered lists for procedures:**
```mdx
1. **Step Title**
   - Sub-step description
   - Another sub-step

2. **Next Step**
   - Description
```

**✅ Bullet points for features:**
```mdx
- **Feature 1**: Description
- **Feature 2**: Description
```

### Code
**✅ Inline code for variables:**
```mdx
Use the <code>caller_name</code> variable in your email template
```

### Punctuation
**✅ Restructure sentences to avoid complex punctuation:**
```mdx
❌ "The agent asks for the name and then proceeds to book - no extra Talk block required."
✅ "The agent asks for the name and then proceeds to book without requiring an extra Talk block."
```

## Writing Patterns

### Feature Descriptions
**Pattern:** Action verb + benefit
```mdx
**Automated Email Dispatch**: Sends emails automatically from your Phonely agent to a specified recipient.
```

### Step Instructions
**Pattern:** Action + Context + Expected Result
```mdx
1. Access the Workflows Page from your Phonely Dashboard.
2. Create a New Flow, or select an existing one to edit.
3. Ensure a Trigger Condition is Set: Define a trigger for your workflow.
```

### Examples
**Pattern:** Scenario + Setup + Implementation + Result
```mdx
**Example**: If asking for a state, you can set a custom type to ensure the output is saved as a two-digit code (e.g., "WI" for Wisconsin, "GA" for Georgia) instead of the full state name.
```

## Common Page Structure

```mdx
---
title: "Page Title"
description: "Brief description"
---

In this guide, we'll introduce you to Phonely's powerful features that help you manage and optimize your call outcomes.

[Optional: Video embed here]

## Key Features

1. **Feature Name**: Description of the feature
2. **Feature Name**: Description of the feature

## How to Use

<Steps>
  <Step stepNumber={1} title="Step Title">
    Step description
  </Step>
</Steps>

## Example Use Case

**Scenario**: Detailed example with specific scenarios

## Best Practices

- **Practice 1** - Description
- **Practice 2** - Description

## Conclusion

Summary paragraph emphasizing value and next steps.
```

## Best Practices

1. **Keep HTML tags on single lines** - Prevents MDX parsing errors
2. **Use consistent terminology** - Stick to established terms like "workflow"
3. **Provide context for new concepts** - Explain terms and concepts clearly
4. **Include practical examples** - Always show real-world usage
5. **Test changes locally** - Always preview changes before committing
6. **Format internal links correctly** - Use `page-name` not `/docs/page-name`
7. **Limit headline depth** - Avoid H4+ headlines, use lists instead

## Critical Don'ts

**❌ Don't:**
- Split HTML tags across lines (causes MDX parsing errors)
- Use inconsistent terminology (e.g., "workflow" vs "flow")
- Skip examples (always show practical usage)
- Forget to test locally before committing
- Use `/docs/` prefix in internal links
- Create too many H3 headlines (clutters overview bar)
- Use H4+ headlines (use lists instead)
- Use em dashes (—) - restructure sentences to avoid needing such punctuation
- Use Properties component - it doesn't display properly, use bold bullet points instead

## Testing

Always test your changes locally:
```bash
mintlify dev
```

Check for:
- Component rendering issues
- Parsing errors in the console
- Visual layout problems
- Broken links or references

## File Organization

- **Use kebab-case filenames** - `call-history-analytics.mdx` not `call_history_analytics.mdx`
- **Group related content** - Keep similar topics together
- **Clean up unused files** - Delete files after refactoring

## Summary

The key to effective Phonely documentation:
1. **Use conversational, helpful tone** - Write for humans, not machines
2. **Follow established patterns** - Consistency builds trust
3. **Provide practical examples** - Show, don't just tell
4. **Structure logically** - Clear hierarchy and flow
5. **Test everything locally** - Catch issues before they go live