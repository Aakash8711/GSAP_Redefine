# 🎮 GSAP Redefine

A cinematic, highly interactive gaming website built with **React, GSAP, Tailwind CSS, and modern frontend animation techniques**.

This project is a frontend recreation inspired by the visual experience of the **Zentry Redefine gaming website**, focusing heavily on immersive animations, scroll interactions, video transitions, 3D effects, and responsive UI.

The goal of this project was not simply to create a static website, but to explore how far a modern React frontend can be pushed using **GSAP-powered interactions and visual storytelling**.

---

## ✨ Features

- 🎬 Cinematic video-based Hero section
- ⚡ GSAP-powered animations
- 📜 Scroll-triggered animations using GSAP ScrollTrigger
- 🎥 Multiple background and feature videos
- 🖱️ Interactive 3D mouse-tilt effects
- 🌀 Clip-path based transitions
- 💫 3D text reveal animations
- 🎨 Custom typography and fonts
- 🎧 Background audio with animated audio indicator
- 🧩 Reusable React components
- 📱 Responsive design
- 🖼️ Bento-style feature cards
- 🔮 SVG filter effects
- 🎭 Animated navigation bar
- 🖱️ Interactive hover effects
- 🌊 Smooth visual transitions
- 🧱 Reusable Button and AnimatedTitle components
- 🎮 Gaming-inspired UI and visual language

---

## 🛠️ Tech Stack

### Frontend

- **React**
- **JavaScript**
- **Vite**
- **Tailwind CSS**

### Animation

- **GSAP**
- **@gsap/react**
- **GSAP ScrollTrigger**

### Icons

- **React Icons**

### Assets

- MP4 videos
- WebP images
- SVG graphics
- Custom WOFF2 fonts
- MP3 audio

---

## 📦 Installation

Follow these steps to run the project locally.

### 1. Clone the repository

```bash
git clone https://github.com/Aakash8711/GSAP_Redefine.git
```

### 2. Navigate into the project

```bash
cd GSAP_Redefine
```

### 3. Install the project dependencies

```bash
npm install
```

### 4. Install GSAP

Install GSAP separately:

```bash
npm install gsap
```

### 5. Install GSAP React integration

This project uses GSAP with React through `@gsap/react`:

```bash
npm install @gsap/react
```

### 6. Install React Icons

The project uses React Icons for interface icons:

```bash
npm install react-icons
```

You can also install all three together:

```bash
npm install gsap @gsap/react react-icons
```

### 7. Start the development server

```bash
npm run dev
```

Vite will start the development server and provide a local URL, usually:

```text
http://localhost:5173
```

Open the URL in your browser.

---

## 🚀 Quick Setup

If you want the shortest installation process:

```bash
git clone https://github.com/Aakash8711/GSAP_Redefine.git

cd GSAP_Redefine

npm install

npm install gsap @gsap/react react-icons

npm run dev
```

---

## 📁 Project Structure

```text
GSAP_Redefine/
│
├── public/
│   │
│   ├── audio/
│   │   └── loop.mp3
│   │
│   ├── fonts/
│   │   ├── circularweb-book.woff2
│   │   ├── general.woff2
│   │   ├── robert-medium.woff2
│   │   ├── robert-regular.woff2
│   │   └── zentry-regular.woff2
│   │
│   ├── img/
│   │   ├── about.webp
│   │   ├── contact-1.webp
│   │   ├── contact-2.webp
│   │   ├── entrance.webp
│   │   ├── gallery-1.webp
│   │   ├── gallery-2.webp
│   │   ├── gallery-3.webp
│   │   ├── gallery-4.webp
│   │   ├── gallery-5.webp
│   │   ├── logo.png
│   │   ├── play.svg
│   │   ├── stones.webp
│   │   ├── swordman.webp
│   │   └── swordman-partial.webp
│   │
│   └── videos/
│       ├── feature-1.mp4
│       ├── feature-2.mp4
│       ├── feature-3.mp4
│       ├── feature-4.mp4
│       ├── feature-5.mp4
│       ├── hero-1.mp4
│       ├── hero-2.mp4
│       ├── hero-3.mp4
│       └── hero-4.mp4
│
├── src/
│   │
│   ├── components/
│   │   ├── About.jsx
│   │   ├── AnimatedTitle.jsx
│   │   ├── Button.jsx
│   │   ├── Contact.jsx
│   │   ├── Features.jsx
│   │   ├── Footer.jsx
│   │   ├── Hero.jsx
│   │   ├── Navbar.jsx
│   │   ├── RoundedCorners.jsx
│   │   └── Story.jsx
│   │
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── eslint.config.js
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

---

# 🧩 Main Sections

The website is divided into several major sections.

## 🧭 Navbar

The navigation bar provides:

- Navigation links
- Dynamic visibility based on scrolling
- Audio controls
- Animated navigation transitions
- Responsive navigation behavior

The navbar detects the user's scroll direction.

When scrolling down, it can hide.

When scrolling up, it reappears.

This creates a cleaner cinematic browsing experience.

---

## 🎬 Hero Section

The Hero section is the visual centerpiece of the project.

It includes:

- Multiple videos
- Video transitions
- GSAP animations
- ScrollTrigger
- Interactive mouse movement
- 3D transformations
- Clip-path animations
- Loading state
- Responsive layout

The hero video system cycles through multiple videos:

```text
Hero Video 1
      ↓
