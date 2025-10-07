# GitHub Wiki Setup Guide

This directory contains comprehensive documentation for the SysDev Genkit Workshop as GitHub Wiki pages.

## 📚 Wiki Pages

1. **[Home](Home.md)** - Overview and navigation
2. **[Getting Started](Getting-Started.md)** - Setup and installation guide  
3. **[Genkit Concepts](Genkit-Concepts.md)** - Understanding core Genkit features
4. **[Flows Guide](Flows-Guide.md)** - Detailed flow documentation
5. **[Tools and Prompts](Tools-and-Prompts.md)** - Tools and prompts reference
6. **[API Reference](API-Reference.md)** - REST API documentation
7. **[Workshop Exercises](Workshop-Exercises.md)** - Hands-on coding exercises
8. **[Advanced Topics](Advanced-Topics.md)** - Advanced patterns and techniques
9. **[Troubleshooting](Troubleshooting.md)** - Common issues and solutions
10. **[FAQ](FAQ.md)** - Frequently Asked Questions

## 🚀 Setting Up GitHub Wiki

### Option 1: Enable GitHub Wiki (Recommended)

1. **Go to your GitHub repository**
2. **Click on Settings** → **Features**
3. **Enable "Wikis"**
4. **Clone the wiki repository:**
   ```bash
   git clone https://github.com/<username>/<repo>.wiki.git
   ```
5. **Copy wiki files:**
   ```bash
   cp wiki/*.md <repo>.wiki/
   cd <repo>.wiki/
   git add .
   git commit -m "Add comprehensive workshop wiki"
   git push origin master
   ```

### Option 2: Use as Docs Folder

1. **Keep in the `wiki/` directory**
2. **Link from main README.md:**
   ```markdown
   ## Documentation
   - [Getting Started](wiki/Getting-Started.md)
   - [Full Wiki Index](wiki/Home.md)
   ```
3. **GitHub will automatically render the markdown files**

### Option 3: GitHub Pages

1. **Create a `docs/` folder:**
   ```bash
   mkdir docs
   cp wiki/*.md docs/
   ```
2. **Enable GitHub Pages** in Settings → Pages
3. **Select source:** `main` branch, `/docs` folder
4. **Add a `_config.yml` in docs:**
   ```yaml
   theme: jekyll-theme-minimal
   title: SysDev Genkit Workshop
   description: Comprehensive guide for learning Genkit
   ```

## 📖 Navigation Structure

```
Home.md (Landing page)
├── Getting Started
│   ├── Prerequisites
│   ├── Installation
│   └── First Steps
├── Core Concepts
│   ├── Genkit Concepts
│   ├── Flows Guide
│   └── Tools and Prompts
├── Development
│   ├── API Reference
│   └── Workshop Exercises
├── Advanced
│   ├── Advanced Topics
│   └── Production Patterns
└── Help
    ├── Troubleshooting
    └── FAQ
```

## ✨ Features

### Comprehensive Coverage
- ✅ Complete setup guide
- ✅ Core concepts explained
- ✅ Step-by-step exercises
- ✅ API documentation
- ✅ Troubleshooting guide
- ✅ Advanced topics
- ✅ Production patterns

### Student-Friendly
- 🎯 Clear learning objectives
- ⏱️ Time estimates for exercises
- 📝 Code examples everywhere
- ✅ Verification steps
- 🚀 Challenge variations
- 🆘 Detailed troubleshooting

### Production-Ready
- 🔐 Security best practices
- ⚡ Performance optimization
- 📊 Observability patterns
- 🧪 Testing strategies
- 🚀 Deployment guides

## 🛠️ Customization

### Update Wiki Content

Edit any `.md` file in this directory and push changes:

```bash
cd wiki/
# Edit files
git add .
git commit -m "Update wiki content"
git push
```

### Add New Pages

1. **Create new markdown file:**
   ```bash
   touch wiki/New-Page.md
   ```

