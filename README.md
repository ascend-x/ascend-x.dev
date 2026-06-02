# 🚀 Ascend-X.dev | Cybersecurity Portfolio & Research Blog

> The personal portfolio and technical blog of **Nandakishore V**, a Penetration Tester, Cloud Security Engineer, and avid CTF competitor. 

Welcome to the source code for [ascend-x.dev](https://ascend-x.dev). This site is built to be more than just a resume—it is a deeply customized, interactive experience designed to showcase cybersecurity skills, cloud engineering architecture, and a passion for infosec.

---

## 🛠️ Architecture & Tech Stack

This project is engineered for maximum performance, security, and developer experience.

- **Framework**: [Astro](https://astro.build/) - For blazing-fast, static HTML generation with islands architecture.
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/) - Utility-first styling with modern optimizations.
- **Logic**: [TypeScript](https://www.typescriptlang.org/) - Strongly typed components and configuration.
- **Analytics**: [GoatCounter](https://www.goatcounter.com/) - A lightweight, open-source, and privacy-respecting analytics solution (Zero tracking pixels).
- **Search**: [Pagefind](https://pagefind.app/) - A static search engine indexing the site at build-time.
- **Hosting**: [Cloudflare Pages](https://pages.cloudflare.com/) - Global edge network deployment with automated CI/CD via npm.

---

## 🔥 Key Features & Highlights

This portfolio includes several unique, cybersecurity-themed features and easter eggs:

### 💻 The Interactive Terminal
An entirely custom, browser-based CLI built directly into the site.
- **Access:** Click the "TERMINAL" button in the bottom right, or use the keyboard shortcut `Ctrl + ~` (or `Ctrl + \``) to toggle it open.
- **Features:** A persistent state utilizing Astro View Transitions so your terminal session survives page navigations.
- **Commands:** Try typing `help`, `whoami`, `ls`, `cat contact.txt`, `decrypt ascendx`, `hack`, or `matrix`!

### 🌧️ Matrix Digital Rain Easter Egg
A hidden canvas animation globally integrated into the `Base.astro` layout.
- **Trigger:** Type the classic Konami Code anywhere on the site: `⬆ ⬆ ⬇ ⬇ ⬅ ➡ ⬅ ➡ B A`
- **Effect:** The screen will overlay a green "Matrix" falling digital rain effect. Type the code again to disable it.

### 🛑 Security Honeypot 404 Page
Standard "Page Not Found" errors are boring.
- If a user (or bot) attempts path traversal or requests an invalid route, they are met with a red **"SECURITY PROTOCOL BREACH"** warning, complete with simulated terminal logs logging their "unauthorized access attempt."

### 🕵️‍♂️ Advanced SEO & Bot Governance
Engineered to be perfectly parsed by search engines and modern AI crawlers.
- **`llms.txt`**: A custom markdown file in the root directory providing high-level context specifically formatted for Large Language Models.
- **`robots.txt` & `humans.txt`**: Strict bot crawling guidelines and author credits.
- **JSON-LD Schema**: Included in the `<head>` for rich Google search results (like the Sitelinks Search Box).
- **Dynamic Sitemap**: Automatically generated for all routes and blog posts.

### 🎨 Glitch Aesthetics
- Features custom CSS keyframe animations to create chromatic aberration "glitch" effects on hover for primary Call-To-Action buttons.
- A "decryption" text scramble effect on the homepage hero section on load.

---

## 🚀 Running Locally

Want to run the site on your own machine? It's simple.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ascend-x/ascend-x.dev.git
   cd ascend-x.dev
   ```

2. **Install dependencies:**
   *(Note: This project relies on `npm` and a strictly generated `package-lock.json` for Cloudflare compatibility. Do not use `pnpm`)*
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```
   *The site will be available at `http://localhost:4321`.*

4. **Test Production Build & Search:**
   Because Pagefind search relies on a built static index, search is disabled in dev mode. To test search locally:
   ```bash
   npm run build
   npm run preview
   ```

---

## 📝 Content Management

Blog posts, projects, and achievements are driven by Astro Content Collections.
- Add new Markdown (`.md`) or MDX (`.mdx`) files into the respective folders inside `src/content/`.
- Frontmatter schemas are strictly validated via Zod in `src/content.config.ts`.

---

## 🤝 Let's Connect
- **Email:** [nk.ascendx@gmail.com](mailto:nk.ascendx@gmail.com)
- **LinkedIn:** [linkedin.com/in/ascend-x](https://linkedin.com/in/ascend-x)
- **GitHub:** [github.com/ascend-x](https://github.com/ascend-x)
- **TryHackMe:** [tryhackme.com/p/ascendx001](https://tryhackme.com/p/ascendx001)
