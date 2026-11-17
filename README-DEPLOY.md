# QuickTools Hub Version 4 — Tools Expansion Edition

## What's included
- Updated `index.html`, based on the previous Version 3 project.
- 10 new tools: solid-color background eraser, PDF merge/extract/rotate, resume builder, social image resizer, invoice generator, HEIC converter, barcode generator, browser text-to-speech, JSON/CSV converter and password strength checker.
- 10 SEO landing pages under `tools/` with distinct titles, descriptions, canonical URLs, FAQs and links to the corresponding tool.
- `robots.txt` and `sitemap-template.xml`.

## Deploy to GitHub Pages
1. Download and extract this ZIP.
2. Open your GitHub repository `mzcrussell/megatools`.
3. Replace the repository's existing files with the contents of this folder. Keep the folder structure, especially `tools/`.
4. Commit to the branch/folder configured in GitHub Pages.
5. Wait for the Pages deployment to finish, then test the homepage and every new tool.

## Custom domain setup (domain name not supplied yet)
1. Buy/register your chosen domain with a registrar.
2. In GitHub: Repository → Settings → Pages → Custom domain, enter the exact domain and save.
3. Configure DNS at your registrar using GitHub's current Pages instructions. Commonly this means A records for an apex domain or a CNAME for `www`; use the exact records GitHub shows for your repository.
4. After GitHub verifies the domain, enable Enforce HTTPS.
5. Add a root-level file named `CNAME` containing only your exact domain name. Do not use the example placeholder.
6. Update canonical URLs and Open Graph URLs in `index.html` and all `tools/*/index.html` pages.
7. Replace `YOUR-DOMAIN.com` in `sitemap-template.xml`, save it as `sitemap.xml`, then update the Sitemap line in `robots.txt`.
8. Submit `https://YOUR-DOMAIN.com/sitemap.xml` in Google Search Console.

## Analytics
No tracking ID has been invented or embedded. Create a GA4 property, copy your Measurement ID (`G-XXXXXXXXXX`), then add Google's official tag only after reviewing your privacy/cookie notice and applicable consent requirements.

## Important technical notes
- The background eraser removes a sampled near-uniform color; it is not AI background segmentation.
- PDF tools merge, extract and rotate. They do not promise aggressive image compression. Password-protected PDFs may fail.
- Text-to-speech uses voices available from the browser/OS and does not export MP3.
- HEIC conversion depends on the browser and external HEIC conversion library.
- Some libraries are loaded from CDNs; an internet connection is required for those tools.
- All SEO pages are English starter content. Add genuinely useful, reviewed localized content before publishing translated pages.
- Do not add fake reviews, doorway pages, keyword stuffing or guaranteed ranking claims. Search ranking and traffic are never guaranteed.

## Contact placeholder
The old V3 file contained `YOUR-EMAIL@example.com`. Replace that placeholder in the contact section with an email address you actively monitor before launch.
