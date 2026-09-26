<p align="center">
  <a href="https://github.com/pournasseh/52hertz">
    <img src="https://raw.githubusercontent.com/pournasseh/52hertz/main/assets/img/logo-v.png" alt="52Hertz" width="180">
  </a>
</p>

<h1 align="center">52Hertz</h1>

<p align="center">
  <strong>A radio does not have to be a stream.</strong><br>
  Deterministic radio from published content + shared time.
</p>

<p align="center">
  <a href="https://github.com/pournasseh/52hertz">Full</a> ·
  <a href="https://github.com/pournasseh/52hertz-lite">Lite</a> ·
  <a href="https://github.com/pournasseh/52hertz.js">52hertz.js</a>
</p>

<br>

<p align="center">
  <a href="https://github.com/pournasseh/52hertz">
    <img src="https://raw.githubusercontent.com/pournasseh/52hertz/main/assets/img/hero-img.png" alt="52Hertz radio" width="760">
  </a>
</p>

## One idea, three layers

Most internet radio begins with a stream: something stays online and continuously pushes audio.

52Hertz starts from a smaller primitive:

```
published station + shared clock → current item + exact offset
```

If every listener has the same published station and the same clock, each listener can independently work out what should be playing **right now**.

<table>
<tr>
<td width="33%" valign="top">
<h3><a href="https://github.com/pournasseh/52hertz">52Hertz</a></h3>
The complete self-hosted station manager: media library, programmes, schedules, publishing, public player, PWA support, backups, deployment docs, and an optional Icecast-compatible origin.
<br><br>
<a href="https://github.com/pournasseh/52hertz/releases/tag/v1.0.0-rc.3"><strong>1.0.0-rc.3 →</strong></a>
</td>
<td width="33%" valign="top">
<h3><a href="https://github.com/pournasseh/52hertz-lite">52Hertz Lite</a></h3>
The same idea reduced to static hosting: a browser editor/player, `station.json`, and hosted audio. No PHP, database, or always-on playout server required.
<br><br>
<a href="https://github.com/pournasseh/52hertz-lite/releases/tag/v1.0.0-rc.3"><strong>1.0.0-rc.3 →</strong></a>
</td>
<td width="33%" valign="top">
<h3><a href="https://github.com/pournasseh/52hertz.js">52hertz.js</a></h3>
The deterministic clock by itself: give it a station and a time; it gives you the item that should be playing and the exact offset inside it.
<br><br>
<a href="https://github.com/pournasseh/52hertz.js/releases/tag/v0.2.1"><strong>0.2.1 →</strong></a>
</td>
</tr>
</table>

## Engineering highlights

- **Deterministic playout:** listeners independently derive the same current item and exact offset from published state plus time.
- **Three deployment surfaces:** a full PHP/SQLite station manager, a static-hosting Lite edition, and a dependency-free ESM primitive.
- **Edge-case driven clocking:** explicit clock-skew handling, deterministic DST behavior, revision handovers, and media-boundary recovery.
- **Release engineering:** independent CI, reproducible archives, SHA-256 release assets, deployment hardening, and security-focused tests.

## Why 52Hertz

The name comes from the 52-hertz whale story: a voice remembered for calling on a frequency unlike the others.

52Hertz is built around a simple goal in the other direction: **lower the infrastructure threshold between having something to say and being able to run your own station.**

It does not remove hosting, bandwidth, law, moderation, or the realities of publishing. It removes one unnecessary assumption: that scheduled radio must begin with continuous streaming infrastructure.

---

<p align="center">
  <em>If a radio is content plus a shared clock, the transmitter can be much smaller than we thought.</em>
</p>
