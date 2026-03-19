# Ashish Khoshya — Portfolio

## Quick Start (Local)

```bash
npm install
npm run dev
```

Opens at `http://localhost:5173`

## Deploy to Vercel (Recommended)

1. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Portfolio v1"
   ```
   Create a repo on github.com, then:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
   git push -u origin main
   ```

2. **Connect to Vercel**
   - Go to [vercel.com](https://vercel.com) → Sign up with GitHub
   - Click "New Project" → Import your repo
   - Framework: Vite (auto-detected)
   - Click Deploy — done in ~60 seconds

3. **Add Custom Domain**
   - Vercel Dashboard → Your Project → Settings → Domains
   - Add `yourdomain.com`
   - Update your domain DNS:
     - **A Record**: `76.76.21.21`
     - **CNAME** (for www): `cname.vercel-dns.com`
   - SSL is automatic

## Deploy to Netlify (Alternative)

1. Push to GitHub (same as above)
2. Go to [netlify.com](https://netlify.com) → New site from Git
3. Build command: `npm run build`
4. Publish directory: `dist`
5. Add custom domain in Site settings → Domain management

## Build for Any Host

```bash
npm run build
```

This creates a `dist/` folder with static files. Upload that folder to any hosting provider (AWS S3, Firebase, Cloudflare Pages, etc).
