# Hi, I'm Stefan Balanica 👋
💻 Passionate About Frontend & Mobile | 🎨 UI/UX Learner | 🚀 Growing as a Software Developer 

### 📌 About Me
- 🔭 I'm currently a second-year student studying Computer Science at the Faculty of Mathematics and Computer Science.
- 🌱 Learning **Nextjs, TypeScript,Python, C#, Java**
- 🌍 Based in Brasov,Romania | Available for freelance & collaborations
- 📫 Reach me at **[stefanbalanica22@yahoo.com]**

### Connect with me:
[<img src="https://github.com/StefanBalanica/StefanBalanica/blob/main/linked-in-alt.svg" alt="LinkedIn" width="30" />](https://www.linkedin.com/in/ștefan-bălănică-4719a0289)

### 🔥 Most Used Languages
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=StefanBalanica&layout=compact&theme=radical&langs_count=10)

name: Update README

on:
  schedule:
    - cron: '0 0 * * *' # Runs at midnight every day

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v2

      - name: Update README
        run: |
          # Your script to update README goes here
          # For example, you can use a Python script to fetch and update stats
          python update_readme.py

      - name: Commit changes
        run: |
          git config --local user.email "your_email@example.com"
          git config --local user.name "Your Name"
          git add README.md
          git commit -m "Update README with latest stats"
          git push

