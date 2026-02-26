# Knowledge App

This project is a practical application developed while following the official Contentful engineering guide: [Integrate Contentful with Next.js App Router](https://www.contentful.com/blog/integrate-contentful-next-js-app-router/).

## 🚀 Features
* **Next.js App Router**: Leverages React Server Components to render and cache HTML on the server, enhancing page speed and SEO.
* **Contentful GraphQL API**: Optimized data fetching that retrieves only the specific fields needed for the UI.
* **Dynamic Routing**: Automatic generation of article pages using the `[slug]` dynamic segment.
* **On-Demand Revalidation**: Real-time cache purging via Contentful Webhooks to ensure content updates instantly.

## 🛠️ Tech Stack
* **Framework**: Next.js (App Router)
* **CMS**: Contentful (Headless)
* **Styling**: Tailwind CSS
* **Rendering**: `@contentful/rich-text-react-renderer`

## 📖 Learning Journey
By following the tutorial, I implemented:
1. **API Integration**: Connecting Next.js to the Contentful Delivery API.
2. **Static Generation**: Using `generateStaticParams` to pre-render pages at build time.
3. **Image Optimization**: Configuring `next.config.js` to serve assets from Contentful.
4. **Cache Management**: Using the `articles` tag for surgical cache revalidation.

## ⚙️ Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/your-username/knowledge-app.git

# 2. Install dependencies
npm install

# 3. Configure Environment Variables
 Create a .env.local file in the root directory and add:
# CONTENTFUL_SPACE_ID=your_space_id
# CONTENTFUL_ACCESS_TOKEN=your_delivery_token
# CONTENTFUL_PREVIEW_ACCESS_TOKEN=your_preview_token

# 4. Run the development server
npm run dev