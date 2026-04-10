# PricePulse


A simple price tracker that emails you when the price drops.

## What it does
- Sign in with Google
- Paste a product URL
- PricePulse tracks the price in the background
- You get an email when the price goes down
- Track multiple products
- Remove products anytime

That’s it.

## Why I built this
I wanted a simple way to track product prices without constantly checking the same page again and again.  
So I built one.

## Tech Stack
- Next.js
- Supabase
- Firecrawl
- shadcn/ui
- Resend (email alerts)

## How it works
1. Add a product link
2. The product is stored in the database
3. Prices are checked periodically
4. When a price drops, an email alert is sent

## Setup (Local)
1. Clone the repo
2. Install dependencies
3. Add environment variables
4. Run the app

```bash
npm install
npm run dev
```

## Environment Variables

Create a .env.local file with:
```bash
FIRECRAWL_API_KEY=your_firecrawl_key

NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key

RESEND_API_KEY=your_resend_key
RESEND_FROM_EMAIL=alerts@yourdomain.com

CRON_SECRET=your_cron_secret
```

## Author

**Om Sharma**  
Indie developer building useful, real-world products.  
🔗 [LinkedIn](https://www.linkedin.com/in/om-sharma1905/)
