# Urchin Keyboard Layout

## Layer Overview
- **Layer 0**: BASE - Default typing layer with extensive Mod-Taps
- **Layer 1**: NUMPAD - Number pad and arithmetic
- **Layer 2**: NAV - Navigation arrows and Layer Toggles
- **Layer 3**: FUNCTION - F-keys and media controls
- **Layer 4**: SYMBOL - Special characters and symbols
- **Layer 5**: SETTINGS - Bluetooth and system settings
- **Layer 6**: INTELLIJ - IntelliJ IDEA shortcuts for Java development

---

## Layer 0: BASE
**Hold Behavior:** Almost every key acts as a modifier or shortcut when held.
- **Home Row Mods:** A/Gui, S/Alt, D/Ctrl, F/Shift (Mirrored on Right)
- **Top Row Mods:** Hold for Alt+Cmd+Key
- **Bottom Row Mods:** Hold for Cmd+Key (Cut/Copy/Paste etc.)

```
┌─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┐
│  Q  │  W  │  E  │  R  │  T  │       │  Y  │  U  │  I  │  O  │  P  │
│A+⌘+Q│A+⌘+W│A+⌘+E│A+⌘+R│A+⌘+T│       │A+⌘+Y│A+⌘+U│A+⌘+I│A+⌘+O│A+⌘+P│
├─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┤
│  A  │  S  │  D  │  F  │  G  │       │  H  │  J  │  K  │  L  │  ;  │
│ ⌘Mod│ ⌥Mod│ ^Mod│ ⇧Mod│^⌘T  │       │⇧⌘SPC│ ⇧Mod│ ^Mod│ ⌥Mod│ ⌘Mod│
├─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┤
│  Z  │  X  │  C  │  V  │  B  │       │  N  │  M  │  ,  │  .  │  /  │
│     │ ⌘X  │ ⌘C  │ ⌘V  │ ⌘B  │       │ ⇧⌘N │ Bksp│ ⇧ , │ ⇧ . │ ⇧ / │
└─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┘
            │Space│ Tab │Enter│       │Bksp │
            │ →L1 │ →L2 │ →L3 │       │ →L4 │
            └─────┴─────┴─────┘       └─────┘
```

## Layer 4: SYMBOL (Hold Backspace)
*Updated: Backtick (`\``) is now on Left Hand Index Inner position.*

```
┌─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┐
│  !  │  @  │  {  │  }  │  `  │       │  |  │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┤
│  ?  │  &  │  (  │  )  │  '  │       │     │  ⇧  │  ^  │  ⌥  │  ⌘  │
│     │ $/& │     │     │     │       │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┤
│  %  │  ^  │  _  │  -  │  "  │       │     │     │     │  ⌥  │     │
│     │     │ [ /_│ ] /-│ ~/" │       │     │     │     │     │     │
└─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┘
            │  =  │ N3  │     │       │     │
            │ \/= │     │     │       │     │
            └─────┴─────┴─────┘       └─────┘
```

## Layer 6: INTELLIJ (Toggle via NAV Layer)
*To Access: Hold Tab (L2) -> Tap T (Inner Top Left) to Toggle.*
*Updated for high-frequency Java tasks.*

```
┌─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┐
│Proj │Struc│ Run │Debug│Rcent│       │Back │Fwd  │Decl │ Gen │Intnt│
│ ⌘1  │ ⌘7  │ ^R  │ ^D  │ ⌘E  │       │ ⌘[  │ ⌘]  │ ⌘B  │ ⌘N  │ ⌥Ent│
├─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┤
│Undo │Redo │ Cmt │FindF│SrchA│       │Left │Down │ Up  │Right│Renam│
│ ⌘Z  │⇧⌘Z  │ ⌘/  │⇧⌘F  │⇧⇧   │       │     │     │     │     │ ⇧F6 │
├─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┤
│Copy │Paste│ Cut │Dupl │Find │       │Usage│FileS│Frmt │Close│Class│
│ ⌘C  │ ⌘V  │ ⌘X  │ ⌘D  │ ⌘F  │       │ ⌥F7 │ ⌘F12│⌥⌘L  │ ⌘W  │ ⌘O  │
└─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┘
            │     │     │     │       │     │
            └─────┴─────┴─────┘       └─────┘
```

*(Other layers 1, 2, 3, 5 omitted for brevity, see code for details)*

---

## Layout Critique & Kaizen

### 1. Mod-Tap Overload
**Observation:** You have mod-taps on almost every key (Row 1, 2, 3).
**Risk:** This creates high cognitive load and latency issues. With `tapping-term-ms = <300>`, you must hold a key for 0.3s to activate the mod. If you type fast, you're fine, but if you hesitate, you might accidentally trigger a modifier. Conversely, rolling keys (typing 'The') might trigger T+H modifier logic if not careful.
**Suggestion:** Consider reducing mod-taps to Home Row (Row 2) only. Shortcuts on Row 3 (Cut/Copy/Paste) are convenient but standard `Cmd+X/C/V` are already very ergonomic with home row mods.

### 2. Backtick Positioning
**Issue:** Originally on the far right top row (Symbol layer).
**Fix:** Moved to Left Hand Index Inner (`T` position on Base). This allows you to hold the layer key (Right Thumb) and press the key with your Left Index finger. Cross-hand combos are generally faster and more ergonomic than same-hand combos.

### 3. IntelliJ Layer Improvements
**Changes:**
- Added **Alt+Enter** (Intentions) - Crucial for Java.
- Added **Cmd+E** (Recent Files) - Faster navigation.
- Added **Cmd+O** (Go to Class) - Essential.
- Added **Cmd+Shift+F** (Find in Files).
- Added **Cmd+/** (Comment Line).
- Added **Cmd+Option+L** (Reformat Code).
- Organized Navigation (Arrows) to match Vim/HJKL positions on the right hand.
- Grouped Run/Debug/Project tools on the left top row.

### 4. Layer Access
**Observation:** Accessing IntelliJ layer is a Toggle (via Nav layer). This is good for "IntelliJ Mode", but remember to toggle back for typing code.
**Suggestion:** If you find yourself toggling too much, consider a "Momentary" layer access (Hold to activate) if you have a spare thumb key, but with 34 keys, toggling is a valid strategy for specific workflows.
