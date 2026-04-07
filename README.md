# Fantasy Island LLC — public site

Static site for **fantasyislandllc.com**, deployed with GitHub Actions to **Cloudflare Pages**.

## Local preview

```bash
cd site && python3 -m http.server 8765
```

Open http://127.0.0.1:8765/

## Deploy

1. In this GitHub repo: **Settings → Secrets and variables → Actions**  
   Add the same secrets you use for Colormac (or new token with Pages Edit):

   - `CLOUDFLARE_API_TOKEN`
   - `CLOUDFLARE_ACCOUNT_ID`

2. In **Cloudflare → Workers & Pages**: create a Pages project named **`fantasy-island-llc`** (or change `--project-name` in the workflow to match an existing project).

3. Attach custom domain **fantasyislandllc.com** to that Pages project.

4. Push to `main` (or **Actions → Run workflow**).

## Related

- **Dreamcycle** (app + dreamcycle.app): [pointever/alarm-clock](https://github.com/pointever/alarm-clock)
