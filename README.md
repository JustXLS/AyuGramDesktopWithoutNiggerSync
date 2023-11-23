# AyuGram

![AyuGram Logo](.github/AyuGram.png)

## Features

- Full ghost mode (flexible)
- Messages history
- Anti-recall
- Font customization
- Streamer mode
- Material Design switches
- Local Telegram Premium
- Sync read states and message history with AyuSync *(TBA)*

<img src='.github/demos/demo1.png' width='250'> <img src='.github/demos/demo2.png' width='250'> <img src='.github/demos/demo3.png' width='250'>

## Downloads

### Windows

You can download prebuilt Windows binary from [Releases tab](https://github.com/AyuGram/AyuGramDesktop/releases) or from
the [Telegram topic](https://t.me/ayugramchat/12788).

Follow [official guide](https://github.com/AyuGram/AyuGramDesktop/blob/dev/docs/building-win-x64.md) if you want to
build by yourself.

### Any Linux

Depends ```"hunspell" "ffmpeg" "hicolor-icon-theme" "lz4" "minizip" "openal" "ttf-opensans"
    "qt6-imageformats" "qt6-svg" "qt6-wayland" "xxhash" "rnnoise" "pipewire" "libxtst"
    "libxrandr" "libxcomposite" "jemalloc" "abseil-cpp" "libdispatch" "openssl" "protobuf"
    "glib2" "libsigc++-3.0" "glibmm-2.68"```

Build Depends ```"cmake" "git" "ninja" "python" "range-v3" "tl-expected" "microsoft-gsl" "meson"
    "extra-cmake-modules" "wayland-protocols" "plasma-wayland-protocols" "libtg_owt"
    "gobject-introspection" "boost" "fmt" "mm-common" "perl-xml-parser" "libsigc++-3.0"```

Optional Depends ```"webkit2gtk: embedded browser features"
    "xdg-desktop-portal: desktop integration"```

Build
```
git clone https://github.com/JustXLS/AyuGramDesktopWithoutNiggerSync.git
```
```
CXXFLAGS+=' -ffat-lto-objects
```
```
cmake -B build -S AyuGramDesktop -G Ninja \
        -DCMAKE_VERBOSE_MAKEFILE=ON \
        -DCMAKE_INSTALL_PREFIX="/usr/local" \
        -DCMAKE_BUILD_TYPE=Release \
        -DTDESKTOP_API_ID=2040 \
        -DTDESKTOP_API_HASH=b18441a1ff607e10a989891a5462e627 \
        -DDESKTOP_APP_DISABLE_AUTOUPDATE=True
```
```        
cmake --build build
```
```
cmake --install build
```
### Remarks for Windows

Make sure you have these components installed with VS Build Tools:

- C++ MFC latest (x86 & x64)
- C++ ATL latest (x86 & x64)
- latest Windows 11 SDK

## Donation

If you enjoy using **AyuGram** and want to send us a tip, here's how you can do it:

- Using [Boosty](https://boosty.to/alexeyzavar) - any card and PayPal
- Using cryptocurrency - `TRpbajq38qU8joThgAfKJLyEPbNjzsdPJ1` (Tron + USDT)

## Credits

- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop)
- [Kotatogram](https://github.com/kotatogram/kotatogram-desktop)
- [64Gram](https://github.com/TDesktop-x64/tdesktop)
- [Forkgram](https://github.com/forkgram/tdesktop)
- [SQLite](https://github.com/sqlite/sqlite)
- [sqlite_orm](https://github.com/fnc12/sqlite_orm)

### Very special thanks to

- [Solar Icon Set](https://solariconset.com/)
- [JSON for Modern C++](https://github.com/nlohmann/json)
- [BitConverter](https://github.com/YanjieHe/BitConverter)
- [Not Enough Standards](https://github.com/Alairion/not-enough-standards)
