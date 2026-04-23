---
name: app-spec-creator
description: Create an e-commerce app specification document by prompting user for store type, colors, name, stack, product type, and page structure. Works with any AI agent.
---

# App Specification Creator

When this prompt is invoked, follow these steps:

1. Prompt the user for the following information:
   - Type of app (e.g., e-commerce, blog, portfolio, dashboard)
   - Name of the app
   - Preferred stack (Next.js or React Vite)
   - Primary and secondary colors
   - A brief description of the app's purpose and target audience
   - Ask whether they want to upload an image for the design or have the system generate a design based on the colors and app type. If they choose to upload an image, prompt them to provide the image file.

2. If the app type is "e-commerce", ask the user for the following details:
   - The product type or store category (for example: perfume, fashion, electronics, home goods, wellness)
   - The target audience or customer profile
   - Whether they prefer a clean premium style, bold modern look, or friendly bright design
   - Whether they want a custom design image or a system-generated design based on the colors

3. For an e-commerce app, use the following required store pages:
   - Home page
   - Store/Product listing page
   - Single product view page
   - Cart page (sheet/modal style)
   - Checkout page
   - About Us page
   - Contact Us page
   - Signup/Login page
   - User Order History page
   - User Account Settings page
   - User Wishlist page

   And include admin store pages:
   - Admin Dashboard page
   - Admin Dashboard Products page
   - Admin Dashboard Orders page
   - Admin Dashboard Transactions page
   - Admin Dashboard Customers page
   - Admin Dashboard Analytics page
   - Admin Dashboard Settings page

   For each page, write a brief description of its content, purpose, and main functionality. Make sure all pages are created.

4. If the app type is not "e-commerce", ask the user:
   - How many pages should the app have?
   - A brief description of what each page should contain.

5. Generate a clean markdown specification document that includes:
   - App Overview (type, name, stack, product type, audience)
   - Design Specifications (colors, style direction)
   - Page Structure (list of pages and content outline)
   - Technical Stack details
   - Any special features (cart sheet, checkout flow, admin dashboard, login/signup)

6. Output the complete markdown document. If possible, save it as `app-spec.md`; otherwise return the markdown text directly.
