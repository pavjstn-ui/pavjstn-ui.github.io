# pavjust-site

Minimal personal CV/portfolio — single static HTML file, no build step.

## Deploy to GitHub Pages

1. Create a new repo on GitHub: `pavjstn-ui/pavjstn-ui.github.io`  
   (or any repo name, e.g. `pavjstn-ui/site`)
2. Push this directory to the `main` branch
3. Go to **Settings → Pages**
4. Under **Source**, select **Deploy from a branch**
5. Branch: `main` · Folder: `/ (root)` → **Save**
6. Site will be live at `https://pavjstn-ui.github.io` (or the repo subdomain) within ~60 seconds

### Custom domain (optional)

1. Add a `CNAME` file to this directory containing your domain, e.g. `pavoljust.dev`
2. In Settings → Pages → Custom domain, enter the same domain
3. Point your DNS: `CNAME www → pavjstn-ui.github.io` (or A records for apex)
4. Enable **Enforce HTTPS** once the cert provisions

## Local preview

```bash
open index.html
# or
python3 -m http.server 8080
```
