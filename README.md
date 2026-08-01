<p align="center">
  <img src="./public/readme-logo.svg" alt="simple-quora-blog logo" width="96" height="96" />
</p>

<h1 align="center">Simple-Quora-Blog</h1>

<p align="center"><i>A simple Quora-style blog app built with Express, EJS, and RESTful routes.</i></p>

<p align="center">
	<img src="https://img.shields.io/badge/VERSION-1.0.0-E11D48?style=for-the-badge" alt="Version 1.0.0" />
	<img src="https://img.shields.io/badge/LICENSE-GPLv3-2563EB?style=for-the-badge" alt="GPLv3 License" />
	<img src="https://img.shields.io/badge/TYPE-CRUD%20BLOG-7C3AED?style=for-the-badge" alt="CRUD Blog" />
</p>

<p align="center">
	<img src="https://img.shields.io/badge/NODE.JS-APP-22C55E?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js App" />
	<img src="https://img.shields.io/badge/EXPRESS-4.x-7C3AED?style=for-the-badge&logo=express&logoColor=white&labelColor=5B21B6" alt="Express 4.x" />
	<img src="https://img.shields.io/badge/EJS-TEMPLATES-0EA5E9?style=for-the-badge" alt="EJS Templates" />
	<img src="https://img.shields.io/badge/METHOD--OVERRIDE-REST%20FORMS-9333EA?style=for-the-badge" alt="Method Override" />
</p>

<p align="center">
  <a href="#-project-intro"><img src="https://img.shields.io/badge/EXPLORE-PROJECT%20INTRO-6366F1?style=for-the-badge" alt="Project Intro" /></a>
  <a href="#️-install-methods"><img src="https://img.shields.io/badge/SETUP-INSTALL%20GUIDE-14B8A6?style=for-the-badge" alt="Install Guide" /></a>
  <a href="#-available-scripts"><img src="https://img.shields.io/badge/RUN-SCRIPTS-A855F7?style=for-the-badge" alt="Scripts" /></a>
</p>


## Table of Contents

- [🚀 Project intro](#-project-intro)
- [📁 Project structure](#-project-structure)
- [🔧 Features](#-features)
- [🧰 Tech stack](#-tech-stack)
- [⚙️ Install methods](#️-install-methods)
	- [📦 npm / Node](#-npm--node)
- [🛣️ Routes](#️-routes)
- [📜 Available scripts](#-available-scripts)
- [📄 License](#-license)

## 🚀 Project intro

`simple-quora-blog` is a beginner-friendly REST-style CRUD app with:

- Create post
- Read all posts and single post
- Edit post content
- Delete post
- In-memory data storage using a local array

This project is ideal for practicing Express routing, EJS templating, and `method-override`.

## 📁 Project structure

```txt
Simple-Quora-Blog/
├── index.js
├── package.json
├── README.md
├── LICENSE
├── public/
│   └── style.css
└── views/
		├── index.ejs
		├── form.ejs
		├── show.ejs
		└── edit.ejs
```

## 🔧 Features

| Feature | Status | Notes |
| --- | --- | --- |
| List posts | ✅ Current | Displays all posts at `/posts` |
| Create post | ✅ Current | Form submission adds a post with generated UUID |
| View single post | ✅ Current | Shows post detail by id |
| Edit post | ✅ Current | Updates post content using `PATCH` |
| Delete post | ✅ Current | Removes post using `DELETE` |

## 🧰 Tech stack

- **Runtime:** Node.js
- **Server:** Express.js
- **Template engine:** EJS
- **Method support:** method-override
- **ID generation:** uuid
- **Styling:** Plain CSS

## ⚙️ Install methods

### 📦 npm / Node

Prerequisites:

- Node.js 18+
- npm

```bash
git clone <your-repo-url> Simple-Quora-Blog
cd Simple-Quora-Blog
npm install
```

Start the server:

```bash
node index.js
```

Open `http://localhost:8080/posts`.

## 🛣️ Routes

- `GET /posts` → show all posts
- `GET /posts/form` → create post form
- `POST /posts` → create a new post
- `GET /posts/:id` → show a single post
- `GET /posts/:id/edit` → edit form for a post
- `PATCH /posts/:id` → update post content
- `DELETE /posts/:id` → delete a post

## 📜 Available scripts

```bash
npm test
```

Current `test` script is a placeholder and exits with an error by default.

## 📄 License

This project is licensed under the GNU GPL v3.
See the `LICENSE` file for details.
