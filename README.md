<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3500&pause=1200&color=7DD3FC&center=true&vCenter=true&width=760&lines=Rust+for+machines+that+move;Local+first.+Small+attack+surface.;Tested+before+I+call+it+done.;Teaching+robots+to+think+but+not+overthink.">
    <img alt="Rust for machines that move. Local first. Small attack surface. Tested before I call it done. Teaching robots to think but not overthink." src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3500&pause=1200&color=0B5394&center=true&vCenter=true&width=760&lines=Rust+for+machines+that+move;Local+first.+Small+attack+surface.;Tested+before+I+call+it+done.;Teaching+robots+to+think+but+not+overthink.">
  </picture>
</p>

## Manifesto

I don't trust code I can't read, machines I can't see, or dependencies nobody chose on purpose.

I build small and own the stack wherever I can. I've written drone flight software in Rust, a Rust web app with its own login and email verification, and a home server that runs its own language model, image models and network defence on a pair of GPUs from 2016. I'd rather understand every layer than trust the one on top.

### Engineering doctrine

Non-negotiable. Open a pull request if you want to argue.

1. **Small attack surface.** Reuse what's already installed. New software comes from a well-maintained official source, gets pinned to a version, and has to earn its place.
2. **Working beats claimed.** I run it before I say it works. If I haven't tested it, I say so.
3. **Numbers over adjectives.** If I say something got faster, the benchmark is in the repo and you can run it yourself.
4. **Delete what you replace.** Git keeps the history, so the working tree doesn't need old versions and scratch files lying around.
5. **Own the stack when it's practical.** I run models, image generation and inference on my own hardware whenever I can. Cloud is for when the job needs it, with the cost and failure modes in view.
6. **Delegate the typing, keep the judgment.** I brief coding agents clearly, check what they hand back, and own the result.

### What's on the bench

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/bench-dark.svg">
    <img alt="Graph of my home server, AI-Bot. Home Hub, one Python server, runs Transcribe, Transmute, Lead Radar, 3D Modeller, AI Gallery, Loom, Pi Fleet and Control Room. Hermes Agent calls the hub's app APIs and builds Transmute and Lead Radar nightly; hermes-vcc-engine is its context engine. The llama.cpp router serves Hermes and its gateway and runs on two Pascal GPUs, which ComfyUI shares after unloading the LLM. AI Gallery scores ComfyUI's images. Loom reads the Pi-hole's DNS log and names devices through it, and Pi Fleet drives it through its API. The gateway and Control Room's uptime alerts go to Discord, which is also home to my game's community. Also on the bench: airborne-oxide, OxidizedOasis, Attendex, a 4v4 tactics game and a Rust VPN." src="assets/bench-light.svg" width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/danbiocchi/hermes-vcc-engine"><img alt="hermes-vcc-engine" src="https://img.shields.io/badge/hermes--vcc--engine-context_compaction-6E56CF?style=for-the-badge"></a>
  <a href="https://github.com/danbiocchi/airborne-oxide"><img alt="airborne-oxide" src="https://img.shields.io/badge/airborne--oxide-drone_flight_software-000000?style=for-the-badge&logo=rust&logoColor=white"></a>
  <a href="https://github.com/danbiocchi/oxidizedoasis-websands"><img alt="OxidizedOasis" src="https://img.shields.io/badge/OxidizedOasis-Rust_web_app-B7410E?style=for-the-badge&logo=rust&logoColor=white"></a>
  <a href="https://github.com/danbiocchi/Attendex"><img alt="Attendex" src="https://img.shields.io/badge/Attendex-live_demo-3178C6?style=for-the-badge&logo=typescript&logoColor=white"></a>
</p>

### Worth a closer look

- **[hermes-vcc-engine](https://github.com/danbiocchi/hermes-vcc-engine).** When a Hermes Agent conversation fills its context window, the stock compactor asks the model to summarize it, which takes about 8 minutes on a local model. My engine does it in 0.05 seconds with no model call, and the agent remembers more afterwards: it gets 91% of follow-up questions right, against 76% after the stock compactor and 87% with the untouched transcript. It's listed in the official Hermes plugin catalog and has 30 stars.
- **[airborne-oxide](https://github.com/danbiocchi/airborne-oxide).** Flight software for drones, in Rust. A deterministic simulator runs much faster than real time, and a hard real-time flight core for STM32 already flies a simulated quad through lost radio, lost GPS, a dead IMU and a lost motor. Any logged flight replays through the core bit for bit.
- **A 4v4 tactics game** where all eight players plan in the same 20 seconds, then the turn plays out in four fixed phases. TypeScript, Three.js and Node, 650+ commits so far, with a Discord community I run. The repo stays private until it's ready to play.
- **Loom**, network defence for my house. Every connection is drawn as a thread from its place on Earth, through the network that owns it, to the device it reached. It reads the Pi-hole's DNS log and the firewall log, and it never draws a number it didn't measure.
- **Lead Radar** pulls about 92,000 building permits and business licences from a municipal open data API and posts a digest to Discord.
- **[Attendex](https://danbiocchi.github.io/Attendex/)**, a clickable prototype for a school board rule that teachers take attendance at every transition in the day. If a student goes missing, the principal's screen raises the alert straight away. The live demo works best with two tabs open side by side.

### Right now

I'm working on the Hermes context engine and the game. I'd like to collaborate on Rust for uncrewed systems. Ask me about Rust on drones and web servers, Hermes Agent, running models on hardware you own, or keeping a game's Discord alive. The easiest way to reach me is an issue on any repo linked here.

### Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![llama.cpp](https://img.shields.io/badge/llama.cpp-111111?style=for-the-badge)
![Hermes Agent](https://img.shields.io/badge/Hermes_Agent-6E56CF?style=for-the-badge)

Pinned repos are right below.

<!-- Contact links go here when you want them public. -->
