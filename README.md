## Updating, Rebuilding, and Redeploying Your Astro Site

1. **Add or Update Static Files (e.g., PDFs, images):**
   - Place new static files in the `public/` directory (e.g., `public/cv/yourfile.pdf`).

2. **Install dependencies (if needed):**
   ```sh
   npm install
   ```

3. **Update lock file if you change dependencies:**
   ```sh
   npm install
   git add package-lock.json
   git commit -m "Update lock file to match package.json"
   git push
   ```

4. **Build the site:**
   ```sh
   npm run build
   ```

5. **Deploy to GitHub Pages (if not using Actions):**
   ```sh
   npx gh-pages -d dist
   ```
   - This pushes the contents of `dist/` to the `gh-pages` branch.

6. **If using GitHub Actions:**
   - Just commit and push your changes. The workflow will build and deploy automatically.

7. **Check your site:**
   - Visit your custom domain or the default GitHub Pages URL to verify updates. 