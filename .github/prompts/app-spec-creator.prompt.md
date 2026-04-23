---
name: app-spec-creator
description: Create an app specification document by prompting user for type, colors, name, stack, and content. For e-commerce apps, includes predefined pages like home, store, product view, cart, checkout, admin dashboard, etc. Works with any AI agent.
---

# App Specification Creator

When this prompt is invoked, follow these steps:

1. Prompt the user for the following information:
   - Type of app (e.g., e-commerce, blog, portfolio, dashboard)
   - Colors (primary and secondary color scheme)
   - Name (app name)
   - Stack (choose between Next.js or React Vite)

2. if the app type is "e-commerce", ask the user if they want to:
   - Provide a design image for it or Use a predefined design based on the colors provided
   - If they choose to provide a design image, prompt them to upload it and analyze the design to extract the color scheme and layout information. Use this information to generate the app specification document.
   - The type of product the user wants to sell (e.g., clothing, electronics, home goods) to tailor the page content and layout accordingly.

3. If the app type is "e-commerce", use the following predefined pages
   - Home page
   - Store/Product listing page
   - Single product view page
   - Cart page (implemented as a sheet/modal)
   - Checkout page
   - About Us page
   - Contact Us page
   - Admin Dashboard page
   - Admin Dashboard Products page
   - Admin Dashboard Orders page
   - Admin Dashboard Transactions page
   - User Order History page
   - User Account Settings page
   - User Wishlist page
   - Signup/Login page

   For each page, include a brief description of the content and functionality.

4. If the app type is not "e-commerce", prompt for:
   - Number of pages
   - Document of the app content (brief description of what each page should contain)

5. After collecting all the information, generate a comprehensive markdown document that includes:
   - App Overview (type, name, stack)
   - Design Specifications (colors)
   - Page Structure (list of pages with content outline)
   - Technical Stack details

6. Output the document. If possible, save it as `app-spec.md`.
