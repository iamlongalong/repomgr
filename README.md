## repomgr - Simplify Your Linux Repository Management

Welcome to repomgr, your trusty sidekick for managing Linux software sources with ease. Breeze through repository switches and ensure your system's software sources are always up-to-date with your preferred mirrors. Wave goodbye to manual editing and let repomgr automate the process with a sprinkle of shell script magic!

## 👨‍💻 Usage

![usage](./assets/usage.mov)

you can get this script this way 👇:
```bash
curl -o repomgr https://raw.githubusercontent.com/iamlongalong/repomgr/main/repomgr && chmod +x repomgr && mv repomgr /usr/local/bin/ && repomgr -h
```

如果访问 github 不方便，可以用这个 👇🏻:
```bash
curl -o repomgr https://static.longalong.cn/scripts/repomgr && chmod +x repomgr && mv repomgr /usr/local/bin/ && repomgr -h
```

## 🚀 Features

Support for Major Distributions: Whether you're a fan of Ubuntu, Debian, CentOS, or Alpine, repomgr has got your back.
Multiple Mirror Sources: Choose from Tsinghua University TUNA, Alibaba, USTC, or stick with the original official mirrors.
Easy Resets: Made a mistake? Fret not! Reset your software sources to the last backed-up version in a snap.
Simplified Switching: Just a command away from switching to your desired mirror.
Verbose Logging: Every action is logged for your perusal and troubleshooting convenience.

## 💻 How It Works

repomgr is intuitive and user-friendly. It detects your Linux distribution, supports various mirrors, and facilitates smooth transitions between them. Here's a breakdown:
Detect Your Flavor: Automatically figures out your operating system and its version.
Backup Repos: Clone your current repo list for a rainy day.
Switching Repos: Change your repos to your chosen mirror with a simple command.
Restoring Peace: Rolled a critical fail? Restore your original repos from backup.

## 📖 Usage Instructions

To use repomgr, simply invoke it with your choice of action. Here's the syntax to sail through your repository management:
```bash
repomgr [OPTION]... [MIRROR_SOURCE]
```

Let's look at the available options:

### 🔄 Switching Mirrors

To switch to a new software source, use the use command followed by your desired mirror's identifier:

```bash
repomgr use THU   # Pings over to the Tsinghua University TUNA mirror
repomgr use ALI   # Swaps to the Alibaba mirror
repomgr use USTC  # Shifts to the USTC mirror
repomgr use ORI   # Returns to the Original official mirror
```

### 🔙 Reset to Backup

If you need to revert to your previous settings, repomgr makes it a cakewalk:
```bash
repomgr reset
```

### ℹ️ Repository Information

Curious about your current repo statuses? Peek at them with:
```bash
repomgr info
```

## 🎉 Conclusion
With repomgr, you're the repository wizard, transforming and tailoring your Linux software sources with minimal fuss. Now go ahead and push it to GitHub, let the world embrace the simplicity of repository management!
Heads Up: You're currently reading the README.md, the prelude to your repository adventure. Got questions or feedback? Raise an issue on GitHub. Happy managing! 🌟