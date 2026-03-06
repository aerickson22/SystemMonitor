# SystemMonitor 📊

A terminal-based system monitor built in C using ncurses, inspired by tools like `btm` (Bottom) and `htop`.
This is a personal long-term learning project to explore C programming, Linux internals, and terminal UI design.

---

## 📁 Project Structure

```
SystemMonitor/
├── src/              # All .c source files
│   ├── main.c        # Entry point
│   ├── cpu.c         # CPU data from /proc/stat
│   ├── memory.c      # Memory data from /proc/meminfo
│   ├── network.c     # Network data from /proc/net/dev
│   └── process.c     # Process list from /proc/[pid]/stat
├── include/          # All .h header files
│   ├── cpu.h
│   ├── memory.h
│   ├── network.h
│   └── process.h
├── screenshots/      # Screenshots of the app as it progresses
├── Makefile          # Build instructions
├── .gitignore        # Ignore compiled files
└── README.md
```

---

## 🛠️ Build Instructions

> Requires GCC and ncurses on Linux or WSL (Windows Subsystem for Linux)

**Install dependencies:**
```bash
sudo apt update
sudo apt install gcc libncurses5-dev libncursesw5-dev -y
```

**Build the project:**
```bash
make
```

**Run it:**
```bash
./systemmonitor
```

---

## 🗺️ Pipeline / Roadmap

- [ ] **Stage 1** — Draw basic ncurses window layout
- [ ] **Stage 2** — Read and display CPU usage from `/proc/stat`
- [ ] **Stage 3** — Read and display Memory usage from `/proc/meminfo`
- [ ] **Stage 4** — Display live updating process list
- [ ] **Stage 5** — Add Network monitoring from `/proc/net/dev`
- [ ] **Stage 6** — Add ASCII/braille graphs for CPU and Memory
- [ ] **Stage 7** — Add colors and theming
- [ ] **Stage 8** — Add keyboard navigation and shortcuts
- [ ] **Stage 9** — Polish and final cleanup

---

## 📚 Learning Resources

### C Programming
- 📖 [Beej's Guide to C](https://beej.us/guide/bgc/) — Best free C book online
- 📖 [cppreference.com](https://en.cppreference.com/w/c) — Reference for any C function

### ncurses (Terminal UI)
- 📖 [TLDP ncurses Programming HOWTO](https://tldp.org/HOWTO/NCURSES-Programming-HOWTO/) — Classic beginner ncurses guide
- 📖 [ncurses Official Docs](https://invisible-island.net/ncurses/)

### Linux /proc Filesystem (System Stats)
- 📖 [Linux man page for /proc](https://man7.org/linux/man-pages/man5/proc.5.html) — Every /proc file explained

### Video Tutorials
- 🎥 Search **"ncurses tutorial C"** on YouTube
- 🎥 Search **"reading /proc/stat C tutorial"** on YouTube

### Inspiration / Source Code
- 💻 [htop on GitHub](https://github.com/htop-dev/htop) — Classic system monitor written in C
- 💻 [bottom on GitHub](https://github.com/ClementTsang/bottom) — The tool that inspired this project

---

## 📸 Screenshots

*Screenshots will be added as the project progresses.*

---

## 👤 Author

**aeric** — building this as a personal learning project.
