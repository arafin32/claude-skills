# Skill: Expense Categorizer

| Category | Business |
| Version | 1.0 |
| Author | Kamrul Arafin |
| Last Updated | 2026 |
| License | MIT |

---

## What it does

Automatically categorizes business or personal expenses, identifies tax-deductible items, and provides a summary for bookkeeping and tax purposes.

---

## How to use it

1. Copy the system prompt below
2. Paste it into Claude
3. List your expenses (date, amount, description)
4. Get a categorized expense report
5. Export for your accountant or bookkeeping system

### Time needed: 2-3 minutes

---

## System Prompt

```
You are a professional accountant and bookkeeper. Your job is to categorize expenses accurately and identify tax deductions.

When given a list of expenses, you will:
1. Categorize each expense by type (Office Supplies, Travel, Meals & Entertainment, etc.)
2. Assess whether each is tax-deductible (for US businesses)
3. Flag any questionable or borderline items
4. Provide a summary with total deductible and non-deductible amounts
5. Return the data in a clear table format

Format your response as a markdown table with columns:
| Date | Description | Amount | Category | Tax Deductible? | Notes |

Rules:
- For Meals & Entertainment: 50% deductible (with exceptions for certain events)
- For Travel: 100% deductible if business-related
- For gifts: $25 per person per year limit
- For home office: Deductible if dedicated workspace
- For vehicles: Deductible if business use only
- Be conservative with deductions (when in doubt, mark as "Consult CPA")
- Always include a summary line at the bottom

Example:
| 2024-01-15 | Laptop for work | $1,200 | Equipment | Yes | 100% deductible, depreciable asset |
| 2024-01-20 | Team lunch | $150 | Meals & Entertainment | Partial (50%) | Business meeting, 50% deductible |

Remember: This is guidance only. A CPA should review before filing taxes.
```

---

## Example Input

```
Here are my business expenses for Q1 2024:

- Jan 5: $150 - Starbucks coffee and meeting with client (lunch for two)
- Jan 12: $2,400 - Adobe Creative Cloud subscription (monthly)
- Jan 18: $85 - Uber to client meeting
- Jan 25: $450 - Home internet (dedicated office space)
- Feb 2: $1,200 - Office supplies from Staples
- Feb 14: $45 - LinkedIn Premium subscription
- Feb 28: $3,000 - Contractor payment for design work
- Mar 1: $200 - Conference ticket (industry event)
- Mar 10: $100 - Client birthday gift (bottle of wine)
- Mar 15: $60 - Domain renewal
- Mar 20: $500 - Office desk (new furniture)
```

## Example Output

| Date | Description | Amount | Category | Tax Deductible? | Notes |
|------|-------------|--------|----------|-----------------|-------|
| Jan 5 | Client meeting lunch | $150 | Meals & Entertainment | Partial (50%) | $75 deductible |
| Jan 12 | Adobe Creative Cloud | $2,400 | Software/Subscriptions | Yes | 100% deductible |
| Jan 18 | Uber to meeting | $85 | Travel | Yes | Business travel, 100% |
| Jan 25 | Home internet | $450 | Utilities | Partial | Only deductible portion of home office use (~30-40%) |
| Feb 2 | Office supplies | $1,200 | Office Supplies | Yes | 100% deductible |
| Feb 14 | LinkedIn Premium | $45 | Professional Development | Yes | 100% deductible |
| Feb 28 | Contract designer | $3,000 | Contractor Fees | Yes | 100% deductible, keep 1099 on file |
| Mar 1 | Conference ticket | $200 | Professional Development | Yes | 100% deductible if directly business-related |
| Mar 10 | Client gift | $100 | Business Gifts | No | Exceeds $25 limit; not deductible |
| Mar 15 | Domain renewal | $60 | Website/Domain | Yes | 100% deductible |
| Mar 20 | Office desk | $500 | Fixed Assets | Yes | Deductible but depreciable (7 year life) |

---

### Summary:
- **Total Expenses:** $8,190
- **Fully Deductible:** $7,160
- **Partially Deductible:** $485 (home internet $150-180, meal $75)
- **Not Deductible:** $100 (gift exceeds limit)
- **Estimated Tax Deductions:** ~$7,600-7,700

---

## Tips & Variations

### Customize for your situation:
- **Personal expenses:** Ask Claude to use personal categories (groceries, utilities, rent)
- **Different country:** Specify "Canadian tax rules" or "UK tax rules"
- **Specific business type:** "Self-employed consultant" or "LLC" has different rules
- **More detail:** Ask for "notes on depreciation" or "quarterly estimates"

### Make it more powerful:
- Add "Currency" column if you have international expenses
- Ask for "year-to-date summary" if running multiple months
- Request "cash flow impact" analysis
- Get "quarterly estimated tax" calculations

### Pro tips:
- Keep receipts for everything — the IRS may ask
- Get a CPA to review before filing
- Use this as a starting point, not final answer
- Track as you go (don't compile at tax time)
- Save in spreadsheet format for easy updates

---

## Common Issues

**Q: It's saying something is deductible, but I'm not sure**
A: Always consult a CPA. This is guidance only, not official tax advice.

**Q: It's categorizing things wrong**
A: Add more detail to the description (what it was for, who it was with, etc.)

**Q: I have expenses in different currencies**
A: Specify in the input: "All amounts in USD" or list currency per item

**Q: I want to know about depreciation**
A: Add to prompt: "Include depreciation schedules for fixed assets over X years"

---

## Related Skills

- [`invoice-analyzer.md`](../finance/invoice-analyzer.md) — Analyze vendor invoices
- [`budget-planner.md`](../finance/budget-planner.md) — Create and track budgets
- [`tax-deduction-finder.md`](../finance/tax-deduction-finder.md) — Find additional deductions

---

## Tags

#accounting #bookkeeping #taxpreparation #finance #deductions

---

## Important Notes

⚠️ **This is not professional tax or accounting advice.** Results should be reviewed by a qualified CPA or tax professional before filing taxes. Tax laws vary by:
- Country and state/province
- Business structure (sole proprietor, LLC, S-corp, C-corp)
- Industry
- Income level
- Special circumstances

Always consult a professional.
