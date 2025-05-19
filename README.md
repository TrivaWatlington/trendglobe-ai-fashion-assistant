# 🧠 TrendGlobe – AI-Powered Fashion Assistant

TrendGlobe is an AI-driven fashion assistant that helps users discover region-specific and seasonally relevant apparel using OpenAI’s GPT-4.1 with function calling. Built with Next.js 13+, it combines generative AI, interactive tooling, and personalization to deliver curated fashion guidance.

---

## 🚀 Features

- 🌍Region & Season-Aware Suggestions
  AI provides outfit and trend recommendations tailored by user's location and current season.

- 🧰Tool-Calling via OpenAI GPT-4.1
  Tools such as `get_trending_products`, `suggest_outfits`, `get_size_chart`, and `check_product_availability` are integrated and invoked automatically via function calls.

- 👤Persona Memory
  Users can define style personas (e.g., “Minimalist,” “Y2K,” “Professional”) which influence ongoing outfit suggestions.

- 💬Streaming Chat Interface
  Real-time AI interaction via a sleek chat UI.

- 🎨Custom Brand Styling
  Uses TrendGlobe’s palette: coral, light coral, teal, and dark teal.

---

## 🛠 Built With

- [Next.js 13+ App Router](https://nextjs.org/docs)
- [OpenAI GPT-4.1](https://platform.openai.com/)
- [Replit Hosting Environment](https://replit.com/)
- `ai` SDK for streaming + tool integration
- Replit DB (optional, for persona memory)

---

## 📂 Project Structure
/app
└── api
└── chat
└── route.ts # API handler using OpenAI function calling
/lib
└── tools
├── index.ts # Tool logic handlers
└── schema.ts # Tool definitions (tool metadata)
/styles
└── globals.css # Brand styling
/pages
└── _app.js # Global CSS imported here
.env.local # API Key for OpenAI


---

## ⚙️ Tools & Functions

| Tool Name | Purpose |
|-----------|---------|
| `get_trending_products(region, season)` | Lists currently trending apparel |
| `check_product_availability(product_id, size, region)` | Returns product availability by region and size |
| `get_size_chart(product_id)` | Returns size breakdown for an item |
| `suggest_outfits(persona, season)` | Recommends full outfit sets for style archetypes |

---

## 🧪 Test Prompts

Try asking the assistant:

- “What’s trending in New York for spring?”
- “Do you have that linen blazer in size medium?”
- “Suggest a Gen Z summer outfit for someone who loves cottagecore.”

---

## 🔐 Environment Variables

Create a `.env.local` file with your OpenAI key:

```env
OPENAI_API_KEY=sk-xxxxxx

npm install
npm run dev
Then visit http://localhost:3000 or your Replit live link.

📈 Future Enhancements
User login + persistent profiles

Pinterest/Google Trends API integration

Visual outfit generation (DALL·E / Midjourney API)

Admin dashboard with AI insights

Favorite & save-to-cart integration

🙋🏽‍♀️ About the Creator
Triva Watlington
Product Manager & Retail Tech Innovator
TrendGlobe is her AI case study project blending fashion, personalization, and emerging tech.
www.trivawatlington.com

📄 License
MIT License
