<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=EB+Garamond&weight=800&size=28&duration=4000&pause=1000&random=false&width=435&lines=+𝗪𝗔𝗧𝗦𝗢𝗡_BUG+©𝐏𝐎𝐖𝐄𝐑𝐄𝐃+𝐁𝐘+𝐖𝐀𝐓𝐒𝐎𝐍+𝐗𝐃+alt="Typing SVG" />
  </a>
</p>

![WATSON-XD](https://files.catbox.moe/rfowi7.jpg)
<p align="center">
<a href="https://www.youtube.com/@WATSON_TECH"><img src="https://img.shields.io/badge/YouTube-ff0000?style=for-the-badge&logo=youtube&logoColor=ff000000&link=https://youtube.com/@DRK-TECH" /><br>
<a href="https://whatsapp.com/channel/0029VajjzuB9sBI890YffB1b"><img src="https://img.shields.io/badge/WhatsApp Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white&link=https://whatsapp.com/channel/0029VajjzuB9sBI890YffB1b" /><br>
<a href="https://t.me/+13472314632"><img src="https://img.shields.io/badge/Telegram-00FFFF?style=for-the-badge&logo=telegram&logoColor=white" />
---

## DEVELOPED BY 𝐏𝐎𝐖𝐄𝐑𝐄𝐃 𝐁𝐘 𝐖𝐀𝐓𝐒𝐎𝐍 𝐗𝐃

---

## CREATE YOUR FORK
<a href="https://github.com/Watson1xd/WATSON-XD-BUG/fork">
  <img title="WATSON-XD-BUG" src="https://img.shields.io/badge/FORK-WATSON-XD-BUG-red?color=red&style=for-the-badge&logo=stackshare">
</a>

---

### 🔐 Generate Pair Code For Session

#### PAIRING SERVER 
<a href="https://watson-xd-bug-1.onrender.com" target="_blank">
  <img alt="Pairing Code Server " src="https://img.shields.io/badge/PAIRING CODE-green?style=for-the-badge&logo=opencv&logoColor=white"/>
</a>

---

###  🚀DEPLOYMENTS🚀

<div align="center">
  <!-- Badges for deployment -->
  <a href="https://youtu.be/AZg7UMMy6q8?si=_YyYGgUS1AL9oR-B" target="_blank">
    <img src="https://img.shields.io/badge/Deployment-GitHub-blue?style=for-the-badge&logo=github" alt="GitHub Deployment" />
  </a>
  <a href="https://youtu.be/4b1HNuaQx54?si=CSRoq27E8nS0AeNA" target="_blank">
    <img src="https://img.shields.io/badge/Deployment-Codespace-blue?style=for-the-badge&logo=github" alt="Codespace Deployment" />
  </a>
  <a href="https://youtu.be/yH2KCK0AD4I?si=F5tjgBpK4ZQO0F-x" target="_blank">
    <img src="https://img.shields.io/badge/Deployment-Replit-blue?style=for-the-badge&logo=replit" alt="Replit Deployment" />
  </a>
  
---

## ⚠️ WARNING ⚠️

I am not responsible for any damage caused by this bot. Use this bot at your own risk. It is developed for educational purposes only. Any malicious use is strictly discouraged.

---

<details>
  <summary><strong>Show more</strong></summary>


---

## Developer 💀

<a href="https://github.com/watsonxdboy">
  <img src="https://github.com/WATSON-XD2.png" width="200" height="200" alt="WATSON-XD2"/>
</a>
<p align="center"><strong>WATSON-XD2</strong></p>

---

## Contributors 🤝

<a href="https://github.com/toge012345">
  <img src="https://files.catbox.moe/rfowi7.jpg" width="200" height="200" alt="toge012345"/>
</a>
<p align="center"><strong>watsonxdboy</strong

---

## GitHub Deployment

```yaml
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  schedule:
    - cron: '0 */6 * * *'  

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Install FFmpeg
      run: sudo apt-get install -y ffmpeg

    - name: Start application with timeout
      run: |
        timeout 21590s npm start  # Limits run to 5h 59m 50s

    - name: Save state (Optional)
      run: |
        ./save_state.sh
