# Vikas V T — Portfolio

One website with three shareable links (replace `yourname.vercel.app` with your deployed address):
- `https://yourname.vercel.app/` opens the intro and both portfolio choices
- `https://yourname.vercel.app/#tech` opens the career portfolio
- `https://yourname.vercel.app/#growth` opens the business / freelancing portfolio

Send recruiters the `#tech` link and clients the `#growth` link.

## What's inside
```
index.html      the whole website (text, design, animation, contact links)
images/         your photos (replace a file, keep the same name)
videos/         put your edited videos here
README.md       this guide
```

## Preview on your computer
Double-click `index.html`. If the photos don't show, run `python3 -m http.server` in this folder and open http://localhost:8000.

## How to edit
Open `index.html` in any editor (VS Code, or edit directly on GitHub with the pencil icon).
- Change text: search for the words you want to change and edit them.
- Change numbers: search `15+` (clients), `6` (countries), `3+ years`.
- Phone, email, WhatsApp: search `8296276443` and `vikastirakannanavar@gmail.com`.
- Photos: replace the files in `images/` with new ones using the same file names.

## Add your edited videos (proof of work)
1. Copy the video into the `videos/` folder, for example `videos/client-a.mp4`. Keep each file under 25 MB, or upload to YouTube instead.
2. In `index.html`, search for `const VIDEOS=[];` and add entries:
```js
const VIDEOS=[
  {title:"Short-form edit — product launch", src:"videos/product-launch.mp4", poster:"images/product-launch-cover.jpg", vertical:true},
  {title:"Ad edit", youtube:"YOUTUBE_VIDEO_ID"}
];
```
3. Save. A "Video proof" section appears on the business page automatically. With no entries it stays hidden.

### What makes strong, safe proof
- Use a short before/after or final video sample that you created. Get the client's permission first; otherwise recreate the work with fictional/sample brand assets.
- For growth results, show a cropped analytics screenshot with the platform, date range, and metric visible. Hide account names, handles, customer data, ad spend, and private campaign details unless the client approved sharing them.
- Add a short case note: goal, your role, work delivered, time period, and the result. State the source and measurement period; use only numbers you can verify.
- If you cannot share client material, describe the work anonymously (for example, “Australian e-commerce brand”) and label any recreated visuals as sample work. Never imply a sample result belongs to a client.

## Deploy free with GitHub and Vercel
1. Create a GitHub repository named `vikas-portfolio` and push this folder's files to its `main` branch.
2. Sign in to Vercel with GitHub, choose **Add New → Project**, and import `vikas-portfolio`.
3. Keep the framework preset as **Other** and deploy the static site from the repository root. No build command is needed.
4. Vercel gives the site a free address ending in `.vercel.app`, for example `vikas-vt-portfolio.vercel.app` if that project name is available. Add `/#tech` or `/#growth` to share only that portfolio view.
5. Future pushes to `main` redeploy the site automatically.

Vercel's free subdomain is free to use. A custom domain such as `vikas.com` usually needs to be purchased separately; add it later under **Project → Settings → Domains**.

## Connect your own domain
1. Buy a domain from a registrar (Namecheap, GoDaddy, Hostinger, Cloudflare). A short, clean name works best, such as `vikastvt.com` or your full name.
2. In your hosting dashboard (Vercel, Netlify, etc.), open Domains and add the domain you bought.
3. It shows the DNS records to add. Open your registrar's DNS settings and add exactly those records.
4. Wait from a few minutes up to a day. HTTPS is turned on for you.

## Who has "admin access"
Nobody needs a separate admin panel. You control the site through three accounts:
- GitHub: edit files and upload videos (this is your editing dashboard)
- The hosting account (Vercel or similar): publishes changes and holds your domain settings
- The domain registrar: owns the domain name

Use a strong password and two-step login on all three.
