# Claude Skills Library

A curated, open-source collection of specialized Claude prompts and workflows for different industries and use cases. Copy, fork, modify, and share freely.

**[Browse All Skills](#skills-by-category)** | **[How to Use](#quick-start)** | **[Contribute](#contribute)** | **[License](LICENSE)**

---

## 🚀 Quick Start

### Option 1: Copy a Single Skill (Fastest)
1. Browse the [`skills/`](skills/) directory
2. Open the `.md` file for the skill you want
3. Copy the **System Prompt** section
4. Paste it into Claude, ChatGPT, Gemini, or any LLM
5. Start using it

### Option 2: Fork the Entire Repo
```bash
git clone https://github.com/[your-username]/claude-skills.git
cd claude-skills
```
Then explore, use, modify, and contribute improvements.

### Option 3: Use in Claude Projects
1. In Claude.ai, create a new Project
2. Upload skill `.md` files or link this repo
3. Use skills directly in your project context

### Option 4: Add to Your Own LLM Setup
If you're using Claude via API or another LLM:
- Copy individual skill prompts
- Integrate into your application
- Modify as needed

### Option 5: Run the repo in Docker
Build and run the library in a container:
```bash
docker build -t claude-skills .
docker run --rm -p 8080:8080 claude-skills
```
Then open `http://localhost:8080` in your browser.

Or use Docker Compose:
```bash
docker compose up --build
```

---

## 📚 Skills by Category

### 💼 **Business & Operations**
- [`expense-categorizer.md`](skills/business/expense-categorizer.md) — Auto-categorize receipts and expenses
- [`meeting-summarizer.md`](skills/business/meeting-summarizer.md) — Extract action items and decisions from meetings

### ✍️ **Copywriting & Content**
- [`social-media-caption.md`](skills/copywriting/social-media-caption.md) — Create engaging social media captions
- [`blog-outline-generator.md`](skills/copywriting/blog-outline-generator.md) — Generate comprehensive blog outlines
- [`landing-page-copy.md`](skills/copywriting/landing-page-copy.md) — Write persuasive landing page copy

### 💰 **Finance & Accounting**
- [`invoice-analyzer.md`](skills/finance/invoice-analyzer.md) — Review and summarize invoices

### ⚖️ **Legal**
- [`contract-reviewer.md`](skills/legal/contract-reviewer.md) — Identify risks and key terms in contracts

### 🛒 **E-commerce**
- [`product-description-writer.md`](skills/ecommerce/product-description-writer.md) — Write compelling product descriptions

### 👥 **HR & Recruiting**
- [`resume-screener.md`](skills/hr/resume-screener.md) — Screen and rank resumes by job fit

### 🎯 **Marketing & SEO**
- [`keyword-researcher.md`](skills/marketing/keyword-researcher.md) — Research high-intent keywords

### 💻 **Development**
- [`code-reviewer.md`](skills/development/code-reviewer.md) — Review code for quality and security

> The `skills/realestate/` and `skills/other/` folders are ready for new skill contributions.

---

## 📖 How to Use a Skill

Each skill file has this structure:

```markdown
# Skill: [Name]

**Category:** [Category]
**Version:** 1.0
**Author:** [Creator]
**License:** MIT

## What it does
[Clear description of what the skill does]

## How to use it
[Step-by-step instructions]

## System Prompt
[The actual prompt to copy and paste]

## Example Input
[Real example of what to input]

## Example Output
[Real example of expected output]

## Tips & Variations
[Ways to customize and improve results]

## Tags
[Searchable tags]
```

### Pro Tips:
- **Customize the prompt** — Change tone, style, output format to match your needs
- **Combine skills** — Use output from one skill as input to another
- **Iterate** — If results aren't perfect, refine your input and try again
- **Test variations** — Most skills have multiple variants in the Tips section

---

## 🤝 Contribute

This is a community project. We need YOUR skills!

### How to Add a Skill

1. **Fork the repo**
   ```bash
   git clone https://github.com/[your-username]/claude-skills.git
   cd claude-skills
   git checkout -b add-[skill-name]
   ```

2. **Create your skill file**
   - Use the template: [`SKILL_TEMPLATE.md`](SKILL_TEMPLATE.md)
   - Place it in the appropriate category folder under `skills/`
   - Filename format: `kebab-case.md`

3. **Test your skill**
   - Copy the system prompt
   - Test it in Claude or another LLM
   - Refine until it works well
   - Add real examples

4. **Commit and push**
   ```bash
   git add skills/[category]/[skill-name].md
   git commit -m "Add [skill-name] skill for [category]"
   git push origin add-[skill-name]
   ```

5. **Open a Pull Request**
   - Describe what the skill does
   - Include a use case example
   - Link to any related skills

### Quality Standards

To be merged, skills should:
- ✅ Have a clear, tested system prompt
- ✅ Include working examples (input + output)
- ✅ Be useful for a real audience
- ✅ Have proper formatting and documentation
- ✅ Be original or significantly improved
- ✅ Include author attribution

### Questions or Ideas?

- **Request a skill:** Open an Issue with the label `skill-request`
- **Report a problem:** Open an Issue with details and which skill
- **Discuss ideas:** Use the Discussions tab
- **Share results:** Show us what you built with these skills!

---

## 📊 Stats

- **Skills:** 10 production-ready skills
- **Categories:** 8 active categories
- **Contributors:** Community-driven
- **License:** MIT (free to use, modify, distribute)

---

## 🏆 Contributing Guidelines

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for detailed contribution guidelines.

---

## 📄 License

All skills in this repository are licensed under the MIT License. See [`LICENSE`](LICENSE) for details.

**TL;DR:** You can use, modify, and distribute these skills freely, even commercially. Just include a license notice.

---

## 🌟 Star This Repo!

If you find these skills useful, please star the repository! It helps others discover them and motivates community contributions.

---

## 🔗 Resources

- **Claude Docs:** [https://claude.ai](https://claude.ai)
- **Claude API:** [https://docs.anthropic.com](https://docs.anthropic.com)
- **Tips for Better Prompts:** [Anthropic Prompt Guide](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)

---

## ❓ FAQ

**Q: Can I use these skills commercially?**
A: Yes! The MIT license allows commercial use. Just include the license notice.

**Q: Can I modify the skills?**
A: Absolutely. Customize them for your needs.

**Q: Do I need an API key?**
A: Only if you're using Claude via API. You can also paste prompts into Claude.ai directly.

**Q: Can I add my own skills?**
A: Yes! Follow the contribution guidelines above.

**Q: Which LLM can I use these with?**
A: These are designed for Claude, but most work with ChatGPT, Gemini, and other LLMs. Results may vary.

---

**Made with ❤️ by the community. Fork, improve, and share!**
