<!-- Powered by BMAD™ Core -->

# Generate Cover Prompts Task

## Purpose

Create exceptional AI image generator prompts for book cover artwork that push creative boundaries and produce visually striking, genre-appropriate covers. This task leverages advanced AI creative capabilities to generate detailed, effective prompts that result in professional-quality cover art concepts.

## Why This Approach Works

AI image generators respond best to specific, detailed prompts that include style descriptors, mood keywords, and technical photography terms. By providing comprehensive creative direction, we enable the AI to produce covers that not only look professional but also effectively communicate the book's genre and emotional tone to potential readers.

## Inputs Required

- **cover-brief.md** - Contains genre, target audience, mood, key themes, and any specific imagery requirements
- Context about the book's content, tone, and market positioning (extracted from brief)

## Process Overview

### Step 1: Creative Foundation Analysis

First, analyze the cover brief to extract and understand these critical elements because they form the creative foundation for all generated prompts:

- **Genre conventions** - Understanding visual expectations helps ensure market appeal
  - *Romance:* Warm colors, intimate compositions, typography with flourishes
  - *Thriller/Mystery:* Dark palettes, dramatic lighting, bold sans-serif fonts
  - *Fantasy:* Rich textures, magical elements, ornate or mystical typography
  - *Literary Fiction:* Minimalist designs, artistic photography, elegant serif fonts
  - *Sci-Fi:* Futuristic elements, cool color schemes, modern geometric fonts
- **Target audience preferences** - Age, demographics inform style choices that resonate
- **Emotional tone** - The feeling the cover should evoke drives color and composition decisions  
- **Key themes and symbols** - Central concepts that should be visually represented
- **Competitive landscape** - What works in this genre and how to stand out

### Step 2: Creative Prompt Generation

**Don't hold back. Give it your all.** Generate 4-6 alternative image prompts that showcase creative excellence and push artistic boundaries. Each prompt should be bold, vivid, and comprehensive.

For each prompt, structure your output using these XML sections:

#### <image_prompt>
Create a detailed, specific prompt (150-200 words) that includes:

- **Visual composition**: Specific framing, perspective, focal points
- **Style descriptors**: Art movement, artistic technique, visual aesthetic
- **Technical specifications**: Camera angle, lighting, depth of field
- **Color palette**: Dominant colors, mood-setting hues, contrast levels  
- **Atmospheric elements**: Weather, time of day, environmental mood
- **Character/object details**: If applicable, specific descriptions of people or key objects

**Include genre-specific visual cues** because these immediately communicate the book's category to browsers and help it stand out in crowded marketplaces.

#### <style_modifiers>
Add 8-12 technical enhancement keywords that refine the artistic approach:
- Photography terms (e.g., "golden hour lighting", "shallow depth of field")  
- Artistic styles (e.g., "digital painting", "photorealistic", "surreal")
- Quality indicators (e.g., "highly detailed", "award-winning", "masterpiece")
- Rendering specifications (e.g., "8K resolution", "professional photography")

#### <negative_prompts>
Specify 6-8 elements to avoid because these commonly create issues in AI-generated cover art:
- Technical flaws: "blurry", "pixelated", "artifacts", "distorted proportions"
- Genre-inappropriate elements: List specific items that would confuse the genre
- Quality issues: "amateur", "low resolution", "watermarks", "text overlays"

### Step 3: Typography Guidance

#### <typography_recommendations>
Provide font pairing suggestions that complement each visual concept because typography integration is crucial for professional cover design:

**Primary Title Font Options:**
- 2-3 Google Fonts with specific reasoning for genre appropriateness
- Consider: readability at thumbnail size, genre conventions, mood alignment

**Secondary Text Font:**
- Complementary font for author name, subtitle, or taglines
- Ensure hierarchy and contrast with primary font

**Design Integration Notes:**
- Suggested placement areas that work with the generated imagery
- Color recommendations for text that ensure readability
- Size and spacing considerations for various formats (print, digital, thumbnail)

### Step 4: Quality Reflection and Iteration

After generating initial prompts, reflect on their effectiveness and creative strength. Consider:
- Do these prompts push creative boundaries while remaining commercially viable?
- Are the technical specifications detailed enough to produce high-quality results?
- Do the concepts effectively communicate the book's genre and appeal to the target audience?
- Are there opportunities to add more unique, memorable visual elements?

Refine and enhance any prompts that could be more compelling or technically precise.

## Output Structure

Create a comprehensive **cover-prompts.md** file with this exact structure:

```markdown
# Cover Art Prompts for [Book Title]

## Creative Brief Summary
[2-3 sentence synthesis of key requirements from the brief]

## Concept 1: [Descriptive Name]
<image_prompt>
[Detailed prompt text]
</image_prompt>

<style_modifiers>
[Technical enhancement keywords]
</style_modifiers>

<negative_prompts>
[Elements to avoid]
</negative_prompts>

<typography_recommendations>
[Font and design integration guidance]
</typography_recommendations>

---

[Repeat structure for each additional concept]

## Implementation Notes
- **Recommended AI tools:** DALL-E, Midjourney, Stable Diffusion, Firefly - these prompts work across platforms with minor adaptations
- **Cross-platform compatibility:** Core prompting principles work universally, though specific syntax may vary by tool
- **Iteration suggestions:** [How to refine results based on initial outputs]
- **Market considerations:** [Genre-specific advice for final selection]
```

## Success Criteria

**Exceptional prompts will:**
- Generate visually striking covers that immediately communicate genre
- Include sufficient technical detail for high-quality AI generation
- Push creative boundaries while maintaining commercial appeal
- Provide clear typography integration guidance
- Offer multiple distinct visual approaches for client choice

**Quality indicators:**
- Prompts are specific and detailed (not generic)
- Technical specifications ensure professional-quality output
- Creative concepts are memorable and emotionally engaging
- Typography recommendations enhance rather than compete with imagery

## Task Configuration

```yaml
task:
  id: generate-cover-prompts
  name: Generate Cover Prompts  
  description: Create exceptional AI image prompts for book cover artwork with universal AI optimization
  persona_default: cover-designer
  inputs:
    - cover-brief.md
  output: cover-prompts.md
  optimization: universal-ai-enhanced
```
