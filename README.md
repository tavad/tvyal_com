# **Tvyal.com Website Source**

This repository contains the source code for the new [tvyal.com](http://tvyal.com) website, built using the [Hugo](https://gohugo.io/) static site generator and the [Blowfish](https://blowfish.page/) theme.

## **Project Goal**

To create a modern, flexible, version-controlled website serving as a hub for Armenian data, showcasing weekly analyses, attracting B2B clients, and supporting multilingual content (Armenian, English, Russian).

## **Development**

* **Framework:** Hugo  
* **Theme:** Blowfish  
* **Content:** Markdown, RMarkdown (processed externally)  
* **Deployment:** GitHub Actions to GitHub Pages (initially)

## **Getting Started (Local Development)**

1. Ensure you have Hugo (extended version) installed.  
2. Clone the repository: git clone \<repository\_url\>  
3. Navigate into the directory: cd tvyal\_com\_hugo  
4. Install theme modules: hugo mod tidy  
5. Start the local server: hugo server  
6. Open your browser to http://localhost:1313/ (or the address provided by Hugo).