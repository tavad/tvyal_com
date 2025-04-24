# **Tvyal.com Website Source**
This repository contains the source code for the new [tvyal.com](http://tvyal.com) website, built using the [Hugo](https://gohugo.io/) static site generator and the [Blowfish](https://blowfish.page/) theme.

## **Project Goal**
To create a modern, flexible, version-controlled website serving as a hub for Armenian data, showcasing weekly analyses, attracting B2B clients, and supporting multilingual content (Armenian, English, Russian).

## **Features**
- Multilingual content (Armenian, English, Russian)
- Interactive data visualizations
- Armenian data hub with downloadable datasets
- FX rates monitoring and visualization
- Weekly economic and data analysis newsletter
- B2B data science services showcase

## **Technology Stack**
- **Framework:** Hugo (Extended Version)
- **Theme:** Blowfish
- **Content:** Markdown, RMarkdown (processed externally)
- **Data Processing:** R scripts
- **Visualization:** Plotly.js, ECharts.js
- **Deployment:** GitHub Actions to GitHub Pages (initially)

## **Getting Started (Local Development)**
1. Ensure you have Hugo Extended version installed (minimum v0.146.7+extended)
2. Clone the repository:
   ```
   git clone <repository_url>
   ```
3. Navigate into the directory:
   ```
   cd tvyal_hugo
   ```
4. Download theme dependencies:
   ```
   hugo mod get -u
   ```
5. Start the local server:
   ```
   hugo server
   ```
6. Open your browser to http://localhost:1313/ (or the address provided by Hugo)

## **Project Structure**
- **content/**: All website content organized by sections
  - **newsletter/**: Weekly analysis posts
  - **data-hub/**: Armenian data catalog and documentation
  - **fx-rates/**: Exchange rate visualization pages
  - **services/**: B2B service descriptions
  - **about/**: Company information
  - **contact/**: Contact information
- **static/**: Static files like images, downloadable data files
- **layouts/**: Custom templates and shortcodes
- **assets/**: CSS, JS, and other project assets
- **config/**: Site configuration files

## **Content Management Workflow**
1. Create RMarkdown files for newsletters and analyses
2. Process these files with R to:
   - Extract static plots and save as images
   - Extract text content as Markdown
   - Generate separate HTML files for interactive plots
3. Place Markdown in content/newsletter/
4. Place static images in static/images/
5. Place interactive HTML files in static/interactive/

## **Multilingual Support**
The site supports three languages with content and UI translation:
- English (en) - Default
- Armenian (hy)
- Russian (ru)

Language files are in i18n/ directory and language-specific content uses language codes in filenames (e.g., _index.en.md, _index.hy.md).

## **Deployment**
The site is automatically deployed when changes are pushed to the main branch using GitHub Actions. The workflow:
1. Checks out the repository
2. Sets up R and dependencies
3. Runs data generation scripts
4. Builds the Hugo site
5. Deploys to GitHub Pages
