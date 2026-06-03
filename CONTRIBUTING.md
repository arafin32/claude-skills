# Contributing to Claude Skills

Thanks for wanting to contribute! We welcome skills, improvements, bug reports, and feedback from everyone.

---

## How to Contribute

### 1. **Add a New Skill**

The most valuable contribution is a new skill.

**Steps:**

1. **Fork the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/claude-skills.git
   cd claude-skills
   git checkout -b add-skill/your-skill-name
   ```

2. **Create your skill file**
   - Copy [`SKILL_TEMPLATE.md`](SKILL_TEMPLATE.md) as a reference
   - Create a new file in the appropriate category folder: `skills/[category]/[skill-name].md`
   - Use kebab-case for filenames: `my-awesome-skill.md`
   - Folder must exist (see list below) or create it

3. **Test thoroughly**
   - Copy the system prompt from your file
   - Paste it into Claude.ai or your LLM
   - Test with the example input
   - Verify the output matches your example
   - Try variations and edge cases
   - Refine the prompt until it works reliably

4. **Document clearly**
   - Clear description of what it does
   - Step-by-step usage instructions
   - Real working examples (input + output)
   - Tips for customization
   - Be concise but complete

5. **Commit with a clear message**
   ```bash
   git add skills/[category]/[skill-name].md
   git commit -m "Add [skill-name]: [brief description]"
   ```

6. **Push and create a Pull Request**
   ```bash
   git push origin add-skill/your-skill-name
   ```
   - Go to GitHub and open a PR
   - Include in the description:
     - What the skill does
     - What problem it solves
     - Any relevant use cases
     - Who would benefit from it

### 2. **Improve an Existing Skill**

Found a way to make a skill better? Suggest improvements!

```bash
git checkout -b improve/skill-name
# Edit the skill file
git commit -m "Improve [skill-name]: [what you improved]"
git push origin improve/skill-name
# Open a PR
```

### 3. **Report Issues**

Found a bug or problem with a skill?

1. Go to **Issues** tab
2. Click **New Issue**
3. Include:
   - Which skill has the problem
   - What you expected vs. what happened
   - The exact input you used
   - The output you got
   - Your LLM (Claude, ChatGPT, etc.)

### 4. **Request a Skill**

Know of a useful skill that doesn't exist yet?

1. Go to **Issues** tab
2. Click **New Issue**
3. Title: `Skill Request: [Skill Name]`
4. Include:
   - What the skill would do
   - Who would use it
   - Why it's valuable
   - Example input/output if you can

### 5. **Share Results**

Show the community what you built!

1. Go to **Discussions** tab
2. Share:
   - What skills you used
   - What you built
   - Results/outcomes
   - Tips you learned
   - Before/after examples

---

## Skill Categories

Skills should go in one of these folders. Create a new category folder if needed:

- `skills/business/` — Business operations, management, administrative tasks
- `skills/copywriting/` — Writing, content creation, marketing copy
- `skills/development/` — Code, APIs, technical documentation
- `skills/ecommerce/` — E-commerce, products, sales
- `skills/finance/` — Accounting, budgeting, financial analysis
- `skills/hr/` — HR, recruiting, interviews, hiring
- `skills/legal/` — Contracts, legal documents, compliance
- `skills/marketing/` — SEO, email marketing, strategy
- `skills/realestate/` — Real estate, property, listings
- `skills/other/` — Anything that doesn't fit above

---

## Skill Quality Checklist

Before submitting a PR, make sure your skill:

- [ ] **Has a clear system prompt** — Specific, testable, well-written
- [ ] **Has been tested** — Works reliably in Claude or another LLM
- [ ] **Has real examples** — Both input and output are realistic and useful
- [ ] **Is well-documented** — Anyone can understand how to use it
- [ ] **Has a clear use case** — Solves a real problem for real people
- [ ] **Follows the template** — Formatted correctly with all sections
- [ ] **Is original or improved** — Not just copying existing skills
- [ ] **Includes author credit** — Your name/GitHub handle for attribution
- [ ] **Has appropriate tags** — 3-5 searchable hashtags

---

## Writing a Good System Prompt

The quality of the skill depends on the quality of the system prompt. Here's how to write a good one:

### Include:
- **Role:** "You are a..."
- **Task:** "Your job is to..."
- **Format:** "Return the output as..." (table, JSON, bullet points, etc.)
- **Rules:** Any specific guidelines or constraints
- **Examples:** If helpful, include an example in the prompt
- **Tone:** "Be professional," "Be conversational," etc.

### Example:
```
You are an expert financial analyst. Your job is to review invoices and summarize the key information.

For each invoice, extract and return:
1. Invoice number
2. Vendor name
3. Total amount
4. Due date
5. Description of services/products
6. Any unusual terms or discrepancies

Format your response as a markdown table. Be concise but thorough.
```

### Don't:
- ❌ Make it too vague ("help me with stuff")
- ❌ Make it too long (if over 500 words, it's probably too detailed)
- ❌ Include personal information or sensitive data in examples
- ❌ Make unrealistic promises ("100% accurate")

---

## PR Review Process

1. **You submit a PR** with your skill
2. **We review** for:
   - Quality of the system prompt
   - Clarity of documentation
   - Working examples
   - Realistic use case
   - Proper formatting
3. **We may suggest changes** — We'll work with you to improve it
4. **Once approved, we merge** — Your skill goes live!

---

## Getting Help

- **Questions about contributing?** Open an Issue with the label `question`
- **Need feedback on your skill before submitting?** Post in Discussions
- **Not sure about something?** Ask in an Issue — we'll help!

---

## Code of Conduct

Be respectful, inclusive, and constructive. We don't tolerate:
- Harassment or discrimination
- Spam or low-effort contributions
- Plagiarism
- Content that violates laws or platform policies

---

## Attribution & Credit

All contributors get credit! When your skill is merged:
- Your name appears as the author in the skill file
- You're listed in the main README (coming soon)
- Your GitHub profile is linked

---

## License

All contributions are licensed under the MIT License. By contributing, you agree that your contribution can be used and modified under the MIT License.

---

## Questions?

Open an issue or start a discussion. We're here to help!

**Thank you for contributing to Claude Skills! 🙏**
