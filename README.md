# sitemap-crawler

Verify the status of each url in a (hosted) sitemap XML file, by crawling through the XML and fetching it to see if returns a 200 OK. Free alternative to Screaming Frog SEO Spider's paid sitemap crawler feature.

https://github.com/dylancl/sitemap-scraper/assets/14956708/d15b02a0-351a-43fd-a91e-90c042603075


# Installation

1. Clone the repository

   ```bash
   git clone https://github.com/dylancl/sitemap-scraper.git
   ```

2. Install the dependencies

   ```bash
   pnpm install
   ```

3. Run the script

   ```bash
   pnpm start
   ```

# Usage

1. Enter the URL of the sitemap XML file you want to check.
2. The script will ask you for configuration options:
   - **Concurrency limit**: The maximum number of requests that can be made at the same time. Default is 5. Must be a number between 1 and 15.
   - **Request delay**: The delay between each request. Default is 1000. Must be a number starting from 250.
   - **Traversal order**: The order in which the URLs will be checked. Default is `sequential`. Options are `sequential` and `random`.
3. The script will start checking the URLs and display the progress in the console.
4. When the script is done, it will ask you if you want to save the results (ok & not ok URLs) to a file.