Hero Video 2
      ↓
Hero Video 3
      ↓
Hero Video 4
      ↓
Hero Video 1
```

The Hero also contains an interactive video preview that responds to mouse movement.

---

# ⚡ GSAP Animations

GSAP is one of the main technologies behind this project.

The project uses GSAP for:

- Element transitions
- Scroll animations
- Timeline-based animations
- 3D transforms
- Opacity transitions
- Clip-path animations
- Mouse interactions
- Navigation animations
- Video transitions

---

## 📜 ScrollTrigger

GSAP ScrollTrigger is used to connect animations with the user's scroll position.

For example:

```js
gsap.to(".element", {
  scale: 1,
  scrollTrigger: {
    trigger: ".element",
    start: "top center",
    end: "bottom center",
    scrub: true,
  },
});
```

This allows the animation to progress as the user scrolls instead of playing independently.

The project uses this technique extensively for its cinematic transitions.

---

# 🧠 React + GSAP

This project uses the official React integration:

```bash
npm install @gsap/react
```

The project uses:

```js
import { useGSAP } from "@gsap/react";
```

This makes it easier to manage GSAP animations inside React components.

Example:

```js
useGSAP(() => {
  gsap.to(".element", {
    opacity: 1,
    duration: 1,
  });
});
```

This approach keeps animation logic connected to the React component lifecycle.

---

# 🖱️ 3D Mouse Tilt

Several sections use mouse movement to create interactive 3D effects.

The cursor position is converted into rotation values.

Conceptually:

```text
Mouse position
      ↓
Calculate distance from center
      ↓
Convert to rotateX / rotateY
      ↓
GSAP animation
      ↓
3D visual movement
```

The effect uses CSS transformations such as:

```css
transform:
  perspective(700px)
  rotateX(...)
  rotateY(...)
  scale3d(...);
```

This technique is used throughout interactive cards and visual elements.

---

# 🧩 AnimatedTitle Component

`AnimatedTitle.jsx` is a reusable component created specifically for animated headings.

It provides:

- 3D text movement
- Scroll-based animation
- Word staggering
- Rotation
- Opacity transitions
- Custom styling

Instead of duplicating animation code for every title, the same component can be reused across different sections.

Example:

```jsx
<AnimatedTitle
  title="Redefine your world"
  containerClass="..."
