## Portfolio Update Checklist (`index.html`)

### 1. Adding a New Project
* **Where:** Inside `<script>` -> `PROJECTS` array
* **Template:**
  ```javascript
  {
    tag: "CATEGORY TAG",
    tagStyle: "cyan", // "cyan", "emerald", or "indigo"
    category: "TECH • STACK",
    title: "Project Title",
    description: "Short description of what the project does.",
    tech: ["Tech 1", "Tech 2", "Tech 3"],
    githubUrl: "[https://github.com/vikramrakr/repo-name](https://github.com/vikramrakr/repo-name)",
    liveUrl: "" // Leave empty if there is no live demo yet
  }
  ```

### 2. Adding a New Certificate
* **Where:** Google Drive (set sharing to **Anyone with the link -> Viewer**) + `<script>` -> `CERTIFICATES` array
* **Template:**
  ```javascript
  {
    issuer: "PLATFORM NAME",
    tag: "TOPIC",
    tagStyle: "emerald", // "cyan", "emerald", or "indigo"
    title: "Certificate Title",
    date: "Month Day, Year • Hours",
    description: "Short summary of skills covered.",
    credentialUrl: "[https://drive.google.com/file/d/YOUR_FILE_ID/view?usp=sharing](https://drive.google.com/file/d/YOUR_FILE_ID/view?usp=sharing)"
  }
  ```
* **Note:** Keep local PDFs inside the git-ignored `certificates/` folder so the repo stays lightweight.

### 3. Updating Education or Chapters
* **Where:** Inside `<section id="education">` in `index.html`
* **Steps:**
  * Edit card text directly inside the NIOS, Allen Online, or Cuemath cards.
  * Add or remove `<li>Chapter Name</li>` items inside `#panel-10`, `#panel-11`, or `#panel-12`.

### 4. Adding New Technical Skills
* **Where:** Inside `<section id="skills">` in `index.html`
* **Template:**
  ```html
  <span class="skill-pill">New Skill</span>
  ```
  *(Paste inside the `.tech-pills` / `.pill-list` container of the matching card.)*

### 5. Updating Hobbies or Contact Info
* **Hobbies (`<section id="hobbies">`):**
  ```html
  <div class="hobby-card">
    <div class="hobby-icon">🎯</div>
    <div class="hobby-title">New Hobby</div>
  </div>
  ```
* **Contact Info:** Update `vikram.rakr@gmail.com` inside `copyEmail()` in `<script>` and inside `<footer>`.