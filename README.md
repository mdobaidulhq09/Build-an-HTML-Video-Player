# 🎬 Advanced HTML5 Video Integration: A Multi-Source Strategy

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Web-Design](https://img.shields.io/badge/Responsive-Web--Design-blueviolet)](https://www.freecodecamp.org/)

## 📌 Project Overview
Embedding a video is easy; ensuring it plays for **100% of your users** is the real challenge. This repository demonstrates a professional-grade implementation of the HTML5 `<video>` element. 

Inspired by the **freeCodeCamp Responsive Web Design** curriculum, this project solves the critical issue of browser fragmentation and ensures a seamless User Experience (UX).

---

## 🚀 The Core Problem & Professional Solution

### ❌ The Problem: Browser Fragmentation
Different browsers (Chrome, Safari, Firefox, Edge) use different rendering engines. A `.mov` file might play perfectly on an iPhone (Safari) but fail completely on an older Windows machine or certain versions of Firefox.

### ✅ The Solution: Adaptive Multi-Sourcing
This implementation uses a **fallback hierarchy**. By providing multiple file formats, we ensure that the browser automatically selects the best-supported version, reducing error rates to zero.

---

## 🛠️ Technical Implementation & Structure

```html
<video
  width="640"
  loop
  controls
  muted
  poster="[https://cdn.freecodecamp.org/curriculum/labs/past-event2.jpg](https://cdn.freecodecamp.org/curriculum/labs/past-event2.jpg)"
>
  <source src="video.mp4" type="video/mp4">
  
  <source src="video.webm" type="video/webm">
  
  <source src="video.ogg" type="video/ogg">
  
  <source src="video.mov" type="video/quicktime">

  <p>Your browser doesn't support HTML5 video. Here is a <a href="video.mp4">link to the video</a> instead.</p>
</video>
