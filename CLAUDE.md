# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a business book project titled "The Gnostic Enterprise: Harnessing the Power of Knowledge and Innovation" written in AsciiDoc format. The book explores enterprise transformation, AI augmentation, agile methodologies, and the creation of "super employees" through technology integration.

## Project Structure

- **Main file**: `book.adoc` - Master document that includes all chapters
- **Chapters**: Located in `chapters/` directory, numbered 01-13 with kebab-case naming
- **Images**: 
  - `ai-images/` - AI-generated illustrations (MidJourney)
  - `images/` - Traditional diagrams and business illustrations
  - `cover/` - Book cover materials
- **Build**: `themes/the-gnostic-enterprise-theme.yml` - PDF styling configuration
- **Automation**: `.github/workflows/build-book.yml` - Automated PDF generation and releases

## Common Commands

### Building the Book
```bash
# Build PDF locally
asciidoctor-pdf -a pdf-theme=the-gnostic-enterprise-theme.yml -a pdf-themesdir=themes book.adoc -o book.pdf --trace -v

# Trigger automated build
gh workflow run build-book.yml
```

### Development Workflow
```bash
# Check recent workflow runs
gh run list --workflow=build-book.yml --limit=5

# View specific run details
gh run view [RUN_ID]

# List releases
gh release list
```

## Writing Style and Tone Guidelines

### Core Voice Characteristics

**Conversational Authority**: Write as an experienced practitioner sharing hard-won insights. Balance accessibility for business leaders with technical depth that demonstrates expertise.

**Forward-Thinking Optimism**: Maintain an enthusiastic yet realistic perspective on technological transformation. Focus on possibilities while acknowledging practical challenges.

**Human-Centered Technology**: Always frame AI and automation as human augmentation, not replacement. Emphasize the power of the individual enhanced by technology.

**Philosophical Grounding**: Incorporate Stoic principles and ethical considerations. Address moral responsibilities of enterprises and the symbiotic relationship with society.

### Audible-Friendly Structure

Since this book should read well as an audiobook:

- **Clear Transitions**: Use phrases like "In conclusion," "Now let's explore," "This brings us to"
- **Memorable Quotes**: Include quotable insights in block quotes (> format)
- **Bullet Points**: Use for key concepts and actionable items
- **Analogies**: Employ real-world comparisons (e.g., "taking a quiz without devices vs. with a phone")
- **Repetition for Emphasis**: Reinforce key concepts across chapters
- **Conversational Asides**: Include parenthetical thoughts and direct reader address

### Content Patterns

**Opening Hooks**: Each chapter should start with a compelling image reference and immediately establish relevance to the reader's challenges.

**Practical Application**: Follow theoretical concepts with concrete examples, actionable steps, or real-world implementations.

**Data Integration**: Reference specific statistics and studies with footnotes when available.

**Personal Reflection**: Include observations about industry trends and personal insights from experience.

**Ethical Considerations**: Address the broader implications and responsibilities of technological adoption.

### Language Guidelines

**Terminology Consistency**:
- "Super employees" (not "super-employees" in text)
- "Artificial Intelligence" or "AI"
- "Cloud technologies" and "low-code platforms"
- "Agile squads" (6-10 people)
- "The enterprise" when referring to organizations generally

**Tone Markers**:
- Use second person ("you," "your organization") to maintain engagement
- Include rhetorical questions to prompt reflection
- Employ active voice predominantly
- Balance formal business language with accessible explanations

**Sentence Structure**:
- Vary sentence length for audio flow
- Use shorter sentences for key points
- Employ parallel structure in lists
- Include transitional phrases between concepts

### Chapter Development

**Standard Structure**:
1. Compelling visual hook (AI-generated image)
2. Problem or opportunity identification
3. Conceptual framework introduction
4. Practical applications and examples
5. Implementation guidance
6. Ethical or philosophical considerations
7. Connection to broader enterprise transformation

**Key Themes to Weave Throughout**:
- People, Process, Technology optimization
- Continuous learning and adaptation
- Employee and customer happiness correlation
- Measurement and data-driven decisions
- Collaboration and team dynamics
- Ethical technology implementation

### Special Considerations

**AI Transparency**: The book openly acknowledges AI assistance in creation (written "with the assistance of AI, including ChatGPT"). Maintain this transparency about AI augmentation as a practical example.

**Visual Integration**: Reference AI-generated images meaningfully, not just decoratively. Connect visuals to chapter themes and concepts.

**Practical Urgency**: Emphasize that transformation is happening "today - not some far off event in the future."

**Individual Empowerment**: Always return to how concepts empower individuals to add value and find meaning in their work.

This book serves as both educational content and a practical demonstration of AI-augmented content creation, embodying the principles it teaches about human-technology collaboration.