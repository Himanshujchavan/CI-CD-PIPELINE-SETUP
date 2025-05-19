#  CI/CD PIPELINE SETUP
COMPANY : CODETECH IT SOLUTION

NAME :Himanshu Jagannath chavan

Intern ID: CT04DK145

Domain : DevOps

Duration : 4 weeks

Mentor : NEELA SANTOSH

---

# 🎵 Spotify Web Clone

A simple Spotify-inspired music player built using **HTML, CSS, and JavaScript**. 
This project includes **CI/CD automation** using **GitHub Actions** to deploy the site on **GitHub Pages**.

---

## 📁 Project Structure

.
├── index.html  
├── style.css  
├── script.js  
├── songs/  
│   ├── song1.mp3  
│   └── song2.mp3  
├── .github/  
│   └── workflows/  
│       └── deploy.yml  
└── README.md

---

## 💻 How to Run the Project Locally

1. Clone the repository:

   https://github.com/Himanshujchavan/CI-CD-PIPELINE-SETUP.git 
   cd CI-CD-PIPELINE-SETUP

2. Open `index.html` in your browser:

   - Option 1: Double-click on `index.html`
   - Option 2: Run a local server:

     Using Node.js:
     npx serve .

     Using Python:
     python3 -m http.server

3. Enjoy your local music player! 🎧

---

## 🚀 CI/CD with GitHub Actions

This project uses GitHub Actions to automatically deploy the site to GitHub Pages on every push to the `main` branch.

### 🔄 Workflow File Path

`.github/workflows/deploy.yml`

### Workflow Configuration:

name: Deploy Spotify Clone to GitHub Pages  
on:  
  push:  
    branches:  
      - main

jobs:  
  build-and-deploy:  
    runs-on: ubuntu-latest  
    steps:  
      - name: Checkout Code  
        uses: actions/checkout@v3  
      - name: Deploy to GitHub Pages  
        uses: peaceiris/actions-gh-pages@v3  
        with:  
          github_token: ${{ secrets.GITHUB_TOKEN }}  
          publish_dir: ./

### ⚙️ How It Works

- When code is pushed to `main`, GitHub triggers the workflow.
- It checks out the code and deploys it to the `gh-pages` branch.
- GitHub Pages then serves the website from the `gh-pages` branch.

---

## 🌐 Deployment

1. Go to your GitHub repository → **Settings** → **Pages**
2. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
3. Access your deployed website at:

   https://himanshujchavan.github.io/CI-CD-PIPELINE-SETUP/

---

## 📸 Screenshots :
## Dark Mode:
![Image](https://github.com/user-attachments/assets/f650dcb0-961b-4fa2-b7e3-0230b3835e5a)

## vgitLight Mode:
![Image](https://github.com/user-attachments/assets/5c39f9e9-b5b5-4fe5-8dc6-0af3c0e7a4f3)

---


