<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=220&section=header&text=CITY%20INFO%20TRAVEL&fontSize=58&fontColor=FFD700&fontAlignY=42&desc=✈️%20Vanilla%20JS%20Travel%20Info%20App%20%C2%B7%20City%20Explorer&descAlignY=62&descColor=DCDCDC&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=700&size=20&duration=2800&pause=900&color=FFD700&center=true&vCenter=true&width=760&lines=%F0%9F%8C%86+No+Frameworks%2C+Pure+Vanilla+JS;%F0%9F%97%BA%EF%B8%8F+Barcelona+%C2%B7+Rome+%C2%B7+Paris+%C2%B7+London;%E2%9C%88%EF%B8%8F+Dynamic+City+Info+%26+Pricing;%F0%9F%8F%86+%231+GitHub+Committer+in+Colombia)](https://git.io/typing-svg)

<br/>

<p align="center">
  <a href="https://github.com/NietoDeveloper">
    <img src="https://img.shields.io/badge/Engineer-Manuel%20Nieto-blue?style=for-the-badge&logo=github"/>
  </a>
  <a href="https://committers.top/colombia#NietoDeveloper">
    <img src="https://img.shields.io/badge/Committers.top-%231%20Colombia-gold?style=for-the-badge"/>
  </a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript">
    <img src="https://img.shields.io/badge/Vanilla-JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000"/>
  </a>
  <a href="https://pages.github.com/">
    <img src="https://img.shields.io/badge/Hosting-GitHub_Pages-222?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge"/>
  </a>
</p>

<p align="center">
  <a href="https://nietodeveloper.github.io/CityInfoTravel/">
    <img src="https://img.shields.io/badge/🌐_Live_Site-nietodeveloper.github.io-FFD700?style=for-the-badge"/>
  </a>
  <a href="https://github.com/NietoDeveloper/CityInfoTravel">
    <img src="https://img.shields.io/badge/📂_Source-NietoDeveloper%2FCityInfoTravel-000000?style=for-the-badge&logo=github&logoColor=FFD700"/>
  </a>
</p>

</div>

---

## 📋 Overview

**City Info Travel** is a travel sales application built with vanilla JavaScript. This tutorial-style project walks through building an app that displays information about different tourist cities and their associated prices. No frameworks or dependencies required.

---

## 🗂️ Project Structure

```text
CityInfoTravel/
└── assets/
    ├── css/          # Stylesheets
    ├── img/            # City images
    └── js/               # JavaScript logic (app.js, ciudades.js)
```

---

## 🔄 City Selection Flow

```mermaid
flowchart LR
    A([👤 Visitor]) -->|Clicks City Link| B[Click Event Listener]
    B -->|Toggle 'active' Class| C[Update Nav State]
    B -->|Look Up City| D[obtenerContenido]
    D -->|Reads| E[ciudades.js\nBarcelona / Rome / Paris / London]
    E -->|Data| F[Update DOM]
    F --> G([📄 Title · Subtitle · Description · Price])

    style A fill:#FFD700,color:#000,stroke:#FFD700
    style D fill:#F7DF1E,color:#000,stroke:#F7DF1E
    style G fill:#000,color:#FFD700,stroke:#FFD700
```

---

## 🛠️ Technologies Used

<div align="center">

| Layer | Technologies |
|:------|:-------------|
| 🎨 **Frontend** | HTML, CSS, JavaScript |
| ☁️ **Hosting** | GitHub Pages |

</div>

---

## ✨ How the JavaScript Works

The provided JavaScript code updates the information displayed on the page when a city link is clicked.

### City Data Import

The `barcelona`, `roma`, `paris`, and `londres` variables are imported from the `ciudades.js` file, which contains the information for each city. This file must be available alongside the main JavaScript code.

### DOM Element Retrieval

The code uses `document.getElementById` to retrieve the DOM elements needed to update the page content:

- **`enlaces`:** A collection of all anchor (`<a>`) elements on the page.
- **`tituloElemento`:** The title element (`<h1>`) where the selected city's title is displayed.
- **`subTituloElemento`:** The subtitle element (`<h2>`) where the selected city's subtitle is displayed.
- **`parrafoElemento`:** The paragraph element (`<p>`) where the selected city's description is displayed.
- **`precioElemento`:** The element where the selected city's price is displayed.

### Click Event Handling

A `click` event is attached to each link via a `forEach` loop. When a link is clicked, the callback function:

- Removes the `active` class from all links (via another `forEach` loop).
- Adds the `active` class to the current link (`this`).
- Retrieves the corresponding city content using the `obtenerContenido` function and the current link's text.
- Updates the DOM elements with the selected city's information.

### City Content Lookup Function

The `obtenerContenido` function takes the link's text as a parameter and returns the corresponding city content from `ciudades.js`, using a `contenido` object to map link text to city data.

### Customizing Content

City content can be customized by editing `ciudades.js`. Each city is represented by an object with properties such as `titulo`, `subtitulo`, `parrafo`, and `precio`.

---

## 🚀 Getting Started

### Prerequisites

- Basic HTML knowledge.
- A development environment to write and run JavaScript.

### Setup

**Step 1 — Clone the repository**

```bash
git clone https://github.com/NietoDeveloper/CityInfoTravel
```

**Step 2 — Open `index.html`** in a web browser.

---

## 👨‍💻 Author

**Manuel Nieto (NietoDeveloper)**

---

## 📄 License

This project is licensed under the **MIT License**.

<div align="center">

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=120&section=footer&animation=fadeIn" width="100%"/>

</div>

























---
iudades.js)
```

---

## 🔄 City Selection Flow

```mermaid
flowchart LR
    A([👤 Visitor]) -->|Clicks City Link| B[Click Event Listener]
    B -->|Toggle 'active' Class| C[Update Nav State]
    B -->|Look Up City| D[obtenerContenido]
    D -->|Reads| E[ciudades.js\nBarcelona / Rome / Paris / London]
    E -->|Data| F[Update DOM]
    F --> G([📄 Title · Subtitle · Description · Price])

    style A fill:#FFD700,color:#000,stroke:#FFD700
    style D fill:#F7DF1E,color:#000,stroke:#F7DF1E
    style G fill:#000,color:#FFD700,stroke:#FFD700
