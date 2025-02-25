# 🌍 European Network for Science of Science - Website  

Welcome to the website repository for the **[European Network for Science of Science](git@github.com:EU-Network-for-the-Science-of-Science/euroscisci.git)**!  
This site was developed during the `hackaton` at **2025 workshop** of the Network, organized by [Justin Sulik](http://justinsulik.com/) at MI3/LMU.

The EuroScisci project builds on a series of [scientific workshops (2022-2023)](https://blogs.helsinki.fi/computational-science-studies/) organized by [Jacob Habinek](https://www.jacobhabinek.net/) (The Institute for Analytical Sociology, Linköping University), [Pantelis Analytis](https://www.sdu.dk/en/forskning/forskningsenheder/samf/sod/simple-employee-list-sod/group-members/pantelis-analytis) (Danish Institute of Advanced Studies, University of Southern Denmark) and [Samuli Reijula](https://www.samulireijula.net/) (TINT/Theoretical Philosophy, University of Helsinki).

## 📌 Overview  
This repository contains everything you need to download, set up, and run the website locally.  

The website is built using the **[Hugo](https://gohugo.io/)** static site generator and follows the **[Hugoplate](https://github.com/zeon-studio/hugoplate)** template.  

---

## ⚙️ Prerequisites  
Before proceeding, ensure you have installed the following dependencies:  

- 🏗 **Hugo Extended** `v0.124+` → [Installation Guide](https://gohugo.io/installation/)  
- 🚀 **Node.js** `v20+` → [Download Node.js](https://nodejs.org/)  
- 🏎 **Go** `v1.22+` → [Get Go](https://go.dev/dl/)  

---

## 📥 Download the Repository  
Navigate to the folder where you want to store the website, then run:  

```bash
git clone git@github.com:EU-Network-for-the-Science-of-Science/euroscisci.git
```

## 🛠 Project Setup & Install Dependencies  
Open a terminal in the project folder and execute:  

```bash
npm run project-setup
```

Then, install the required dependencies:  

```bash
npm install
```

---

## 🚀 Run the Website Locally  
To preview the site on your local machine, run:  

```bash
hugo server -D
```

Then, open **[http://localhost:1313/euroscisci/](http://localhost:1313/euroscisci/)** in your browser to view the site.  

---

📢 *For additional details and customization, refer to the project's documentation or the Hugo official guides.*  

## How to add new members

🗂 Navigate to the members folder
```bash
cd content\english\members
```

📄 Create a Markdown file with the name of the member

```bash
touch firstname_lastname.md
```

✍️ Copy and paste the following content into the new file and complete with the correct information
```
---
title: FirstName LastName
email: FirstName.LastName@example.com
image: "/images/profiles/FirstNameLastName.jpg"
website: https://LastName.com/
description: Researcher | Data Science | AI
social:
  # - name: github
  #   icon: fa-brands fa-github
  #   link: https://www.github.com/FirstNameLastName

   - name: linkedin
     icon: fa-brands fa-linkedin
     link: https://www.linkedin.com/in/FirstNameLastName
  
  - name: google scholar
    icon: fab fa-google-scholar
    link: https://scholar.google.com/citations?user=XXXXXXXXXX

  - name: email
    icon: fa fa-envelope
    link: mailto:FirstName.LastName@example.com

  - name: website
    icon: fa fa-globe
    link: https://LastName.com/
---
```
💾 Save your changes

If you are using the online interface on GitHub, remember to save the file.
If you are working locally, run the following commands:
```bash
git add firstname_lastname.md
```
```bash
git commit -m "adding new member"
git pull
git push
```
