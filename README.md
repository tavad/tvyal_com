# Tvyal.com Hugo Website

This repository contains the source code for the Tvyal.com website, built with Hugo and the Congo theme.

## Project Overview

Tvyal.com is a hub for Armenian data (economic, social, demographic, etc.) and showcases data analysis expertise to attract B2B clients for data science services.

## Setup Status

### Phase 0: Preparation & Foundation (Setup) - COMPLETED
- [x] Install Git
- [x] Verify & Update Hugo: Hugo v0.146.7+extended installed
- [x] Create GitHub Repository: tvyal_com created on GitHub
- [x] Initialize Hugo Project: tvyal_hugo directory created, git init run
- [x] Add Congo Theme & Configure: Theme installed directly in themes directory
- [x] Basic Site Configuration: Created hugo.toml with necessary settings
- [x] Initial Commit: Done (README.md, .gitignore, initial Hugo files)
- [x] Push to GitHub: Repository successfully pushed to GitHub

### Phase 1: Basic Site Structure & Layout - IN PROGRESS
- [ ] Define Site Structure based on vision:
  - Home (potentially featuring FX highlights)
  - Newsletter / Blog (weekly analysis)
  - Armenian Data Hub (data catalog/downloads)
  - FX Rates (dedicated interactive page)
  - Services (B2B offerings)
  - About
  - Contact
- [ ] Create Section Placeholders
- [ ] Configure Navigation
- [ ] Configure Basic Theme Options
- [ ] Test Locally
- [ ] Commit Changes

## Development

To run the development server:

\`\`\`bash
hugo server
\`\`\`

## Technology Stack

- Static Site Generator: Hugo (v0.146.7+extended)
- Theme: Congo (installed in themes directory)
- Version Control: Git / GitHub
- Deployment: GitHub Actions deploying to GitHub Pages (planned)
- Primary Content Language: R / RMarkdown (for analysis)
- Database (for dynamic data): Plan to use PostgreSQL or DuckDB
- Future Backend (API/Login): Likely Go or Python
