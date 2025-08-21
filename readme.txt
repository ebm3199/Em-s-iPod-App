# 🎵 Em's iPod App – iPod Classic support for Android Head Units

## 📌 Overview
The goal of **Em's iPod App** is to make old iPods (like the Classic 5th Gen) usable with modern Android devices and car head units.  
Instead of letting your iPod sit in a drawer, this project makes it possible to browse and play your iPod’s music library directly through an Android app.  

- ✅ Keep the **stock iPod OS** (no Rockbox required).  
- ✅ Support **Android phones & car head units**.  
- ✅ Browse by **Artist, Album, Song** using the iTunesDB library.  
- ✅ Support for **Light & Dark mode**, scalable UI across different screen sizes.  

Long-term, the project may also implement **iPod remote control (iAP protocol)** so the iPod itself handles playback.  

---

## 🔧 Current Status
🚧 Early development — currently experimenting with:  
- Detecting an iPod over Android’s **USB Host API**.  
- Reading the iPod’s file system in **Disk Mode**.  
- Parsing the **iTunesDB** (using open-source libraries like `libgpod`).  

---

## 🛠 Tech Stack
- **Language**: Kotlin  
- **UI Framework**: Jetpack Compose (for adaptive, scalable UI with light/dark mode)  
- **USB Access**: Android USB Host API  
- **iTunesDB Parsing**: Based on [libgpod](https://github.com/libgpod/libgpod) and/or Rockbox utilities  
- **Media Playback**: Android MediaPlayer API  

---

## 📍 Roadmap
### Phase 0 – Groundwork
- [ ] Set up Android Studio project  
- [ ] USB detection: identify when an iPod is connected  

### Phase 1 – File Access
- [ ] Mount iPod in Disk Mode via Android  
- [ ] List raw files from `/iPod_Control/Music`  

### Phase 2 – iTunesDB Parsing
- [ ] Parse iTunesDB for metadata (title, artist, album)  
- [ ] Display tracks in a simple list  

### Phase 3 – Playback
- [ ] Play audio directly from iPod storage via Android MediaPlayer  
- [ ] Basic play/pause/next controls  

### Phase 4 – UI Improvements
- [ ] Light/Dark mode support  
- [ ] Adaptive layouts for phones & head units  
- [ ] Album art extraction & display  

### Phase 5 – Stretch Goal
- [ ] Implement **iAP (iPod Accessory Protocol)** for remote control playback  

---

## 🤝 Contributing
We welcome contributors!  
If you’re interested in Android dev, reverse engineering, or just love old iPods, feel free to fork the repo and open a pull request.  

- Discussions → GitHub Issues or Discussions tab  
- Code style → Kotlin w/ Jetpack Compose  
- License → GPLv3 (due to `libgpod` dependencies)  

---

## 📚 Resources
- [libgpod](https://github.com/libgpod/libgpod) – Library for accessing iPod content & iTunesDB  
- [Rockbox](https://www.rockbox.org/wiki/Main_Page) – Open source iPod firmware (great docs on iPod internals)  
- [Android USB Host](https://developer.android.com/guide/topics/connectivity/usb/host) – Official Android docs  
- [gtkpod](http://www.gtkpod.org/) – Old Linux iPod manager  

---

## ⚡ Vision
Old iPods are still some of the best music players ever made. This project is about keeping them alive and making them usable in the modern Android ecosystem — especially in cars with Android-based head units.  

