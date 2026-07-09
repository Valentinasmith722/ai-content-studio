# AI Content Studio 🎨

> Your all-in-one AI-powered content creation workspace. Generate blog posts, social media content, video scripts, email campaigns, and SEO-optimized copy — all from one intuitive dashboard. Perfect for marketers, creators, agencies, and businesses.

## ✨ Features

### Content Generation
- **Blog Posts**: Long-form articles with SEO optimization, internal linking, and readability scoring
- **Social Media**: Platform-specific content for Twitter, LinkedIn, Instagram, TikTok, Facebook
- **Video Scripts**: YouTube scripts, TikTok hooks, podcast outlines with timing
- **Email Campaigns**: Welcome sequences, newsletters, promotional emails, cold outreach
- **Ad Copy**: Google Ads, Facebook Ads, LinkedIn Ads with A/B test variants
- **Product Descriptions**: E-commerce copy that converts with SEO keywords
- **Landing Pages**: High-converting copy with psychological triggers
- **Press Releases**: Professional announcements for media distribution

### AI Assistants
- **Brand Voice Trainer**: Train AI on your brand's tone, style, and vocabulary
- **Competitor Analyzer**: Analyze competitor content and identify gaps
- **Trend Hunter**: Discover trending topics in your niche before they peak
- **Content Calendar AI**: Auto-generate monthly content calendars
- **Repurposer**: Turn one piece of content into 10+ formats automatically
- **Translator**: Translate and localize content for global audiences
- **Fact Checker**: Verify claims and suggest citations
- **Plagiarism Detector**: Ensure originality before publishing

### Workflow Tools
- **Kanban Board**: Drag-and-drop content pipeline (Ideas → Writing → Review → Published)
- **Collaboration**: Real-time editing, comments, and approvals
- **Version History**: Track changes and revert to previous versions
- **Content Library**: Organize and tag all your content assets
- **Publishing Scheduler**: Queue content for automatic publishing
- **Performance Analytics**: Track engagement, CTR, and conversion rates
- **A/B Testing**: Test headlines, CTAs, and content variations
- **SEO Score**: Real-time SEO optimization suggestions

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/valentinasmith722/ai-content-studio.git
cd ai-content-studio

# Install dependencies
npm install

# Configure AI providers
cp .env.example .env
# Add your OpenAI, Anthropic, or Google AI API keys

# Start the application
npm run dev

# Open http://localhost:3000
```

## 🎨 Dashboard Preview

```
┌─────────────────────────────────────────────────────────────┐
│  AI Content Studio v2.5                    [New Project +]  │
├──────────────────┬────────────────────────────────────────────┤
│  📁 Projects     │  ✨ Today's Content                         │
│  ┌──────────────┐ │                                          │
│  │ Blog Posts   │ │  📝 "10 Solana DeFi Strategies"           │
│  │   (12)       │ │     Status: ✅ Published | Views: 2.3k   │
│  └──────────────┘ │                                          │
│  ┌──────────────┐ │  📱 Twitter Thread: "AI Tools 2026"       │
│  │ Social Media │ │     Status: 🔄 Scheduled | 9:00 AM       │
│  │   (45)       │ │                                          │
│  └──────────────┘ │  📧 Newsletter: "Weekly Crypto Digest"    │
│  ┌──────────────┐ │     Status: 📝 Draft | 85% complete       │
│  │ Video Scripts│ │                                          │
│  │   (8)        │ │  🎥 YouTube Script: "DeFi Tutorial"       │
│  └──────────────┘ │     Status: ⏳ In Review                  │
│  ┌──────────────┐ │                                          │
│  │ Emails       │ │  📊 Performance This Week                 │
│  │   (23)       │ │  Content: 15 pieces | Engagement: +32%   │
│  └──────────────┘ │  Top Performer: Blog Post (+450 shares)   │
└──────────────────┴────────────────────────────────────────────┘
```

## 🛠️ Tech Stack

- **Frontend**: Next.js 14 + Tailwind CSS + shadcn/ui
- **Backend**: Next.js API Routes + tRPC
- **Database**: PostgreSQL + Prisma ORM
- **AI Models**: OpenAI GPT-4 + Anthropic Claude + Google Gemini
- **Vector DB**: Pinecone (semantic search, content similarity)
- **File Storage**: AWS S3 (assets, exports)
- **Queue**: Bull + Redis (background AI generation)
- **Auth**: Clerk (user management, organizations)
- **Real-time**: Socket.io (collaborative editing)
- **Export**: Puppeteer (PDF) + docx (Word)

## 🎯 Use Cases

- **Content Creators**: Generate weeks of content in hours, not days
- **Marketing Agencies**: Handle multiple clients with brand-specific AI training
- **E-commerce**: Auto-generate product descriptions, ads, and email campaigns
- **SaaS Companies**: Blog posts, case studies, documentation, and changelog
- **Newsletters**: Daily/weekly newsletters with curated content and original analysis
- **YouTubers**: Script writing, thumbnail ideas, title optimization, descriptions
- **Real Estate**: Property descriptions, market reports, email campaigns
- **Restaurants**: Menu descriptions, social media, email promotions
- **Nonprofits**: Grant proposals, donor communications, impact reports

## 🔧 Configuration

Create a `.env` file:

```env
# Database
DATABASE_URL=postgresql://user:pass@localhost/ai_content_studio

