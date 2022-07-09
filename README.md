### Hi, I'm Mirian 👋
<div id='header' align='center'>
  <img src='https://media.giphy.com/media/idSEtVpsq0zpzKIhW1/giphy.gif' width='500'/>
  
<div id='header' align='center'>
  <img src='https://s4.aconvert.com/convert/p3r68-cdx67/atugy-e8sqi.png' width='900'/>
  
### About me: 
- ✨ I study at the National University of San Agustín
- 😄 You can contact me by: mosoriov@unsa.edu.pe

  
name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:  
jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}



<!--
**mirianosoriov/mirianosoriov** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
- ✨ I study at the National University of San Agustín
- 😄 You can contact me by: mosoriov@unsa.edu.pe
- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
