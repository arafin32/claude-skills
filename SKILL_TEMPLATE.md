# Skill: [Skill Name Here]

**Category:** [Business, Copywriting, Finance, Legal, Real Estate, E-commerce, HR, Marketing, Development, etc.]
**Version:** 1.0
**Author:** [Your Name / GitHub Handle]
**Last Updated:** [Date]
**License:** MIT

---

## What it does

[Clear, concise description of what this skill does. 1-3 sentences explaining the primary use case and outcome.]

**Example:** This skill takes a list of business expenses and automatically categorizes them by type, helping with bookkeeping and tax preparation.

---

## How to use it

[Step-by-step instructions for using this skill. Make it easy for someone who's never used it before.]

### Steps:
1. Copy the system prompt below
2. Paste it into Claude or your LLM of choice
3. Provide the input (e.g., "Here's my expense list...")
4. Get your output and refine as needed

### Parameters:
- **Input format:** [Describe what format the user should provide data in]
- **Output format:** [Describe what you'll get back]
- **Time to complete:** [Estimated time needed, e.g., "30 seconds"]

---

## System Prompt

Copy everything between the dashed lines and paste into Claude:

---

```
[Your system prompt goes here. Be specific about:
- What role Claude should take (e.g., "You are a financial analyst")
- What the task is (e.g., "Categorize the following expenses")
- How to format the output (e.g., "Return as a table with columns: Date, Amount, Category, Notes")
- Any specific rules or guidelines (e.g., "Be conservative with tax deduction claims")
- Edge cases to handle (e.g., "If amount is unclear, ask for clarification")
- Tone and style (e.g., "Be professional but friendly")]
```

---

## Example Input

```
Here are my business expenses for Q1 2024:

- Jan 5: $150 - Starbucks coffee and meeting with client
- Jan 12: $2,400 - Monthly software subscription (QuickBooks)
- Jan 18: $85 - Uber to meeting
- Feb 2: $1,200 - Office supplies from Staples
- Feb 14: $45 - LinkedIn Premium
- Feb 28: $3,000 - Contractor payment for design work
- Mar 10: $200 - Conference ticket
- Mar 15: $60 - Domain renewal
```

## Example Output

| Date | Amount | Category | Notes | Tax Deductible? |
|------|--------|----------|-------|-----------------|
| Jan 5 | $150 | Meals & Entertainment | Client meeting | Partial (50%) |
| Jan 12 | $2,400 | Software | Business software | Yes |
| Jan 18 | $85 | Travel | Meeting transportation | Yes |
| Feb 2 | $1,200 | Office Supplies | Supplies | Yes |
| Feb 14 | $45 | Professional Development | Membership | Yes |
| Feb 28 | $3,000 | Contractors | Design services | Yes |
| Mar 10 | $200 | Professional Development | Conference | Yes |
| Mar 15 | $60 | Website | Domain | Yes |
| **Total** | **$7,140** | | | **~$6,915** |

---

## Tips & Variations

### Customize it:
- **Change the tone** — Make it more casual, formal, or humorous
- **Change the output format** — Get CSV, JSON, bullet points, or narrative summary instead
- **Add rules** — Specify your company's expense policies
- **Expand categories** — Add custom categories relevant to your business

### Example variations:

**Variation 1: Personal Expense Tracker**
Change the system prompt to use consumer categories (groceries, utilities, rent) instead of business categories.

**Variation 2: Multi-Currency Support**
Add: "If amounts are in different currencies, convert to USD using current rates."

**Variation 3: Suspicious Activity Detection**
Add: "Flag any expenses that seem unusual or potentially fraudulent."

---

## Common Issues

**Q: The output format isn't what I want**
A: Modify the system prompt to specify exactly what format you need (table, JSON, CSV, bullet points, etc.)

**Q: It's categorizing things wrong**
A: Add more detail to your input or clarify the rules in the system prompt.

**Q: It's not recognizing certain expenses**
A: Provide more context (e.g., "Starbucks is a meals & entertainment expense for client meetings")

---

## Related Skills

- [Other related skill 1](path/to/skill)
- [Other related skill 2](path/to/skill)

---

## Tags

#[tag1] #[tag2] #[tag3] #[tag4]

**Example:** #finance #accounting #automation #bookkeeping

---

## Notes

- [Any important notes or disclaimers]
- [When this skill works best]
- [When you might need human review]

**Example:**
- This is not professional accounting advice. Consult a tax professional.
- Works best with clear, detailed expense descriptions
- Should be reviewed by a human accountant for tax purposes
- Best for personal finance or small business use
