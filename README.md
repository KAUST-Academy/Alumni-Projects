# KAUST Academy Alumni Open Source Projects

A  collection of open source projects built by KAUST Academy alumni. This repository serves as a central hub linking to alumni projects hosted across GitHub, organized by topic and research area.

Each project folder is a Git submodule — a direct link to the alumni's own repository. This means you can browse all projects from one place, while each contributor maintains full ownership of their work.

---

## 📁 Repository Structure

Projects are organized into folders by topic (e.g., `VLMs/`, `NLP/`, `Computer-Vision/`). Each folder contains submodules linking to individual alumni repositories.

---

## 🚀 How to Clone This Repository

To clone this hub along with all linked alumni projects, run:

```bash
git clone --recurse-submodules https://github.com/KAUST-Academy/Alumni-Projects
```

If you already cloned it without `--recurse-submodules`, run:

```bash
git submodule update --init --recursive
```

---

## 🔄 How to Update All Submodules

Alumni projects are updated independently on their own repositories. To pull the latest changes from all linked projects into this hub, run:

```bash
git submodule update --remote
```

To update a specific project only, specify its path:

```bash
git submodule update --remote VLMs/ViC
```

After updating, commit and push the changes to keep the hub in sync:

```bash
git add .
git commit -m "Update submodules to latest commits"
git push
```

---

## 🤝 How to Add Your Project (Pull Request Guide)

Are you a KAUST Academy alumnus with an open source project? We'd love to include it! Follow these steps to submit a pull request:

### 1. Fork this repository
Click the **Fork** button at the top right of this page to create your own copy.

### 2. Clone your fork
```bash
git clone --recurse-submodules https://github.com/YOUR-USERNAME/YOUR-FORK-NAME
cd YOUR-FORK-NAME
```

### 3. Add your repository as a submodule
Place it in the most relevant topic folder. If a suitable folder doesn't exist, feel free to create one.

```bash
git submodule add https://github.com/YOUR-USERNAME/YOUR-PROJECT-REPO TOPIC-FOLDER/YOUR-PROJECT-NAME
```

For example:
```bash
git submodule add https://github.com/jane-doe/vision-transformer VLMs/vision-transformer
```

### 4. Commit your changes
```bash
git add .
git commit -m "Add YOUR-PROJECT-NAME by YOUR-NAME"
git push
```

### 5. Open a Pull Request
Go to your fork on GitHub and click **"Contribute" → "Open Pull Request"**. Please include the following in your PR description:

- **Your name, graduation year and program**
- **A short description of your project** (2–3 sentences)
- **The topic folder** you added it to and why

### ✅ Submission Requirements

- The repository must be **public**
- The project must have a **README** in its own repository
- The project must be related to your **work or research at KAUST Academy or KAUST**

