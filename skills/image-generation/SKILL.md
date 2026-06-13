---
name: image-generation
description: Use this skill whenever the user wants to generate, edit, or describe images using Grok Imagine render components or similar AI image capabilities. Triggers include generate image, create picture, AI art, visualize, diagram, illustration, edit this image, Grok Imagine, prompt engineering, orientation, layout requests.
---

# Image Generation & Editing

## When to Use
- User requests image creation, modification, or visualization.
- Leverage `render_generated_image` and `render_edited_image` components.
- Ensure prompts are detailed, faithful to user intent, and avoid prohibited content (hate, violence, etc.).

## Core Workflow
1. Clarify the prompt if ambiguous.
2. Craft a high-quality prompt: subject, style, lighting, composition, mood.
3. Decide on orientation (portrait/landscape) and layout (block/inline).
4. Output the render component in final response.
5. For edits, reference previous image_id.

## Best Practices
- Be specific: "photorealistic, 8k, detailed textures"
- Maintain consistency across multiple generations.
- Use `view_image` tool if needed for reference.

## Examples
- Generate: Use render_generated_image with detailed prompt.
- Edit: Use render_edited_image with image_id and modification prompt.