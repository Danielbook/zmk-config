# 🔥 ZMK Config for Corne v3 with E-Paper Display

An ergonomically optimized ZMK configuration for the Corne v3 keyboard (3x6+3) featuring e-paper display, RGB underglow, and workflow-tuned keymaps designed specifically for vim, tmux, and tiling window managers.

## ✨ Features

- **🏠 Home Row Modifiers** - Reduces pinky strain with balanced timing (280ms)
- **👍 Optimized Thumb Cluster** - Strategic placement for Space, Tab, and Delete
- **⚡ Smart Combos** - Quick access to Escape and Tab via key combinations
- **🎯 One-Shot Workspace Switching** - Dedicated Super+number macros for instant workspace access
- **📱 E-Paper Status Display** - Custom battery, connectivity, and layer indicators
- **🌈 RGB Underglow** - Full color and effect control
- **⌨️ Colemak-DH Primary** - Optimized for typing comfort
- **🔧 Workflow-Optimized** - Tailored for development with vim, tmux, and window management

## 🎯 Optimized For

This configuration is specifically tuned for development workflows including:

- **Vim/Neovim** - Escape on Caps Lock tap, N+E combo for quick Escape
- **tmux** - `Ctrl+Q` prefix with thumb Ctrl, `Ctrl+hjkl` navigation via home row
- **Hyprland/i3/Sway** - One-keypress workspace switching with Super+numbers
- **Terminal-heavy** development with multiple Ctrl access points
- **Coding** with optimized symbol and function key layers

## 📋 Layer Overview

### Layer 0: Colemak-DH (Base Layer)
```
┌─────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬─────┐
│ TAB │  Q  │  W  │  F  │  P  │  B  │   │  J  │  L  │  U  │  Y  │  ;  │CTRL/│
│     │     │     │     │     │     │   │     │     │     │     │     │BKSP │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL/│ A/  │ R/  │ S/  │ T/  │  G  │   │  M  │ N/  │ E/  │ I/  │ O/  │  '  │
│ ESC │GUI  │ALT  │CTRL │SHFT │     │   │     │SHFT │CTRL │ALT  │GUI  │     │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHFT/│  Z  │  X  │  C  │  D  │  V  │   │  K  │  H  │  ,  │  .  │  /  │GUI/ │
│CAPS │     │     │     │     │     │   │     │     │     │     │     │SPC  │
└─────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │GUI/ │ SYM │NUM/ │   │NAV/ │ DEL │ ALT │
                  │ TAB │  ↓  │SPC  │   │ENTR │     │     │
                  └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

**Key Improvements:**
- **Caps Lock**: Tap for Escape (vim!), Hold for Ctrl (terminal!)
- **Left Thumb**: Tap for Tab, Hold for Super/GUI (window mgmt)
- **Right Thumb**: Delete key for easy access
- **Bottom Right**: Tap for Space, Hold for Super (alternative Super access)

### Layer 1: Symbols & Media
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

**Features:**
- Symbols for coding on top row
- Media controls (prev/play/next, mute, volume) on home row left
- Paired brackets and operators easily accessible

### Layer 2: Navigation & Functions
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

**Features:**
- All 16 function keys (F1-F16) for development tools
- Arrow keys in vim-style HJKL positions
- Home/End/PgUp/PgDn for document navigation

### Layer 3: Numbers & Workspace Management
```
┌─────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬─────┐
│BTCLR│ BT1 │ BT2 │ BT3 │ BT4 │ BT5 │   │ ⊞+1 │ ⊞+2 │ ⊞+3 │ ⊞+4 │ ⊞+5 │PRSCR│
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │RGB  │RGB  │RGB  │RGB  │RGB  │   │ ⊞+6 │ ⊞+7 │ ⊞+8 │ ⊞+9 │ ⊞+0 │     │
│     │ ON  │EFF  │HUE+ │SAT+ │BRI+ │   │     │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │RGB  │RGB  │RGB  │RGB  │RGB  │   │  1  │  2  │  3  │  4  │  5  │     │
│     │OFF  │EFR  │HUE- │SAT- │BRI- │   │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │ ▼▼▼ │   │     │  6  │  0  │
                  └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

**Major Feature - One-Shot Workspace Switching:**
- **⊞+1 through ⊞+0** = Super+number macros for instant workspace switching
- Single keypress to switch workspaces (no holding multiple keys!)
- Regular numbers (1-6, 0) on bottom rows for typing
- Bluetooth profile switching (BT1-BT5)
- Full RGB underglow control

## 🏠 Home Row Modifiers

Ergonomic modifiers reduce finger travel and pinky strain:

**Left Hand (Colemak):**
- `A` → GUI/Super (hold)
- `R` → Alt (hold)
- `S` → Ctrl (hold)
- `T` → Shift (hold)

