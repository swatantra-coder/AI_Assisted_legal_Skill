# Legal Assistant Skill for Claude Code

A comprehensive Claude Code skill designed specifically for lawyers to streamline legal research, document drafting, contract analysis, and case management.

## What This Skill Does

This skill helps lawyers with:

- ⚖️ **Legal Research**: Finding and analyzing case law, statutes, and regulations
- 📝 **Document Drafting**: Creating contracts, briefs, memoranda, and motions
- 🔍 **Contract Review**: Analyzing agreements, identifying risks, suggesting redlines
- 📋 **Case Management**: Preparing case briefs, chronologies, and fact summaries
- 🗂️ **Discovery**: Reviewing documents, drafting interrogatory responses
- ✅ **Due Diligence**: Creating checklists and reviewing corporate documents
- ✍️ **Legal Writing**: Crafting persuasive arguments and client communications
- 📚 **Citation Help**: Proper Bluebook formatting and verification

## Installation

### Prerequisites
- [Claude Code](https://claude.ai/code) installed on your system
- Node.js (required for Claude Code)

### Setup Steps

1. **Create a skills directory** (if you don't have one):
   ```bash
   mkdir -p ~/.claude/skills
   ```

2. **Copy the skill file**:
   ```bash
   cp legal-assistant-SKILL.md ~/.claude/skills/
   ```

3. **Activate in Claude Code**:
   Open Claude Code and the skill will be automatically available.

## How to Use This Skill

### Quick Start Examples

**Legal Research:**
```
Research whether California recognizes the economic loss doctrine in 
construction defect cases. I need recent appellate decisions.
```

**Contract Drafting:**
```
Draft a software license agreement for a SaaS product. The license 
should be non-exclusive, subscription-based, and include standard 
limitation of liability and IP protection clauses.
```

**Contract Review:**
```
Review this NDA. My client is the receiving party. Flag any 
problematic provisions and suggest specific changes.
[paste contract text]
```

**Motion Writing:**
```
Draft the argument section for a motion for summary judgment. 
Jurisdiction is federal court (9th Circuit). The issue is whether 
plaintiff can establish causation. Here are the facts: [...]
```

### Best Practices

1. **Be Specific About Jurisdiction**: Always mention which court, state, or federal system applies
   
2. **Provide Context**: Share relevant facts, procedural posture, and your role (plaintiff/defendant, buyer/seller)

3. **Specify the Audience**: Let Claude know if the document is for a court, client, or opposing counsel

4. **Request Specific Formats**: Ask for memos, briefs, bullet points, tables, or redlines as needed

5. **Iterate and Refine**: Start with a draft, then ask for revisions to specific sections

### Example Workflows

#### Workflow 1: Contract Negotiation
```
You: "Review this employment agreement. Client is the employee. 
     Focus on IP assignment and non-compete clauses."

Claude: [Provides detailed analysis with issues flagged]

You: "Draft alternative language for the IP assignment clause 
     that's more favorable to employee."

Claude: [Provides specific redline suggestions]

You: "Now draft an email to opposing counsel explaining our 
     position on these changes."

Claude: [Provides professional email]
```

#### Workflow 2: Legal Research & Brief Writing
```
You: "Research the standard for preliminary injunctions in the 
     Northern District of California."

Claude: [Provides legal research with cases]

You: "Using that research, draft the legal standard section 
     for a motion for preliminary injunction."

Claude: [Provides drafted section with citations]

You: "Now add an argument section addressing the likelihood 
     of success factor. Here are my facts: [...]"

Claude: [Provides argument with application to facts]
```

#### Workflow 3: Due Diligence Project
```
You: "Create a due diligence checklist for acquiring a 
     healthcare tech startup."

Claude: [Provides comprehensive checklist]

You: "Focus on HIPAA compliance items. What documents should 
     I specifically request?"

Claude: [Provides detailed HIPAA-focused list]

You: "Draft a document request list I can send to the seller."

Claude: [Provides formatted request list]
```

## Features

### Intelligent Analysis
- Applies legal reasoning frameworks (IRAC, CRAC)
- Considers jurisdiction-specific rules
- Flags ambiguities and areas requiring human judgment
- Distinguishes between binding and persuasive authority

### Professional Formatting
- Proper legal citation (Bluebook format)
- Standard document structures (briefs, memos, contracts)
- Clean, professional output ready for attorney review
- Tables, bullet points, and numbered lists as appropriate

### Risk Awareness
- Identifies potential issues in contracts
- Flags ethical considerations
- Notes statute of limitations concerns
- Highlights privilege questions

### Practical Guidance
- Provides strategic options when appropriate
- Suggests next steps in research or litigation
- Prioritizes issues by importance
- Includes explanations for recommendations

## What This Skill Does NOT Do

⚠️ **Important Limitations**:

- **Does not replace legal advice**: A licensed attorney must review all work
- **Does not create binding attorney-client relationships**
- **Cannot access external databases**: No Westlaw, LexisNexis, or court docket access
- **Cannot verify current law**: Knowledge cutoff is January 2025
- **Should not handle highly confidential matters without proper security**

**Always have a licensed attorney**:
- Review all research and citations
- Sign court filings
- Make final strategic decisions
- Provide client advice
- Handle ethical issues

## Practice Area Coverage

This skill supports multiple practice areas:

- **Litigation**: Motions, briefs, discovery, trial prep
- **Corporate/Transactional**: Contracts, M&A, corporate governance
- **Employment Law**: Employment agreements, policies, disputes
- **Intellectual Property**: Licenses, assignments, prosecution support
- **Real Estate**: Purchase agreements, leases, title issues
- **Regulatory/Compliance**: Policy review, compliance audits
- **Family Law**: Agreements, motions, settlement documents
- **Estate Planning**: Wills, trusts, estate documents

## Tips for Best Results

### For Research Tasks
- Specify the jurisdiction precisely
- Mention the specific legal issue or doctrine
- Indicate the time period if relevant
- Note if you need primary or secondary sources

### For Drafting Tasks
- Share any templates or prior examples
- Mention page limits or formatting requirements
- Specify the tone (aggressive, balanced, conciliatory)
- Indicate any required or preferred clauses

### For Review Tasks
- State which party you represent
- Note your priorities (speed vs. comprehensiveness)
- Mention any deal-breaker issues
- Indicate if you want redlines or just analysis

### For Client Communications
- Specify the client's sophistication level
- Note any sensitive issues to handle carefully
- Indicate the purpose (advice, update, request)
- Mention if you need a particular tone

## Advanced Features

### Multi-Document Analysis
```
I have three contracts: [upload files]
Compare the indemnification provisions across all three and 
create a chart showing the differences.
```

### Chronology Building
```
Create a chronology from these emails and documents [upload files]
Focus on communications about the contract dispute.
```

### Citation Checking
```
Review this brief and verify all citations are in proper 
Bluebook format. Also check for any pinpoint citation errors.
```

### Template Creation
```
Create a template for a motion to compel discovery in federal 
court that I can reuse for future cases.
```

## Troubleshooting

**Issue**: Citations seem outdated or incorrect
- **Solution**: Always verify citations independently. This skill cannot access live legal databases.

**Issue**: Analysis doesn't match my jurisdiction's law
- **Solution**: Be very specific about jurisdiction in your prompt. Follow up with corrections.

**Issue**: Output is too formal/informal
- **Solution**: Specify the desired tone: "draft in a formal litigation tone" or "explain this in plain language for a client"

**Issue**: Missing key analysis
- **Solution**: Ask follow-up questions: "What about [specific issue]?" or "Analyze the [specific clause] more deeply"

## Security & Confidentiality

⚠️ **Important**: Be mindful of confidentiality obligations when using AI tools:

- Avoid sharing highly sensitive client information
- Redact party names and identifying details when possible
- Do not share privileged communications without protection
- Check your firm's AI usage policy
- Consider using hypotheticals for sensitive matters

## Support & Feedback

This skill was created to help lawyers work more efficiently. For:

- **Skill improvements**: Consider what works well and what could be better
- **Bug reports**: Note any incorrect legal analysis or formatting issues
- **Feature requests**: Think about what additional capabilities would help your practice

## License & Disclaimer

This skill is provided as-is for use with Claude Code. It is designed to assist lawyers but does not constitute legal advice. All outputs should be reviewed by a licensed attorney before use. The skill creator assumes no liability for errors or omissions.

---

## Example Prompts to Get Started

Try these to see what the skill can do:

1. "Explain the difference between a motion to dismiss under 12(b)(6) and a motion for summary judgment."

2. "Draft a cease and desist letter for trademark infringement. Keep it firm but professional."

3. "What are the key provisions I should include in a commercial lease?"

4. "Review this termination clause and tell me if it's favorable to the employer or employee: [paste clause]"

5. "Create a witness list template for a federal civil trial."

6. "What's the test for personal jurisdiction in the Ninth Circuit?"

7. "Draft boilerplate language for a severability clause."

8. "Explain attorney-client privilege to a client in simple terms."

---

**Happy lawyering! This skill is here to make your legal work faster and more efficient.** 🎯