```

---

## 🛠️ Technologies Used

<div align="center">

| Layer | Technologies |
|:------|:-------------|
| 🎨 **Frontend** | HTML, CSS, JavaScript |
| ☁️ **Hosting** | GitHub Pages |

</div>

---

## ✨ How the JavaScript Works

The provided JavaScript code updates the information displayed on the page when a city link is clicked.

### City Data Import

The `barcelona`, `roma`, `paris`, and `londres` variables are imported from the `ciudades.js` file, which contains the information for each city. This file must be available alongside the main JavaScript code.

### DOM Element Retrieval

The code uses `document.getElementById` to retrieve the DOM elements needed to update the page content:

- **`enlaces`:** A collection of all anchor (`<a>`) elements on the page.
- **`tituloElemento`:** The title element (`<h1>`) where the selected city's title is displayed.
- **`subTituloElemento`:** The subtitle element (`<h2>`) where the selected city's subtitle is displayed.
- **`parrafoElemento`:** The paragraph element (`<p>`) where the selected city's description is displayed.
- **`precioElemento`:** The element where the selected city's price is displayed.

### Click Event Handling

A `click` event is attached to each link via a `forEach` loop. When a link is clicked, the callback function:

- Removes the `active` class from all links (via another `forEach` loop).
- Adds the `active` class to the current link (`this`).
- Retrieves the corresponding city content using the `obtenerContenido` function and the current link's text.
- Updates the DOM elements with the selected city's information.

### City Content Lookup Function

The `obtenerContenido` function takes the link's text as a parameter and returns the corresponding city content from `ciudades.js`, using a `contenido` object to map link text to city data.

### Customizing Content

City content can be customized by editing `ciudades.js`. Each city is represented by an object with properties such as `titulo`, 