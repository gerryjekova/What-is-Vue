# [How to Start the App](https://github.com/gerryjekova/What-is-Vue/blob/main/Docs/Project/WIV-1.md)
- Firstly I went to my [Custom GPT - Fifi](https://chatgpt.com/g/g-674259cb1c0881919c42c6a6d42ea0be-fifi).
> a Custom GPT is just ChatGPT with extra customizations tailored to specific needs. Fifi is my custom GPT that I have made for the purpose of studying, analysis, brainstorming & project management. I have trained her for these purposes, therefore I prefer to use her for this, rather than just normal ChatGPT. 
- The below part of the README is the first response I got after I requested a structured learning path for Vue JS before I start the tutorials on the basics. 
- There will be further commits with the steps I take broken down intuitively and I will also commit them step-by-step to make the processes I go through visible. 
- Do not take the below generated guide as a guideline for this project. The steps will be documented separately in a [Docs](https://github.com/gerryjekova/What-is-Vue/tree/main/Docs/AI-Brainstorming) dedicated directory with more .md files like this one and they will be linked here in the end. 
- Any future conversations with Fifi or any AI in regards to the project will also be stored in their own .md file in the [Docs](https://github.com/gerryjekova/What-is-Vue/tree/main/Docs/AI-Brainstorming) dedicated directory. 
- I now proceed to dissect the below study plan that was suggested by Fifi and commit onto the project. 
- I will be using VSCode as IDE. 
---

## 🚀 **Vue Learning Path (From Zero to "Render a Vue.js Design")**  

💡 **Goal**: Learn Vue **fast**, apply it in a well-documented GitHub repo, and demonstrate a Vue-rendered design effectively.  

### **⏳ Timeline & Strategy**  
1. **Day 1-2**: Core Vue concepts + Setup  
2. **Day 3**: Build a structured Vue project  
3. **Day 4**: Implement a design in Vue  
4. **Day 5**: Documentation + GitHub structuring  
5. **Final Day**: Polish & prepare for presentation  

---

### 📌 **Step-by-Step Guide**  

### **🟢 Step 1: Understanding Vue Basics (Day 1-2)**  
🔹 **What to Learn:**  
- Vue Instance & Reactivity (`data`, `methods`, `computed`, `watch`)  
- Vue Directives (`v-bind`, `v-model`, `v-if`, `v-for`, `v-on`)  
- Components & Props  
- Vue Lifecycle Hooks (`created`, `mounted`, etc.)  
- Simple API Fetching  

🔹 **What to Do:**  
✅ Set up Vue using Vite (faster dev experience)  
✅ Build a basic counter app with Vue’s reactivity (`v-model`, `v-on`)  
✅ Create a small API fetch example using `fetch()`  

🔹 **Resource:**  
- [Vue 3 Docs (Quick Start)](https://vuejs.org/guide/introduction.html)  

🔹 **GitHub Documentation:**  
📝 Create a `README.md` with:  
- **Project goal**: "Learning Vue from scratch to render a UI design"  
- **Tech Stack**: Vue 3 + Vite  
- **Day-by-day progress log**  

---

### **🟡 Step 2: Building a Vue Project Structure (Day 3)**  
🔹 **What to Learn:**  
- Vue Router (for navigation)  
- Vue Components (splitting UI into reusable parts)  
- Event Emitting (`$emit`) and Props  

🔹 **What to Do:**  
✅ Start a new project with Vue Router  
✅ Create a basic page navigation (`Home`, `About`, etc.)  
✅ Set up reusable components (e.g., `Button.vue`, `Navbar.vue`)  

🔹 **GitHub Documentation:**  
📌 Organize repo like:  
```
/my-vue-project
│── /src
│   │── /components
│   │   │── Button.vue
│   │   │── Navbar.vue
│   │── /views
│   │   │── Home.vue
│   │   │── About.vue
│   │── App.vue
│   │── main.js
│── README.md
│── package.json
```
📌 Create GitHub Issues:  
- **"Set up Vue Router"**  
- **"Create reusable components"**  

---

### **🔵 Step 3: Rendering a Vue Design (Day 4)**  
🔹 **What to Learn:**  
- CSS Framework (Tailwind or Bootstrap for speed)  
- Working with APIs in Vue  
- Handling form inputs (`v-model`, `v-bind`)  

🔹 **What to Do:**  
✅ Take a UI design (Figma or simple HTML/CSS template)  
✅ Break it into Vue components  
✅ Implement it in Vue (use `v-for`, `v-if` to handle dynamic parts)  
✅ Fetch & display data from an API  

🔹 **GitHub Documentation:**  
📌 Add a **"Rendering UI in Vue"** issue  
📌 Write detailed commits (`git commit -m "Added navbar component"`)  

---

### **🟣 Step 4: Clean Up, Document & Finalize (Day 5-6)**  
🔹 **What to Learn:**  
- Writing a strong `README.md`  
- GitHub Pages (if needed for deployment)  

🔹 **What to Do:**  
✅ Write clear documentation on:  
  - **Project Purpose**  
  - **How to Run It**  
  - **Features Implemented**  
✅ Create a `docs/` folder for additional notes  
✅ **Push to GitHub with well-structured commits**  
✅ **Test it & prepare to present it**  

---

## **📝 GitHub Documentation Tips**  
- **Use Issues & Milestones**: Track tasks clearly  
- **Write Clean Commits**: Example → `git commit -m "Added responsive navbar"`  
- **README.md Example Structure**:  
  ```markdown
  # Vue Learning Project  

  🚀 **Goal**: Learn Vue.js & render a UI design  

  ## Features  
  - Vue 3 + Vite setup  
  - Vue Router for navigation  
  - UI Components (Navbar, Cards, etc.)  
  - API Data Rendering  

  ## How to Run  
  ```sh
  npm install  
  npm run dev  
  ```
  ```

---

## **🎯 Final Notes & Next Steps**  
- **Make sure the UI actually works well** (no broken components)  
- **Be ready to explain how Vue reactivity works**  
- **Have a short demo script** (walk through components, show how it’s structured)  

---

> WIV = What Is Vue
# We came to a further conclusion that we are using Vue CLI in VSCode and I will begin the project with this. Will document the process and steps in regards to this in Docs/Project/WIV-1.md  


## **🛠 Step 1: Install Vue CLI**  
Since you already have **Node.js** installed, we’ll now install Vue CLI globally.  

### **1️⃣ Open VSCode & Terminal**  
- Open your terminal inside VSCode (`Ctrl + ~` or `Terminal > New Terminal`).  

### **2️⃣ Install Vue CLI**  
Run:  
```sh
npm install -g @vue/cli
```
This installs Vue CLI globally so you can use it anywhere.  

### **3️⃣ Verify the Installation**  
Check if Vue CLI installed correctly:  
```sh
vue --version
```
You should see a version number (e.g., `@vue/cli 5.x.x`). If you get an error, let me know.  



## **🛠 Step 2: Create a New Vue Project**  
Now, let’s create your Vue project.  

### **1️⃣ Run the Project Creation Command**  
```sh
vue create my-vue-project
```
It will ask you to choose a preset:  
- **Select "Manually select features"** (this gives us control).  
- Use the arrow keys to choose features:  
  - ✅ **Babel** (needed for JS compatibility)  
  - ✅ **Vue Router** (for navigation)  
  - ✅ **Vuex** (state management, optional but good to know)  
  - ✅ **ESLint** (code quality, optional)  
  - (Skip TypeScript unless you want it)  
- **Press Space to select** a feature, then **Enter** to continue.  



## **🛠 Step 3: Move Into the Project & Start It**  
After Vue CLI sets up the project, navigate into it:  
```sh
cd my-vue-project
```
Run the development server:  
```sh
npm run serve
```
You should see:  
```
App running at:
http://localhost:8080/
```
Open that in your browser—you should see the default Vue welcome page! 🎉  



## **🛠 Step 4: Open in VSCode & Set Up Git**  
1️⃣ Open the project in VSCode:  
```sh
code my-vue-project
```
2️⃣ Initialize Git:  
```sh
git init
git add .
git commit -m "Initial commit - Set up Vue CLI project"
```
3️⃣ If you haven’t created a GitHub repo yet, do so at [GitHub](https://github.com/) and get the repo link. Then link your local repo:  
```sh
git remote add origin <your-github-repo-url>
git branch -M main
git push -u origin main
```



## **🛠 Step 5: Project Structure Overview**  
Your project now has this structure:  
```
/my-vue-project
│── /src
│   │── /assets
│   │── /components  <-- Where you'll create Vue components
│   │── /views       <-- Where you'll define pages (if using Vue Router)
│   │── App.vue      <-- Main component
│   │── main.js      <-- Entry point
│── /public
│── index.html
│── package.json
│── README.md
```
Now Vue is **installed, running, and linked to GitHub**.  



### **📌 Next Steps**
1️⃣ **Confirm the Vue app runs at `localhost:8080`.**  
2️⃣ **Push everything to GitHub** and check that the repo is updated.  
3️⃣ **Start learning Vue basics**—I’ll guide you next.  