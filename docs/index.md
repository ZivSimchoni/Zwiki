---
hide:
    - toc
    - navigation
    - footer
title: Home
---

<center><h1>:material-button-cursor: Heres quick navigation buttons for your convince.</h1></center>

<style>
.container { 
  display: grid;
  grid-template-columns: minmax(10px, auto)  minmax(10px, auto) ;
  grid-template-rows: auto auto auto auto auto;
  grid-auto-columns: min-content;
  grid-auto-rows: auto;
  gap: 0px 2px;
  padding left: 2px;
  padding right: 2px;
  grid-auto-flow: row;
  justify-content: space-evenly; 
  align-content: space-evenly; 
  justify-items: center; 
  align-items: center; 
  grid-template-areas:
    "android ios"
    "windows programs"
    "linux links"
    "github programming"
    "win-key mac-key";
}

.android { grid-area: android; }

.ios { grid-area: ios; }

.windows { grid-area: windows; }

.programs { grid-area: programs; }

.win-key { grid-area: win-key; }

.mac-key { grid-area: mac-key; }

.github { grid-area: github; }

.programming { grid-area: programming; }

.links { grid-area: links; }

.linux { grid-area: linux; }
</style>

<div class="container" markdown>
 <div class="android" markdown> [:fontawesome-brands-android: **Android**](./Wiki/Android.md){ .md-button .md-button--primary } </div>
  <div class="ios" markdown> [:fontawesome-brands-linux: **Linux**](./Wiki/Linux.md){ .md-button .md-button--primary } </div>
  <div class="windows" markdown>[:fontawesome-brands-windows: **Windows**](./Wiki/Windows.md){ .md-button .md-button--primary }</div>
  <div class="linux" markdown> [:fontawesome-brands-app-store-ios: **IOS**](./Wiki/IOS.md){ .md-button .md-button--primary } </div>
  <div class="programs" markdown> [:fontawesome-solid-download: **Programs**](./Wiki/Programs.md){ .md-button .md-button--primary }</div>
  <div class="links" markdown>[:fontawesome-solid-link: **Links & Repos**](./Wiki/Links.md){ .md-button .md-button--primary }</div>
  <div class="github" markdown> [:fontawesome-brands-github: **GitHub**](./Wiki/GitHub.md){ .md-button .md-button--primary }</div>
  <div class="programming" markdown> [:fontawesome-solid-code: **Programming**](./Wiki/Programming.md){ .md-button .md-button--primary }</div>
  <div class="win-key" markdown> [:fontawesome-brands-microsoft: **Windows Shortcuts**](./Wiki/keyboard-shortcuts/Windows-Keyboard-Shortcuts.md){ .md-button .md-button--secondary } </div>
  <div class="mac-key" markdown> [:fontawesome-brands-apple: **Mac Shortcuts**](./Wiki/keyboard-shortcuts/Mac-Keyboard-Shortcuts.md){ .md-button .md-button--secondary } </div>
</div>

<h6>Content page layout<br> Navigation | Content | TOC </h6>

> _This is a list of guides and sources that I've collected/created.<br>
> I'm not a professional - just a man who likes to learn and share knowledge.<br>
> Please read the [disclaimer](./about-me/Wiki-ETC/disclaimer.md).<br>
> There are probably some errors or typos and If you have any suggestions, please let me know! - [Contribution Guidelines](./about-me/Wiki-ETC/contributions.md)_
