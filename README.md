# 🔥 ZMK Config for Corne v3 with E-Paper Display

An ergonomically optimized ZMK configuration for the Corne v3 keyboard (3x6+3) featuring e-paper display, RGB underglow, and workflow-tuned keymaps.

## ✨ Features

- **🏠 Home Row Modifiers** - Reduces pinky strain with balanced timing
- **👍 Optimized Thumb Cluster** - Strategic placement for common modifiers
- **📱 E-Paper Status Display** - Custom battery, connectivity, and layer indicators
- **🌈 RGB Underglow** - Full color and effect control
- **⌨️ Dual Layout Support** - Seamless Colemak-DH ↔ QWERTY switching
- **🔧 Workflow-Optimized** - Tailored for tmux, vim, and window management

## 🎯 Optimized For

This configuration is specifically tuned for development workflows including:

- **tmux** with `Ctrl+Q` prefix and `Ctrl+hjkl` navigation
- **Neovim** with Space leader key accessibility  
- **Hyprland/i3** window management (`Super+1-9` workspace switching)
- **Terminal-heavy** development with thumb-accessible Ctrl
- **Coding** with symbol layer and function key access

## 📋 Layer Overview

### Layer 0: Colemak-DH (Primary)
```
┌─────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬─────┐
│ TAB │  Q  │  W  │  F  │  P  │  B  │   │  J  │  L  │  U  │  Y  │  ;  │CTRL/│
│     │     │     │     │     │     │   │     │     │     │     │     │BKSP │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│GUI/ │ A/  │ R/  │ S/  │ T/  │  G  │   │  M  │ N/  │ E/  │ I/  │ O/  │  '  │
│SPC  │GUI  │ALT  │CTRL │SHFT │     │   │     │SHFT │CTRL │ALT  │GUI  │     │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHFT/│  Z  │  X  │  C  │  D  │  V  │   │  K  │  H  │  ,  │  .  │  /  │ ESC │
│CAPS │     │     │     │     │     │   │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ALT │ SYM │NUM/ │   │NAV/ │TOGG │ ALT │
                  │     │  ↓  │ENT  │   │SPC  │ ↓   │     │
                  └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Layer 1: QWERTY (Secondary)
Standard QWERTY with same modifiers and thumb cluster.

### Layer 2: Symbols & Media
```
┌─────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │  !  │  @  │  #  │  $  │  %  │   │  ^  │  &  │  *  │  (  │  )  │ DEL │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │PREV │PLAY │NEXT │MUTE │VOL+ │   │  -  │  =  │  '  │  [  │  ]  │  `  │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │VOL- │   │  _  │  +  │  ~  │  {  │  }  │  |  │
└─────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │ ▼▼▼ │     │   │ INS │ DEL │     │
                  └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Layer 3: Navigation & Functions
```
┌─────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │ F1  │ F2  │ F3  │ F4  │ F5  │   │ F6  │ F7  │  ↑  │ F8  │ F9  │ F10 │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ F11 │ F12 │ F13 │ F14 │ F15 │   │ F16 │  ←  │  ↓  │  →  │HOME │PGUP │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │     │   │     │     │     │     │ END │PGDN │
└─────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │   │ ▼▼▼ │     │     │
                  └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Layer 4: Numbers & System
```
┌─────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬─────┐
│BTCLR│ BT1 │ BT2 │ BT3 │ BT4 │ BT5 │   │  +  │  1  │  2  │  3  │  *  │ DEL │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │RGB  │RGB  │RGB  │RGB  │RGB  │   │  -  │  4  │  5  │  6  │  =  │PRNT │
│     │ ON  │EFF  │HUE+ │SAT+ │BRI+ │   │     │     │     │     │     │SCRN │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │RGB  │RGB  │RGB  │RGB  │RGB  │   │  _  │  7  │  8  │  9  │  /  │     │
│     │OFF  │EFR  │HUE- │SAT- │BRI- │   │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │   │  .  │  0  │ ▼▼▼ │
                  └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

## 🏠 Home Row Modifiers

Ergonomic modifiers reduce finger travel and pinky strain:

**Left Hand:**
- `A` → GUI/Super (hold)
- `R` → Alt (hold) 
- `S` → Ctrl (hold)
- `T` → Shift (hold)

**Right Hand:**
- `N` → Shift (hold)
- `E` → Ctrl (hold)
- `I` → Alt (hold)
- `O` → GUI/Super (hold)

## ⚙️ Key Behaviors

- **Tap-Dance**: Shift/Caps on left pinky
- **Layer Toggles**: Seamless layout switching
- **Hold-Tap**: Optimized timing for home row mods (280ms)
- **Balanced Flavor**: Prevents accidental modifier activation

## 🔧 Hardware

- **Board**: Corneish Zen v2 (left/right split)
- **Layout**: Corne v3 (3x6+3 keys)
- **Display**: E-paper with custom status widgets
- **RGB**: Full underglow with 16+ effects
- **MCU**: Nice Nano v2 compatible

## 📦 Installation

1. Fork this repository
2. Enable GitHub Actions for automated builds
3. Download firmware from Actions tab
4. Flash `.uf2` files to your keyboard halves
5. Enjoy your optimized layout!

## 🎨 Customization

The layout includes custom status display widgets and extensive RGB configuration. Modify `corneish_zen.keymap` to adjust:

- Key positions and behaviors
- Layer arrangements  
- Tap-hold timings
- RGB effects and colors

## 🙏 Credits

- Built with [ZMK Firmware](https://zmk.dev/)
- Inspired by the [Corne](https://github.com/foostan/crkbd) keyboard
- Home row mod timings from [Miryoku](https://github.com/manna-harbour/miryoku)