# Portfolio 3D Galaxy

An interactive 3D portfolio where each of my projects is a planet orbiting a sun. Built with Three.js as a single HTML file, with no build step and no framework.

**Live demo:** https://eya-eya1.github.io/portfolio-3d-galaxy/
**Classic version:** https://eya-eya1.github.io

<!-- Add a screenshot: upload an image to this repository, then replace the line below with ![Preview](screenshot.png) -->

## Features

- Eleven rotating planets, one per project, colour-coded by category.
- Hover a planet to see its name. Click it to fly the camera to it and read its description and GitHub link.
- Mouse parallax: the camera follows the pointer.
- Menu with five sections: About, Skills, Badge, Projects, and Contact.
- Project list as a fallback for touch screens and keyboard users.
- Responsive layout. The details panel becomes a bottom sheet on phones.
- Respects the `prefers-reduced-motion` setting and shows a message if WebGL is unavailable.
- Keyboard support: Tab through the menu and project list, Escape closes the panel.

## Tech stack

| Part | Tool |
|---|---|
| 3D rendering | [Three.js](https://threejs.org/) r128, loaded from cdnjs |
| Structure, style, logic | HTML, CSS, and vanilla JavaScript |
| Fonts | Bricolage Grotesque and Newsreader (Google Fonts) |
| Hosting | GitHub Pages |

## Project structure

```
portfolio-3d-galaxy/
├── index.html   # the whole site: markup, styles, and scripts
└── README.md
```

## Run locally

1. Clone the repository:
   ```bash
   git clone https://github.com/EYA-EYA1/portfolio-3d-galaxy.git
   ```
2. Open `index.html` in a modern browser. An internet connection is needed to load Three.js and the fonts.

## Customise

All content is stored in plain arrays and objects inside `index.html`.

- **Add or edit a project:** find `var P=[` and add a line in this format:
  ```js
  ["Project name","Category","Short description","repository-name"],
  ```
  Valid categories are `Algorithms and validation`, `Business tools`, `Games`, `Tools`, and `Web`. Each project gets its own planet automatically.
- **Change colours:** edit the `COL` object for planets, and the CSS variables at the top of the stylesheet for the interface.
- **Update text and contact details:** edit the `V` object, which holds the About, Skills, Badge, and Contact sections.

## Deploy on GitHub Pages

1. Push `index.html` to the `main` branch.
2. Go to **Settings**, then **Pages**.
3. Under **Branch**, select `main` and `/ (root)`, then save.
4. The site goes live after one or two minutes.

## Browser support

Works in current versions of Chrome, Edge, Firefox, and Safari with WebGL enabled.

## Credits

Designed and maintained by **Eya Hamdaoui**. The code was written with the help of an AI assistant, and the content, project selection, and customisation are my own.

## Contact

- GitHub: [@EYA-EYA1](https://github.com/EYA-EYA1)
- Email: eyahamdaoui4@gmail.com