/>
```

---

# 🎴 Bento Feature Cards

The Features section uses a Bento-style layout.

Each card can contain:

- Video
- Text
- Icons
- Hover effects
- Mouse-based 3D movement
- Responsive sizing

The cards are designed to create a dynamic gaming interface rather than a traditional grid.

---

# 🌀 SVG Filter Effects

The Story section uses SVG filters to create a distorted visual effect.

The project contains a reusable:

```text
RoundedCorners.jsx
```

component that defines SVG filter functionality.

This works together with:

- SVG filters
- CSS clip-path
- GSAP
- Image transformations

to create more organic visual transitions.

---

# 🎧 Audio

The project includes background audio:

```text
public/audio/loop.mp3
```

The navigation contains an audio control.

The audio indicator uses animated bars to visually communicate the audio state.

When audio is active, the bars animate.

When audio is paused, the animation stops.

---

# 🎨 Custom Fonts

The project uses custom fonts to recreate its gaming-inspired visual identity.

Included fonts:

```text
Circular Web
General
Robert Medium
Robert Regular
Zentry
```

These fonts are stored inside:

```text
public/fonts/
```

and are loaded through the project's CSS.

---

# 🎥 Video Assets

The project uses multiple MP4 assets for immersive visual experiences.

### Hero Videos

```text
hero-1.mp4
hero-2.mp4
hero-3.mp4
hero-4.mp4
```

### Feature Videos

```text
feature-1.mp4
feature-2.mp4
feature-3.mp4
feature-4.mp4
feature-5.mp4
```

The videos are integrated directly into React components and controlled through state and GSAP animations.

---

# 🧱 Reusable Components

The project is structured around reusable React components.

### `Button.jsx`

Reusable button component supporting:

- Title
- Left icon
- Right icon
- Custom classes
- Custom IDs

### `AnimatedTitle.jsx`

Reusable animated heading component.

### `Navbar.jsx`

Navigation and audio controls.

### `Hero.jsx`

Hero video experience and major introductory animations.

### `About.jsx`

About section with large image expansion animation.

### `Features.jsx`

Interactive Bento-style feature cards.

### `Story.jsx`

Story section with image interactions and SVG effects.

### `Contact.jsx`

Contact section and CTA.

### `Footer.jsx`

Footer navigation and social links.

### `RoundedCorners.jsx`

Reusable SVG filter definitions.

---

# 🎯 Learning Objectives

This project was built to explore and practice advanced frontend development concepts such as:

- React component architecture
- GSAP animation
- ScrollTrigger
- React + GSAP integration
- CSS transforms
- 3D interactions
- Mouse tracking
- Clip-path
- SVG filters
- Video manipulation
- Audio controls
- Responsive UI
- Tailwind CSS
- Reusable components
- Interactive web design

---

# 🧪 Development

Start the development server:

```bash
npm run dev
```

Build the project:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

Run ESLint:

```bash
npm run lint
```

---

# 📦 Required Packages

The core packages required by this project include:

```bash
npm install gsap @gsap/react react-icons
```

Along with the project's React and Vite dependencies:

```bash
npm install
```

If you're setting up the project from scratch, the recommended sequence is:

```bash
npm install
npm install gsap @gsap/react react-icons
npm run dev
```

---

# 🌐 Deployment

Because this is a Vite-based frontend project, it can be deployed using platforms such as:

- Vercel
- Netlify
- GitHub Pages
- Cloudflare Pages

Before deployment, create a production build:

```bash
npm run build
```

The production files will be generated inside:

```text
dist/
```

---

# ⚠️ Performance Considerations

This project contains multiple high-resolution videos, images, fonts, and animations.

For production deployment, consider:

- Compressing MP4 files
- Using optimized video formats
- Adding poster images
- Lazy-loading media
- Reducing simultaneous video playback
- Optimizing images
- Loading fonts efficiently
- Supporting reduced-motion preferences

These optimizations can significantly improve performance, especially on mobile devices.

---

# ♿ Accessibility

Because this project relies heavily on animation, future improvements can include support for:

```css
@media (prefers-reduced-motion: reduce) {
  /* Reduce or disable animations */
}
```

Other accessibility improvements can include:

- Better button labels
- Improved keyboard navigation
- Improved video accessibility
- Better semantic HTML
- Accessible navigation states
- Appropriate image alt text

---

# 🚧 Future Improvements

Possible improvements for future versions:

- [ ] Add a live production deployment
- [ ] Improve mobile performance
- [ ] Optimize all videos
- [ ] Add reduced-motion support
- [ ] Improve accessibility
- [ ] Add more interactive sections
- [ ] Improve loading experience
- [ ] Add responsive video sources
- [ ] Improve SEO metadata
- [ ] Add Open Graph metadata
- [ ] Add project screenshots
- [ ] Add a live demo link
- [ ] Improve documentation
- [ ] Add automated deployment

---

# 📚 What I Learned

Building this project helped me understand how animation can become part of the actual architecture of a website rather than simply being decorative.

Some of the major concepts explored were:

```text
React
  +
GSAP
  +
ScrollTrigger
  +
CSS
  +
Video
  +
SVG
  +
Mouse interaction
  =
Interactive frontend experience
```

The project especially focuses on creating a connection between **scrolling, movement, video, typography, and user interaction**.

---

# 🙌 Credits

This project is a frontend recreation inspired by the visual design and interaction patterns of the **Zentry Redefine** website.

The purpose of this project is educational and to practice modern frontend development, animation, and interactive web experiences.

All original trademarks, branding, and intellectual property belong to their respective owners.

---

# 👨‍💻 Author

**Aakash**

GitHub:

https://github.com/Aakash8711

---

# ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.

It helps support continued experimentation with creative frontend development.

---

## 🚀 Run It Locally

The complete setup in one place:

```bash
git clone https://github.com/Aakash8711/GSAP_Redefine.git

cd GSAP_Redefine

npm install

npm install gsap @gsap/react react-icons

npm run dev
```

Then open the local Vite development URL in your browser and explore the experience. 🎮