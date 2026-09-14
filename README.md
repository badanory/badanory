<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=220&section=header&text=Yoonseok%20Son&fontSize=64&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=Robotics%20%C2%B7%20Embodied%20AI%20%C2%B7%20Real-time%20Control&descSize=20&descAlignY=60" alt="header" />
</div>

<p align="center">
  Robotics engineer building <b>embodied AI</b>: LLM-driven robot behavior, real-time motor control, and simulation-in-the-loop.<br/>
  Currently working on <b>Phil</b>, an AI drummer robot, at KIST.
</p>

<div align="center">
  <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">🧑‍💻 Contact me 🧑‍💻</h2>
  <a href="https://velog.io/@badanory"><img src="https://img.shields.io/badge/Velog-20C997?style=for-the-badge&logo=velog&logoColor=white" alt="Velog" /></a>
  <a href="mailto:0314jacob@naver.com"><img src="https://img.shields.io/badge/Mail-03C75A?style=for-the-badge&logo=naver&logoColor=white" alt="Mail" /></a>
  <a href="https://github.com/badanory"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <br/><br/>
  <strong>📧 0314jacob@naver.com</strong>
</div>

<br/>

<div align="center">
  <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">✨ Tech Stack ✨</h2>

  <h4>Languages</h4>
  <img src="https://img.shields.io/badge/C++17-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" />

  <h4>Robotics &amp; Control</h4>
  <img src="https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/SocketCAN-333333?style=for-the-badge&logo=linux&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Dynamixel-2E7D32?style=for-the-badge" />&nbsp;
  <img src="https://img.shields.io/badge/PyBullet-2D3E50?style=for-the-badge" />&nbsp;
  <br/>
  <img src="https://img.shields.io/badge/NVIDIA%20Jetson-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Linux%20RT-FCC624?style=for-the-badge&logo=linux&logoColor=black" />

  <h4>AI / ML</h4>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Ollama%20%2F%20Qwen3-000000?style=for-the-badge&logo=ollama&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Whisper%20STT-412991?style=for-the-badge&logo=openai&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />&nbsp;
  <br/>
  <img src="https://img.shields.io/badge/YOLO-111F68?style=for-the-badge" />&nbsp;
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=for-the-badge&logo=openai&logoColor=white" />

  <h4>Backend &amp; Tools</h4>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />&nbsp;
  <img src="https://img.shields.io/badge/VS%20Code-2C2C32?style=for-the-badge&logo=visualstudiocode&logoColor=22ABF3" />
</div>

<br/>

<div align="center">
  <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">🥁 Phil, the AI Drummer 🥁</h2>
</div>

<p align="center">
  Phil listens, talks back, and plays a real drum kit.<br/>
  A local LLM plans the performance, a C++ controller drives the motors over CAN in real time,<br/>
  and a frame-level SIL runs the <i>same</i> controller against PyBullet with zero code changes.
</p>

```text
voice ─▶ Whisper ─▶ Qwen3 planner ─▶ TCP ─▶ C++ controller ─▶ CAN / serial ─▶ motors
                                                          └──▶ vcan / PTY ─▶ PyBullet (SIL)
```

| Repo | Role | Stack |
|:--|:--|:--|
| [**phil-control**](https://github.com/badanory/phil-control) | Real-time body controller: state machine, trajectory generation, TMotor / Maxon / Dynamixel drive | C++17, SocketCAN, Dynamixel SDK |
| [**phil-interaction**](https://github.com/badanory/phil-interaction) | Brain: Whisper STT → Qwen3 classifier / planner → validated commands → MeloTTS | Python, Ollama, LangGraph |
| [**phil-simulation**](https://github.com/badanory/phil-simulation) | Frame-level SIL: replays raw `can_frame` / Dynamixel packets into PyBullet | Python, PyBullet, vcan, PTY |
| [**phil-midi-converter**](https://github.com/badanory/phil-midi-converter) | MIDI ↔ score converter: Groove MIDI Dataset drum tracks → Phil's text scores (quantize, merge, assign hands) and back to MIDI | C++17 |
| [Phil_Robot-AI-Drummer](https://github.com/badanory/Phil_Robot-AI-Drummer) | Legacy monorepo snapshot before the split | archive |

<!-- TODO: 데모 GIF 또는 YouTube 링크. 예: <p align="center"><img src="docs/phil_demo.gif" width="600"/></p> -->

<br/>

<div align="center">
  <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">🛠 Other Projects 🛠</h2>
</div>

- **[Smart Duct Inspection Robot](https://github.com/badanory/Smart-Duct-Inspection-Robot)** · Award-winning capstone. ROS2, LiDAR 2D SLAM, frontier exploration, YOLO cable-damage detection, web monitoring. Owned SLAM, track-drive mechanics, and detector real-world robustness (>90% on-site accuracy).
- **[Amorepacific Short-form Ad Agent](https://github.com/badanory/Amore_project)** · Vision + LLM pipeline that turns a product page URL into a 15-second short-form ad. Playwright DOM asset extraction, GPT storyboard, MoviePy rendering, C# WinForms client over WebSocket.

<br/>

<div align="center">
  <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">📋 Stats 📋</h2>
  <img src="https://github-readme-stats.vercel.app/api?username=badanory&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" height="165" alt="stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=badanory&layout=compact&theme=tokyonight&hide_border=true&langs_count=6" height="165" alt="top langs" />
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer" alt="footer" />
</div>