2. **Add content with proper heading:**
   ```markdown
   # New Page Title
   
   Content here...
   ```

3. **Link from Home.md:**
   ```markdown
   - [New Page](New-Page)
   ```

4. **Link from related pages**

### Sidebar Navigation (GitHub Wiki)

If using GitHub Wiki, create a `_Sidebar.md`:

```markdown
## Navigation

**Getting Started**
- [Home](Home)
- [Setup](Getting-Started)

**Core Concepts**
- [Genkit Basics](Genkit-Concepts)
- [Flows](Flows-Guide)
- [Tools & Prompts](Tools-and-Prompts)

**Development**
- [API Reference](API-Reference)
- [Exercises](Workshop-Exercises)

**Advanced**
- [Advanced Topics](Advanced-Topics)

**Help**
- [Troubleshooting](Troubleshooting)
- [FAQ](FAQ)
```

### Footer (GitHub Wiki)

Create `_Footer.md`:

```markdown
---
💡 **Need help?** Check [Troubleshooting](Troubleshooting) | [FAQ](FAQ) | [GitHub Issues](https://github.com/username/repo/issues)
```

## 📝 Maintenance

### Keep Wiki Updated

When you update the codebase, update relevant wiki pages:

**Code Changes → Wiki Updates:**
- New flow → Update [Flows Guide](Flows-Guide.md)
- New tool → Update [Tools and Prompts](Tools-and-Prompts.md)
- API changes → Update [API Reference](API-Reference.md)
- Bug fixes → Update [Troubleshooting](Troubleshooting.md)

### Review Schedule

- **Weekly:** Check for outdated links and code examples
- **Monthly:** Review and update exercises
- **Quarterly:** Update dependencies and best practices

## 🤝 Contributing

Students and contributors can improve the wiki:

1. **Fork the repository**
2. **Create a branch:**
   ```bash
   git checkout -b improve-wiki-docs
   ```
3. **Make changes to wiki files**
4. **Submit a pull request**

### Contribution Guidelines

- ✅ Clear, concise explanations
- ✅ Working code examples
- ✅ Proper markdown formatting
- ✅ Cross-reference related pages
- ✅ Test all code snippets
- ❌ Don't break existing links
- ❌ Don't remove content without discussion

## 📊 Wiki Statistics

- **Total Pages:** 10
- **Code Examples:** 100+
- **Exercises:** 10+
- **Estimated Reading Time:** 4-6 hours
- **Hands-on Practice Time:** 8-12 hours

## 🎓 Learning Paths

### For Beginners (8-12 hours)
1. [Getting Started](Getting-Started.md) - 1h
2. [Genkit Concepts](Genkit-Concepts.md) - 2h
3. [Flows Guide](Flows-Guide.md) - 2h
4. [Workshop Exercises](Workshop-Exercises.md) 1-5 - 5h
5. [Troubleshooting](Troubleshooting.md) - As needed

### For Intermediate (6-8 hours)
1. [Genkit Concepts](Genkit-Concepts.md) - 1h
2. [Flows Guide](Flows-Guide.md) - 1h
3. [Tools and Prompts](Tools-and-Prompts.md) - 1h
4. [Workshop Exercises](Workshop-Exercises.md) 1-10 - 4h
5. [API Reference](API-Reference.md) - 1h

### For Advanced (4-6 hours)
1. [Advanced Topics](Advanced-Topics.md) - 2h
2. [Workshop Exercises](Workshop-Exercises.md) Bonus - 2h
3. Build custom features - 2h

## 🔗 External Resources

Complement this wiki with:
- [Official Genkit Docs](https://firebase.google.com/docs/genkit)
- [Genkit GitHub](https://github.com/firebase/genkit)
- [Google AI Studio](https://makersuite.google.com/)
- [OpenAI Platform](https://platform.openai.com/)

## 📄 License

This documentation is part of the SysDev Genkit Workshop project. See LICENSE file for details.

---

**Ready to start?** Begin with [Getting Started](Getting-Started.md) →

