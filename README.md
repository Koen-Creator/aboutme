# AboutMe Jekyll Blog

This repository is a personal blog powered by [Jekyll](https://jekyllrb.com/) using the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) theme. It provides a minimal, modern, and fast static site for sharing posts, projects, and personal information.

## Features
- **Chirpy Theme**: Clean, responsive, and feature-rich Jekyll theme.
- **Blog Posts**: Write and manage posts in Markdown under the `_posts/` directory.
- **Custom Pages**: Add custom tabs and pages in the `_tabs/` directory.
- **Live Reload**: Development server with live reload for fast editing.
- **SEO & Social**: Built-in SEO, sitemap, and social sharing support.

## Project Structure
```
.
├── _config.yml         # Main configuration file
├── _data/              # Data files (contact, share info)
├── _plugins/           # Custom Jekyll plugins
├── _posts/             # Blog posts (Markdown)
├── _site/              # Generated static site (output)
├── _tabs/              # Custom navigation tabs/pages
├── assets/             # CSS, images, and libraries
├── tools/              # Helper scripts (run.sh, test.sh)
├── index.html          # Home page
├── Gemfile             # Ruby gem dependencies
└── README.md           # Project documentation
```


## Getting Started

### 1. Create Your Site Repository

You can start your blog in two ways:

- **Using the Starter Template (Recommended):**
   1. Go to the [Chirpy Starter](https://github.com/cotes2020/chirpy-starter) repository.
   2. Click "Use this template" and create a new repository named `<username>.github.io`.

- **Forking the Theme (For Advanced Users):**
   1. Fork the [Chirpy Theme](https://github.com/cotes2020/jekyll-theme-chirpy) repository.
   2. Name your new repository `<username>.github.io`.

### 2. Setting Up the Environment

- **Dev Containers (Recommended for Windows):**
   - Install Docker and VS Code with the Dev Containers extension.
   - Clone your repository and open it in a container using VS Code.

- **Native Setup (Recommended for Unix-like OS):**
   1. Install [Jekyll](https://jekyllrb.com/docs/installation/) and [Git](https://git-scm.com/).
   2. Clone your repository.
   3. Run `bundle install` to install dependencies.

### 3. Usage

- **Start the Jekyll Server:**
   ```sh
   bundle exec jekyll serve
   ```
   The site will be available at [http://127.0.0.1:4000](http://127.0.0.1:4000/).

- **Configuration:**
   - Edit `_config.yml` for site settings (URL, avatar, timezone, language, etc.).
   - Update social contacts in `_data/contact.yml`.

- **Customizing Styles:**
   - To override styles, copy `assets/css/jekyll-theme-chirpy.scss` and add your custom CSS at the end.

### 4. Deployment

- **GitHub Actions (Recommended):**
   - Push your changes to GitHub.
   - Configure GitHub Pages to use GitHub Actions as the build source.
   - If you use a non-Linux system, run:
      ```sh
      bundle lock --add-platform x86_64-linux
      ```
   - Your site will be deployed automatically.

- **Manual Deployment:**
   - Build the site:
      ```sh
      JEKYLL_ENV=production bundle exec jekyll b
      ```
   - Upload the contents of the `_site` directory to your server.

## Writing Posts
- Add new Markdown files to the `_posts/` directory. Follow the naming convention: `YYYY-MM-DD-title.md`.
- Customize navigation tabs in the `_tabs/` directory.

## Customization
- Edit `_config.yml` to update site settings, author info, and theme options.
- Add or update data files in `_data/` for contact and sharing information.

## License
This project is licensed under the [MIT License](LICENSE).
