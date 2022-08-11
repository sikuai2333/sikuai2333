<!-- 动态打字效果 -->
<h1 align="center">
  <a href="https://bing.com/">
    <img src="https://readme-typing-svg.herokuapp.com/?lines=print(%22Hello%2C%20World!%22);这是一个小菜鸡的Github&center=true&size=27">
  </a>
</h1>
<!-- 动态打字效果结束 -->


  
![Christmas's GitHub stats](https://github-readme-stats.vercel.app/api?username=sikuai2333&show_icons=true&theme=tokyonight)


[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=sikuai2333)](https://github.com/sikuai2333/github-readme-stats)

# Visit https://github.com/lowlighter/metrics#-documentation for full reference
name: Metrics
on:
  # Schedule updates (each hour)
  schedule: [{cron: "0 * * * *"}]
  # Lines below let you run workflow manually and on each commit
  workflow_dispatch:
  push: {branches: ["master", "main"]}
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          # Your GitHub token
          # The following scopes are required:
          #  - public_access (default scope)
          #  - public_repo
          #  - repo
          # The following additional scopes may be required:
          #  - read:org      (for organization related metrics)
          #  - read:user     (for user related data)
          #  - read:packages (for some packages related data)
          #  - repo          (optional, if you want to include private repositories)
          token: ${{ secrets.METRICS_TOKEN }}

          # Options
          user: sikuai2333
          template: classic
          base: header, activity, community, repositories, metadata
          config_timezone: Asia/Shanghai
          plugin_pagespeed: yes
          plugin_pagespeed_detailed: yes
          plugin_pagespeed_url: .user.website
          plugin_projects: yes
          plugin_projects_limit: 4
          plugin_stars: yes
          plugin_stars_limit: 4
          plugin_traffic: yes
          repositories_forks: yes

共有![Visitor Count](https://profile-counter.glitch.me/sikuai2333/count.svg)位伙伴来访

<!--
**sikuai2333/sikuai2333** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