**Right Hand (Colemak):**
- `N` → Shift (hold)
- `E` → Ctrl (hold)
- `I` → Alt (hold)
- `O` → GUI/Super (hold)

**Timing:** 280ms tap-hold threshold with quick-tap enabled for balanced response.

## ⚡ Combos

Quick access key combinations that activate when pressed simultaneously:

| Keys | Result | Use Case |
|------|--------|----------|
| **N + E** | Escape | Vim muscle memory (like JK in insert mode) |
| **Q + W** | Tab | Quick tab without reaching |

**Combo Timing:** 50ms window for simultaneous key presses

## 🎯 Smart Key Positions

### Caps Lock → Escape/Ctrl
- **Tap**: Escape (essential for vim users!)
- **Hold**: Ctrl (for terminal commands)
- Eliminates pinky strain from corner Ctrl

### Left Inner Thumb → Tab/Super
- **Tap**: Tab (autocomplete, window switching)
- **Hold**: Super/GUI (window management commands)
- Most frequently used thumb position

### Right Inner Thumb → Delete
- Quick access to forward delete
- Replaces redundant layer toggle

### Bottom Right Corner → Space/Super
- **Tap**: Space (alternative access)
- **Hold**: Super/GUI (for one-handed window mgmt)

## ⚙️ Key Behaviors

- **Tap-Dance**: Shift/Caps on left pinky (tap twice for Caps Lock)
- **Hold-Tap**: Optimized 280ms timing for home row mods
- **Balanced Flavor**: Prevents accidental modifier activation during fast typing
- **Quick-Tap**: 175ms window for repeated taps without triggering hold
- **Combos**: 50ms simultaneous press window for combo triggers

## 🔧 Hardware

- **Board**: Corneish Zen v2 (left/right split)
- **Layout**: Corne v3 (3x6+3 keys)
- **Display**: E-paper with custom status widgets
- **RGB**: Full underglow with 16+ effects
- **MCU**: Nice Nano v2 compatible
- **Wireless**: Bluetooth 5.0 with 5 profile support
- **Battery**: Built-in rechargeable with e-paper battery indicator

## 📦 Installation

1. **Fork this repository**
2. **Enable GitHub Actions** in your fork's settings
3. **Push changes** to trigger automatic firmware build
4. **Download firmware** from the Actions tab (artifacts)
5. **Flash to keyboard**:
   - Put keyboard half into bootloader mode (double-tap reset)
   - USB drive appears named "NICENANO" or similar
   - Drag `corneish_zen_v2_left-zmk.uf2` to left half
   - Drag `corneish_zen_v2_right-zmk.uf2` to right half
   - Drive auto-ejects when complete
6. **Pair Bluetooth** (if wireless)
7. **Enjoy your optimized workflow!**

## 🎨 Customization

The layout is highly customizable. Edit `config/corneish_zen.keymap` to adjust:

### Common Tweaks
- **Tap-hold timings**: Change `tapping-term-ms` values in behaviors section
- **Combo timeout**: Adjust `timeout-ms` in combo definitions
- **Layer arrangements**: Reorder or modify layer bindings
- **RGB effects**: Configure colors, brightness, and patterns
- **Workspace macros**: Customize Super+number combinations

### Files to Modify
- `corneish_zen.keymap` - Main keymap and behavior definitions
- `corneish_zen.conf` - System settings (sleep timeout, RGB, etc.)
- `widgets/*.c` - Custom e-paper display widgets

## 💡 Usage Tips

### For Vim Users
- Use **Caps Lock (tap)** for Escape - no more pinky reach!
- **N+E combo** provides quick Escape from home row
- Ctrl on home row (S/E) makes `Ctrl+[` easy to reach
- Tab on thumb makes autocomplete (`Ctrl+N`/`Ctrl+P`) comfortable

### For Tmux Users
- **Caps Lock (hold)** gives Ctrl for `Ctrl+Q` prefix
- Home row Ctrl (S/E) makes `Ctrl+hjkl` navigation natural
- Space on thumb keeps prefix combos comfortable

### For Window Management
- **Single-press workspace switching**: Just press Layer 3 + number
- No more awkward Super+Layer+number combinations!
- Tab on thumb (hold for Super) enables easy `Super+Tab` window switching

## 🙏 Credits

- Built with [ZMK Firmware](https://zmk.dev/)
- Inspired by the [Corne](https://github.com/foostan/crkbd) keyboard
- Home row mod timings from [Miryoku](https://github.com/manna-harbour/miryoku)
- Corneish Zen hardware by [Darryl deHaan](https://lowprokb.ca/)

## 📝 License

MIT License - See LICENSE file for details