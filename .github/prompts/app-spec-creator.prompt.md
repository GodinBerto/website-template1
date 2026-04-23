---
name: app-spec-creator
description: Create an app specification document by prompting user for type, colors, name, stack, pages, and content. Works with any AI agent.
---

# App Specification Creator

When this prompt is invoked, follow these steps:

1. Prompt the user for the following information:
   - Type of app (e.g., e-commerce, blog, portfolio, dashboard)
   - Colors (primary and secondary color scheme)
   - Name (app name)
   - Stack (choose between Next.js or React Vite)
   - Number of pages
   - Document of the app content (brief description of what each page should contain)

2. After collecting all the information, generate a comprehensive markdown document that includes:
   - App Overview (type, name, stack)
   - Design Specifications (colors)
   - Page Structure (number of pages and content outline)
   - Technical Stack details

3. Output the document. If possible, save it as `app-spec.md`.
