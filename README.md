## Hi, I'm Dylan 👋

<!--
**dstier-git/dstier-git** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

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
Computer Science and Data Science @ UC Berkeley  
Building at the intersection of machine learning, full-stack systems, and music technology.

---

## Currently building


**Texture**

We're building Texture, an active AI music production collaborator. You direct, it executes. Challenging Suno's push to brand AI as a way to skip the little bits of music. We think AI can be the ramp that keeps people making music and helps beginners pick it up, launching songs while keeping the power to edit and shape in your hands. Join early access crew [on our landing page](https://www.textureai.app/) for launch announcements!

**Fraud Code**

Finally, a [coding agent harness that _maximizes hallucination._](https://github.com/dstier-git/fraud-code) Satire, early stage.

## Some other projects

**Music Clipboard (AI + DAWs)**  
A [cross-platform music workflow tool](https://github.com/dstier-git/Music-Clipboard) using file extraction and MCPs to enable **AI-assisted editing** *across* standard music production softwares. Provides an easy and simple way to move music information from one DAW to another.

**JamGuide**  
A live jam-session discovery platform helping musicians organize sessions, network, and manage bookings in real time.  
Visit now at [jamguide.org](https://jamguide.org) 

---


## Interests

- Machine Learning (modeling, inference, applied systems)
- Backend architecture
- AI tool integration & agent workflows
- Music technology

---

## Tech Stack

- **Languages:** Python, Java, SQL, Javascript/TS
- **ML:** PyTorch, scikit-learn  
- **Code frameworks:** FastAPI, Node.js, React, Next.js
- **Data Science:** PostgreSQL, Pandas, NumPy, Matplotlib, Seaborn, Requests

---

## Outside of Code

- Trumpet player (11+ years) 
- Music production, jazz, arranging 🎶
- Rocket League ⚽🚗


---
<details>
<summary><h2>Some useful open-source tools I've been using (on macOS)</h2></summary>

- **iTerm**, a terminal alternative that easily supports tmux, cursor movement by mouse, easy-copy pasting, amazing customization. [Download](https://iterm2.com/index.html) and [lots of cool color schemes](https://iterm2colorschemes.com/) (I use Monokai Pro Spectrum)
- **Glow**, a very simple renderer for markdown files inside the terminal. [Repo](https://github.com/charmbracelet/glow)
- **Orca**, an agentic IDE that lets you group agent CLI sessions into tasks and projects for quick management. Includes smooth multi-pane terminal, a gorgeous UI, and very active maintainment.


And for coding agents specifically...
- **CodexBar**, amazingly convenient list for your current usage on every major agent provider (macOS). Simple dropdown list from the menu bar. [Repo](https://github.com/steipete/CodexBar) <details><summary>Click here to see preview pic</summary><img width="154" height="411" alt="image" src="https://github.com/user-attachments/assets/56236539-0671-424a-aa4a-6f1805f81d8b" /></details>
- **Plannotator**, a plugin that uses hooks to automatically open your browser and load clean renders of proposed agent plans. Enables both a smooth visual experience for reading the plans and the ability to annotate plans and send back more specific feedback than the general options most providers give. [Link to install](https://plannotator.ai/)
- **code-review-graph** is a set of skills for creating and maintaining graphs of your codebase. Lowers token usage, increases response speed, identifies gaps. [Repo](https://github.com/tirth8205/code-review-graph). A quick note, I've found this integration to be smoother and much simpler than the also-prominent [Graphify package](https://github.com/safishamsi/graphify), but to each their own.
- **CC Statusline Upgrade**, an improvement for the /statusline command on Claude Code. I found this to be the most useful setup for displaying model, effort level, token usage, etc. Find it under the umbrella of plugins [here](https://github.com/setouchi-h/cc-marketplace).<details><summary>Click here to see preview pic</summary><<img width="1356" height="102" alt="image" src="https://github.com/user-attachments/assets/a28719ae-14a9-4979-8567-fa15f47fc2d5" /></details>
- **oh-my-codex**, a multi-agent workflow manager for Codex. Pretty cool and works well sometimes but riddled with bugs and inefficiencies. Still fun to try out and is better than native Codex for distributing work and actively monitoring subagents. [Repo](https://github.com/Yeachan-Heo/oh-my-codex)
- **gstack**, Garry Tan's enormous Claude Code skill stack. Still not sure on the full CEO/manager-style workflow stuff but the office-hours skill is very powerful and I need to start using it more. The most important skill from here is the Codex skill, which provides Claude with workflows to call the Codex CLI and go back and forth to improve its plans or prep for PRs. [Repo](https://github.com/garrytan/gstack)
</details>

---
<details>
<summary><h2>Some of my custom bash aliases</h2></summary>
  
```bash
# git stuff
alias gdn='git diff --name-only'
alias ga='git add'
# git add multiple files separated by line breaks (press enter after ga-mul, then paste all, and press enter again)
# useful for adding untracked files from git ls-files --others
ga-mul() {
  if [ -t 0 ]; then
    local files=("$@")
    local line
    while IFS= read -r line; do
      [[ -z "$line" ]] && break
      files+=("$line")
    done
    git add "${files[@]}"
  else
    xargs git add
  fi
}
# type a commit message after 'gc ' and it will wrap in quotes and send the commit
gc() {
  git commit -m "$*"
}

# local dev environment
alias ports='lsof -i -P | grep LISTEN'
alias activate='source venv/bin/activate'

# general
alias ..='cd ..'
alias ...='cd ../..'
alias ~='cd ~'
alias ls='ls -G' # adds color for directories
```
</details>

---

## Contribution-eating snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dstier-git/dstier-git/output/github-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/dstier-git/dstier-git/output/github-snake.svg">
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/dstier-git/dstier-git/output/github-snake.svg">
</picture>
