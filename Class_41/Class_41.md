# Readings: React 4

## Class_41

**Question 1:**

    Dynamic routes refer to the capability of creating pages with variable parameters in the URL, allowing for more flexible and dynamic content rendering. Dynamic routes enable you to create pages that can handle different data and content based on the values passed in the URL. This is in contrast to static routes, where each page has a fixed URL and the content remains the same until a new build.
---

**Question 2:**

1. Create a Next.js app
2. Push to GitHub
3. The easiest way to deploy Next.js to production is to use the Vercel platform
4. Deploy to Vercel
   - Create a Vercel account
   - Import your GitHub project
   - You’ll need to Install Vercel for GitHub. You can give it access to All Repositories. Once you’ve installed Vercel, import `nextjs-blog`.
   - Next.js can be deployed to any hosting provider that supports Node.js. Some deployment platforms are:
     - Vercel
     - Netlify

---

**Question 3:**
Next.js handles static file serving in a simple and efficient manner. By default, it automatically serves static assets from a folder called "public" in the root directory of the Next.js application. The "public" folder is intended for files that should be publicly accessible and do not require any special server-side processing, such as images, fonts, and videos.

To reference static assets in a Next.js application, you use the `next/image` component for images, which provides automatic image optimization and additional features like lazy loading and responsive images. For other types of static files, you can reference them directly using standard HTML tags.

The default folder structure of a Next.js application includes the "public" folder, where you can organize your static assets into subdirectories, making it easy to manage and access these files in your components.

---