# AI Providers (at least one required)
OPENAI_API_KEY=sk-...
ANTHROPIC_API_KEY=sk-ant-...
GOOGLE_AI_API_KEY=AIza...

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_...
CLERK_SECRET_KEY=sk_...

# Pinecone (vector search)
PINECONE_API_KEY=...
PINECONE_ENVIRONMENT=...
PINECONE_INDEX_NAME=...

# AWS S3
AWS_ACCESS_KEY_ID=...
AWS_SECRET_ACCESS_KEY=...
AWS_REGION=us-east-1
AWS_S3_BUCKET=...

# Redis (queue)
REDIS_URL=redis://localhost:6379/0

# Optional: Analytics
POSTHOG_KEY=...
POSTHOG_HOST=...

# Optional: Image generation
REPLICATE_API_TOKEN=...
STABILITY_API_KEY=...
```

## 🎓 AI Prompt Templates

### Blog Post Generator
```
Write a [word_count]-word blog post about [topic] for [target_audience].

Tone: [professional/casual/technical/persuasive]
Include:
- Hook in first 2 sentences
- 3-5 main sections with H2 headings
- Data/statistics where relevant
- Actionable takeaways in conclusion
- SEO keywords: [keyword1, keyword2, keyword3]

Format: Markdown with proper headings and bullet points
```

### Social Media Generator
```
Create [platform] content about [topic].

Platform: [Twitter/LinkedIn/Instagram/TikTok/Facebook]
Goal: [engagement/leads/awareness/sales]
Tone: [inspirational/educational/humorous/controversial]
Include: [hashtags/CTA/questions/polls]

Generate [number] variations
```

### Email Sequence Generator
```
Write a [number]-email sequence for [goal].

Audience: [description]
Trigger: [signup/purchase/abandoned_cart/lead_magnet]
Tone: [friendly/professional/urgent/exclusive]

Each email should:
- Have a compelling subject line
- Be 150-300 words
- Include one clear CTA
- Build on previous emails
```

## 📦 Content Types Supported

| Type | AI Model | Avg. Generation Time | Export Formats |
|------|----------|---------------------|----------------|
| Blog Post | GPT-4 | 30-60s | Markdown, HTML, PDF, Word |
| Social Media | GPT-4/Claude | 10-20s | Text, JSON, CSV |
| Video Script | GPT-4 | 45-90s | Markdown, PDF, Final Draft |
| Email | GPT-4/Claude | 15-30s | HTML, Text, JSON |
| Ad Copy | GPT-4 | 10-20s | Text, JSON |
| Product Description | GPT-4 | 15-30s | HTML, Text |
| Landing Page | GPT-4 | 60-120s | HTML, React, Vue |
| Press Release | GPT-4 | 30-60s | Markdown, PDF, Word |

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Ways to Contribute

- 🐛 Report bugs via GitHub Issues
- 💡 Suggest features via GitHub Discussions
- 🔧 Submit pull requests
- 🎨 Design UI components and themes
- 📖 Write documentation and tutorials
- 🌍 Translate the interface
- 🤖 Add new AI prompt templates
- 📊 Improve analytics and reporting

## ☕ Support This Project

This tool is **100% free and open source**. We built it because we believe every creator, marketer, and business deserves access to powerful AI content tools without paying $100+/month for proprietary platforms.

If AI Content Studio helped you create better content faster, grow your audience, or save hours of writing time, consider supporting its continued development:

**Solana (USDT)**: `BKjS4agVRowFGqUuWHEKZerk3dCS52V1n4NdWaeNTo8E`

Your support helps us:
- Integrate more AI models (Llama, Mistral, local models)
- Develop advanced features like video generation and voice cloning
- Create prompt libraries for every industry
- Build a marketplace for community templates
- Improve performance and reduce generation costs
- Keep the tool free for individual creators and small businesses
- Support open-source AI development

*Every contribution helps us democratize AI content creation. Thank you for being part of our mission.* 🙏

## 📄 License

MIT License — free to use, modify, and distribute.

## 🌟 Star History

If this tool 10x'd your content output, please give it a star ⭐ on GitHub!

---

*Built with ❤️ for creators everywhere | 2026*
