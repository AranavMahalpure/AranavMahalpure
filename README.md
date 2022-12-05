[![@aranavmahalpure's Holopin board](https://holopin.me/aranavmahalpure)](https://holopin.io/@aranavmahalpure)  
<!--**AranavMahalpure / AranavMahalpure** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.-->
## Hi there 👋, I'm AranavMahalpure 👩🏻‍💻
I'm a student, pursuing Bachelor of Technology in Computer Science and Engineering.
Student at International Institute of Information Technology, Pune.
- 🔭 I’m currently working on Web App Dev.
- 🌱 I’m currently learning Backend  Used for All domain.
- 🤔 I’m looking for help with Backend part for my projects.
- 💬 Ask me about Web Devlopment.
- 😄 Pronouns: He
- 📫 How to reach me: aranav1289@gmail.com
<h3 align="left">Tools and languages: </h3>

![My Skills](https://skillicons.dev/icons?i=html,css,js,php,c,cpp,py,)

### 📊 GitHub Stats
![](https://github-readme-stats.vercel.app/api/top-langs/?username=AranavMahalpure&theme=gotham&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

<div style="display: flex; flex-direction: row;">

<img width="46%" src="https://github-readme-stats.vercel.app/api?username=Aranavmahalpure&theme=gotham&hide_border=false&include_all_commits=false&count_private=false" />

<img width="46%" src="https://github-readme-streak-stats.herokuapp.com/?user=AranavMahalpure&theme=gotham&hide_border=false" />

</div>

# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

# Controls when the action will run. This action runs every 6 hours.

on:
  schedule:
      # every 6 hours
    - cron: "0 */6 * * *"

# This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:

    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

    # Generates the snake  
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: mishmanners
          # these next 2 lines generate the files on a branch called "output". This keeps the main branch from cluttering up.
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

     # show the status of the build. Makes it easier for debugging (if there's any issues).
      - run: git status

      # Push the changes
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
<p align="center"> 
  Visitor count<br>
  <img src="https://profile-counter.glitch.me/daweedkob/count.svg" />
</p>
