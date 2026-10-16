# WinRunner

A taskbar and app menu for Windows 11 with a Cinnamon (Linux) feel: your open apps, pinned apps, tray icons, volume and clock on one bar, plus a menu with search, categories, favorites and power buttons. It can sit next to the Windows taskbar or take its place.

> This application is built by AI. I made this for myself and I'm uploading it to GitHub for backup and to share in case anyone can get any use out of it. It's pretty specific to my setup and my needs, but if you can get any use out of it, then enjoy.
>
> Use at your own risk. I offer no warranty or guarantees for this software.

## Download

**Latest version: v1.4** (Oct 16, 2026)

- [WinRunner_v1.4_no-install.zip](https://github.com/codenomics/WinRunner/releases/download/v1.4/WinRunner_v1.4_no-install.zip) - 119 KB
- [WinRunner_v1.4_Setup.exe](https://github.com/codenomics/WinRunner/releases/download/v1.4/WinRunner_v1.4_Setup.exe) - 155 KB
- [WinRunner_v1.4_source.zip](https://github.com/codenomics/WinRunner/releases/download/v1.4/WinRunner_v1.4_source.zip) - 108 KB

What's new in v1.4:

- New snap layouts: pick a layout (halves, thirds, quarters ...) and a spot, then fill the other spots with your open windows
- Opens from a button on the bar or with Win+Z (each can be turned off in Settings > Widgets); optional: drag a window to the top edge of a screen (off by default)
- Adjustable space around snapped windows; the last layout you used is highlighted
- Resize snapped windows together: drag the edge two windows share and the other one follows (can be turned off in Settings > Widgets)
- Draw your own snap layouts (Settings > Widgets > Snap layouts > New layout): split the screen, drag the lines, name it; it shows up in the picker with the built-in ones

Older versions are on the [Releases page](https://github.com/codenomics/WinRunner/releases).

## Getting started

### Installer (recommended)

1. Download the file ending in `_Setup.exe` above.
2. Double-click it and click Install. It installs just for you - no admin password needed - and adds Start menu and Desktop shortcuts.
3. To remove it later: Windows Settings > Apps, find WinRunner and click Uninstall.

### No install (portable zip)

1. Download the file ending in `_no-install.zip` above.
2. Right-click it > Extract All, and pick a folder. Don't run it from inside the zip.
3. Open the folder and double-click the app's .exe. Nothing is installed; delete the folder to remove it.

Windows says "Windows protected your PC"? Click More info > Run anyway. It shows that for apps without a paid signing certificate.

## Source code

Want to see how it works, or build it yourself? Download the file ending in `_source.zip` above, extract it and double-click `Build.bat`. It only uses the C# compiler that already comes with Windows, so there is nothing to install.

## More details

```
GETTING STARTED
---------------
Pick one. Both give you the same app.

OPTION 1 - INSTALLER (recommended)
  Download the file ending in _Setup.exe, double-click it and click Install.
  It installs just for you (no admin password) and adds Start menu and
  Desktop shortcuts. Needs Windows 11 (64-bit).
  To remove it later: first close WinRunner (right-click its bar -> Exit
  WinRunner), then Windows Settings > Apps > WinRunner > Uninstall.

OPTION 2 - NO INSTALL (zip)
  1. Download the file ending in _no-install.zip. Right-click it -> Extract
  All... and put the WinRunner folder somewhere it can stay (for example
  Documents). Don't run it from inside the zip.
  2. Double-click WinRunner.exe. Nothing is installed; to remove it, close
  WinRunner (right-click its bar -> Exit WinRunner) and delete the folder.

EITHER WAY
  WinRunner starts as a bar above the normal Windows taskbar, so nothing
  is taken away until you choose. To let it take over, right-click the
  bar -> Settings... -> Taskbar & tray -> tick "Hide the Windows taskbar".
  Press Ctrl+Alt+Shift+T at any time to bring the Windows taskbar back.

"Windows protected your PC"? Click "More info" -> "Run anyway".
Windows shows that for apps downloaded from the internet that aren't
signed with a paid certificate.


USING IT
--------
The bar sits along the bottom of your main monitor (or the monitors you
pick in Settings), just above the Windows taskbar. Maximized windows stop
at the top of it. In Settings you can let it take over: the Windows
taskbar is hidden and WinRunner's bar sits at the very bottom (or top).

- Menu button (left end)
    Click it to open the app menu. It lists the same apps as "All apps"
    in the Windows Start menu, Microsoft Store apps included.
    - Search box (top): start typing to search ALL apps, then press
      Enter (or click an app) to open it. Esc clears the search, a
      second Esc closes the menu. Up/Down arrows move the highlight.
    - Categories (middle): All apps, Recently used, Runner Suite (apps
      whose name ends in "Runner"), Games,
      Internet, Media, Office, Development, System, Utilities, Other.
      Point at one for a moment (or click it) to switch. Left/Right
      arrows also switch when nothing is typed. Empty ones are hidden.
    - Apps (right): the apps in that category.
    - Favorites strip (far left): your favorite apps as icons.
    - Power buttons (bottom of the strip): Lock, Sign out, Sleep,
      Restart, Shut down. Sign out, Restart and Shut down ask first.
    - Right-click an app (in the list or the favorites strip):
      open it as administrator (not for Microsoft Store apps),
      add/remove favorites, pin/unpin it on the bar, or change its
      category. Categories are a best guess from the app's name; your
      changes are remembered ("Use the automatic category" undoes one).
    - Menu style (Settings -> Menu): Full, Favorites + apps (no
      categories), or Apps only (search, apps list and a row of power
      buttons along the bottom).
- Open apps (middle)
    One button per open window (or per app, see Settings).
    Click a button to bring that window to the front.
    Click the window that's already in front to minimize it.
    The cyan line under a button marks the window in front.
    When there are lots of windows, the buttons shrink to icons only.
    Grouped apps show how many windows they have on the icon; clicking
    one lists its windows so you can pick one.
    Right-click a button: open a new window, pin / unpin, move the
    window to another monitor, or close it.
    Pinned apps stay on the bar (left side) even when they're closed;
    click one to start it.
    Middle-click: opens a new window of the app (or closes the window,
    or nothing - see Settings).
    Drag a button left or right to change the order.
    A button that pulses pink means the app wants your attention.
    Hover preview (switch it on in Settings): rest the mouse on a button
    to see the window; click the picture to switch to it, x to close it.
- Tray icons and volume (left of the clock, main monitor's bar)
    While WinRunner has the Windows taskbar hidden, apps' tray icons
    (Discord, Steam ...) show here. Left-click, right-click and
    double-click work like on the Windows taskbar.
    The small arrow left of the tray icons folds the tray away (only the
    icons you picked as "always show" stay). Click it again to show all.
    Right-click the arrow to pick which icons are always shown.
    When you open the tray with the arrow, clicking anywhere else folds
    it away again (you can switch that off in Settings).
    The speaker is the Windows volume: click it for a slider, Mute, and
    the list of speakers/headsets and microphones (click one to switch
    to it), or roll the mouse wheel over it. Hover shows which device
    is in use.
    Clicking the network icon shows what you're connected with, plus
    links to Wi-Fi networks and the Windows network settings.
    The Windows Security (shield) icon opens Windows Security.
- Snap layouts (button just left of the Spotify player, or Win+Z)
    Opens a small picker of screen layouts (halves, thirds, quarters ...).
    Click a spot and the window you were just in snaps there; then click
    other open windows to fill the empty spots. Layouts stop at the bar.
    Optional (off by default, switch it on in Settings -> Widgets): drag a
    window to the top edge of a screen and the layouts appear there; move
    over a spot and let go. Windows already maximizes at the top edge and
    fills the halves at the left and right edges by itself.
    Settings -> Widgets has the space around windows, and switches for the
    button, Win+Z and the dragging.
    Draw your own layouts: Settings -> Widgets -> Snap layouts -> New
    layout. Click a spot, split it side by side or top / bottom, drag the
    lines to set the sizes, give it a name and Save. Your layouts show up in
    the picker after the built-in ones (Edit or Delete them in Settings).
    Windows that sit side by side (or stacked) resize together: drag the
    edge they share and the other window follows. Switch it off in
    Settings -> Widgets.
    Keep Windows' own "Snap windows" switch ON (Windows Settings -> System
    -> Multitasking); with it off, Windows won't let you drag a maximized
    window down by its title bar. Untick the options under it instead.
- Spotify player (Settings -> Widgets, on by default on the main bar)
    Shows the song and artist from the Spotify desktop app, with
    previous, play/pause and next buttons. It only reads and controls
    Spotify, nothing else that plays sound. Click the song name to bring
    Spotify forward (or start it). Each monitor has its own width.
    You can hide the buttons and show only the title: click = play/pause,
    double-click = next song, middle-click = open Spotify.
- Clock
    Click it for a calendar (arrows change the month).
- Show desktop (thin strip at the far right end)
    Click it to show the desktop; click again to bring the windows back.
- Windows key
    Opens the WinRunner menu instead of the Windows Start menu (you can
    turn this off in Settings). Windows key shortcuts like Win+E still
    work as usual.
- Right-click anywhere on the bar:
    Settings...                     see SETTINGS below
    Exit WinRunner                  closes the bar

SETTINGS
--------
Changes show on the bar right away and are remembered. Pick a category
on the left (Menu, Bars, Buttons, Widgets, Look, Theme, Taskbar & tray, About).
  Menu icon             Choose Menu Icon... picks your own picture for the
                        menu button (PNG, JPG or ICO). It can be:
                          - one picture, or
                          - a 3-part picture: three equal squares stacked
                            top to bottom = normal, mouse over, menu open.
                            The button fades between them.
                        WinRunner guesses which kind from the shape (three
                        times as tall as wide = 3-part); you can switch it.
                        "Trim empty space" cuts off see-through edges so the
                        icon fills the button. "Use the default icon" goes
                        back to the built-in one.
  Bars                  main monitor only, all monitors, or the ones you
                        tick; bottom or top of the screen (on a top bar
                        the menu and pop-ups open downward)
  Open apps on each bar all open apps, or only the apps on that monitor
  Buttons               one button per window, or one per app (grouped);
                        icon + title, icons only, or titles only
  Buttons               also: the widest a button with a title may get
  Widgets               the Snap layouts button and Win+Z; the Spotify player: off, main monitor's bar or every
                        bar, its width for each monitor, and the buttons on/off
  Look                  Solid, Clear (see-through), Blur, or Frosted glass,
                        and how strong the background color is (0% fully
                        see-through, 100% solid; each look remembers its
                        own, Frosted glass starts at 30%); normal or compact
                        (thinner) bar; the colored line along the top on/off.
                        The app menu uses the same look as the bar.
  Windows taskbar       hide the Windows taskbar (WinRunner takes over);
                        show tray icons on WinRunner's bar while it's hidden;
                        Windows key opens the WinRunner menu; start
                        WinRunner when Windows starts
  About                 the version, Check for updates, and a tick box to
                        check for updates when WinRunner starts
Plugging monitors in or out (or turning them off) updates the bars by
themselves after a second or two.

When a game or video goes full screen, the bar on that monitor stops
staying on top so it doesn't cover it.


THEMES (Settings -> Theme)
--------------------------
- Built in: WinRunner (neon), Dark and Light. Click one to use it.
- Your own: click "Make a copy to change" (or just change any color of
  a built-in theme - WinRunner makes your copy first), give it a name,
  then click a color square to pick a color, or type a code like
  #3D55E8 and press Enter. Every color can be changed: bar, menus,
  boxes, borders, text, accent, the highlight gradient, the top line
  gradient, mouse-over, selected, warnings and scrollbars.
- Themes are .theme files in %APPDATA%\WinRunner\themes. Export saves
  one anywhere to share it; Import adds one someone sent you.
- Tray icons are drawn by their own apps, so some may be hard to see
  on the Light theme.

IF THE WINDOWS TASKBAR IS HIDDEN
--------------------------------
- Its tray icons move to WinRunner's bar (you can switch that off in
  Settings). The Windows taskbar is kept up to date too, so if WinRunner
  closes, every icon is still there.
- Closing WinRunner (right-click the bar -> Exit WinRunner) brings the
  Windows taskbar back.
- If WinRunner crashes or is ended in Task Manager, a small helper brings
  the Windows taskbar back by itself.
- Press Ctrl+Alt+Shift+T at any time to bring the Windows taskbar back.
  This also switches hiding off in Settings.
- If WinRunner isn't running and the Windows taskbar still hides
  itself: open Windows Settings > Personalization > Taskbar > Taskbar
  behaviors and untick "Automatically hide the taskbar".


GOOD TO KNOW
------------
- Settings, themes and your menu button picture are kept in
  %APPDATA%\WinRunner.
- If something goes wrong, WinRunner-log.txt next to WinRunner.exe says
  what.
- Updates: a little while after WinRunner starts it checks GitHub for a
  newer version (it only reads the public release page; nothing is sent).
  If there is one, a small box by the clock asks whether to update. With
  the installer, Update now downloads the new installer and runs it; with
  the no-install zip, it opens the download page. Settings > About has
  Check for updates, and a tick box to turn the startup check off.
- To start WinRunner with Windows, tick that box in Settings.
- To remove WinRunner: close it first (right-click its bar -> Exit
  WinRunner, which gives the Windows taskbar back), then uninstall it or
  delete its folder, plus %APPDATA%\WinRunner.
```

