# stark-home-firefox

A minimal Firefox startpage with an arch linux terminal aesthetic. Single HTML file, zero dependencies, fully configurable via an inline config block.

<img width="1142" height="889" alt="start-home-page" src="https://github.com/user-attachments/assets/1e5570f0-aefb-4d57-b860-2b1eba89a9bc" />

---

## install

Save `homepage.html` anywhere on your disk, then point Firefox at it:

1. Open `about:preferences#home` in the address bar
2. Under **New Windows and Tabs** → **Homepage and new windows**, select **Custom URLs**
3. Paste the file path, e.g. `file:///home/bolan/.config/stark-home/homepage.html`

Done.

## configuration

All customization lives in the `CONFIG` block at the top of the `<script>` tag — no build step, no separate config file.

```js
const CONFIG = {
  user:   "bolan",        // username shown in prompt + greeting
  host:   "xutopia",      // hostname shown in prompt + footer
  branch: " main",       // prompt git branch
  path:   "~/",           // prompt path

  kernel: "linux 6.17.0-35",
  wm:     "openbox",
  distro: "lubuntu",

  defaultEngine: "google", // fallback search engine
  bangs: { ... },          // !g !yt !gh !aw !mdn etc.
  links: [ ... ],          // categories + bookmarks
  theme: { ... },          // optional CSS variable overrides
};
```

## topics
`startpage` `firefox` `newtab` `catppuccin` `dotfiles` `ricing` `arch-linux` `hyprland` `terminal` `minimal` `dark-theme` `vanilla-js` `single-file`
