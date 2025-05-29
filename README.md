# 🖼️ feh — Lightweight CLI Image Viewer and Wallpaper Setter

**feh** is a minimalist command-line image viewer for X11. It is commonly used to quickly view images or set wallpapers without the overhead of a full graphical image viewer. Perfect for lightweight window managers like i3, bspwm, or Openbox.

---

## ✅ Features

* Fast and lightweight image viewer
* Supports viewing single images, directories, and slideshows
* Can set desktop wallpapers with multiple scaling options
* Minimal dependencies, no GUI menus or toolbars
* Supports thumbnail previews and montage creation
* Highly scriptable via CLI options

---

## 🔧 Installation

### Debian / Ubuntu

```bash
sudo apt install feh
```

### Arch Linux

```bash
sudo pacman -S feh
```

### Fedora

```bash
sudo dnf install feh
```

---

## 🚀 Basic Usage

```bash
feh /path/to/image.jpg
```

Open a single image in a window.

---

## ⚙️ Command-Line Options

| Option                        | Description                                  |   |
| ----------------------------- | -------------------------------------------- | - |
| `/path/to/images`             | Load one or multiple images                  |   |
| `--bg-scale <file>`           | Set wallpaper scaled to fit the screen       |   |
| `--bg-fill <file>`            | Set wallpaper scaled and cropped to fill     |   |
| `--bg-center <file>`          | Set wallpaper centered                       |   |
| `--slideshow-delay <seconds>` | Time delay between images in slideshow       |   |
| `-r` / `--recursive`          | Recursively search directories for images    |   |
| `-t` / `--thumb`              | Display thumbnail preview mode               |   |
| `-z` / `--randomize`          | Randomize image order                        |   |
| `--no-fehbg`                  | Do not write wallpaper setting to `~/.fehbg` |   |

---

## 🎯 Examples

### Open an image:

```bash
feh ~/Pictures/wallpaper.jpg
```

### Set a wallpaper scaled to screen size:

```bash
feh --bg-scale ~/Pictures/wallpaper.jpg
```

### Start a slideshow of all images in a directory with 5s delay:

```bash
feh --slideshow-delay 5 ~/Pictures/
```

### Set a wallpaper filling the screen (cropping if needed):

```bash
feh --bg-fill ~/Pictures/wallpaper.jpg
```

---

## 📂 Sample Output

When running `feh` on an image, a window opens with the image displayed. Keyboard shortcuts are used for navigation (e.g., arrow keys, space, q to quit).

---

## 📚 More Info

* Manual:

```bash
man feh
```

* Arch Wiki: [https://wiki.archlinux.org/title/Feh](https://wiki.archlinux.org/title/Feh)

---

## 🧩 Alternatives

* `sxiv` — Simple X Image Viewer with minimal GUI
* `ristretto` — Lightweight GTK image viewer
* `pqiv` — Powerful CLI image viewer with zoom/pan features
