<p align="center">
  <a href="https://github.com/pournasseh/52hertz">
    <img src="https://raw.githubusercontent.com/pournasseh/52hertz/main/assets/img/logo-v.png" alt="52Hertz" width="190">
  </a>
</p>

<h1 align="center">52Hertz</h1>

<p align="center">
  <strong>A radio does not have to be a stream.</strong><br>
  Open-source tools for deterministic, shared-clock radio.
</p>

<p align="center">
  <a href="https://github.com/pournasseh/52hertz/actions/workflows/ci.yml"><img src="https://github.com/pournasseh/52hertz/actions/workflows/ci.yml/badge.svg" alt="52Hertz CI"></a>
  <a href="https://github.com/pournasseh/52hertz-lite/actions/workflows/ci.yml"><img src="https://github.com/pournasseh/52hertz-lite/actions/workflows/ci.yml/badge.svg" alt="52Hertz Lite CI"></a>
  <a href="https://github.com/pournasseh/52hertz.js/actions/workflows/ci.yml"><img src="https://github.com/pournasseh/52hertz.js/actions/workflows/ci.yml/badge.svg" alt="52hertz.js CI"></a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/pournasseh/52hertz/main/assets/img/hero-img.png" alt="52Hertz radio" width="760">
</p>

## One idea, three repositories

<table>
<tr>
<td width="33%" valign="top">
<h3><a href="https://github.com/pournasseh/52hertz">52Hertz</a></h3>
The complete self-hosted station manager: PHP + SQLite, media library, programmes, schedules, publishing, public player, PWA support, and an optional Icecast-compatible origin.
<br><br>
<a href="https://github.com/pournasseh/52hertz/releases/tag/v1.0.0-rc.3"><strong>v1.0.0-rc.3 →</strong></a>
</td>
<td width="33%" valign="top">
<h3><a href="https://github.com/pournasseh/52hertz-lite">52Hertz Lite</a></h3>
The same core idea reduced to static hosting: a browser editor, <code>station.json</code>, hosted audio, and a synchronized player. No PHP. No database.
<br><br>
<a href="https://github.com/pournasseh/52hertz-lite/releases/tag/v1.0.0-rc.3"><strong>v1.0.0-rc.3 →</strong></a>
</td>
<td width="33%" valign="top">
<h3><a href="https://github.com/pournasseh/52hertz.js">52hertz.js</a></h3>
The primitive by itself: pure ESM, no dependencies, no audio API. Give it a station and a time; it returns what should be playing and the exact offset.
<br><br>
<a href="https://github.com/pournasseh/52hertz.js/releases/tag/v0.2.1"><strong>v0.2.1 →</strong></a>
</td>
</tr>
</table>

## The primitive

```text
published station + shared clock → current item + exact offset
```

Traditional internet radio starts with a continuous stream. 52Hertz asks a
smaller question: if every listener has the same published station definition
and the same clock, why can't each listener independently derive what is on
**right now**?

That makes scheduled radio possible without requiring a permanent playout
process. Hosting and bandwidth still exist; the always-on streaming origin is
no longer a prerequisite for the deterministic player.

## Why 52Hertz

The name is a reference to the 52-hertz whale story: a voice remembered for
calling on an unusual frequency.

The project is built around the opposite outcome — lowering the infrastructure
threshold between having something to say and being able to run your own
station.

<p align="center">
  <a href="https://github.com/pournasseh/52hertz"><strong>Full</strong></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/pournasseh/52hertz-lite"><strong>Lite</strong></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/pournasseh/52hertz.js"><strong>Primitive</strong></a>
</p>
