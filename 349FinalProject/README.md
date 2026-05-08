# 🍽️ Cooking Web App


> Originally developed as part of coursework at California State University, Fullerton. (https://github.com/JosephRan1324)
> This repository has been migrated to my personal GitHub for archival, portfolio purposes, and possible continued development.



A full-featured React-based recipe web application that allows users to browse, search, filter, and view details of various recipes. Users can also manage their favorites and plan meals.

## 🚀 Features

- 🔍 **Search** recipes by title or ingredients
- 🎯 **Filter** by difficulty
- 📃 **Detailed view** of each recipe with ingredients, directions, nutrition, and image
- ❤️ **Favorites** system for saving preferred recipes
- 📅 **Meal planner** functionality
- 🖼️ **Local and remote images** for recipes
- 🗂️ Data-driven UI using a `recipes.json` file

## 🛠️ Tech Stack

- React (with Hooks)
- React Router DOM
- JSON for mock data
- CSS (or your preferred styling method)

## 📁 Folder Structure

```
src/
│
├── components/
│   ├── SearchBar.js
│   ├── FilterPanel.js
│   ├── RecipeCard.js
│   ├── RecipeDetail.js
│   ├── Favorites.js
│   └── MealPlanner.js
│
├── data/
│   └── recipes.json
|
├── styles/
│   └── global.css
|
├── App.jsx
└── main.jsx
```

## 🧑‍🍳 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/cooking-web-app.git
cd cooking-web-app
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the development server

```bash
npm run dev
```

> Make sure you're using a bundler like **Vite** or **Create React App** configured to allow local image imports from `/public/images`.

## 🖼️ Adding Images

- Place your image files inside `public/images/`.
- In `recipes.json`, reference them like this:

```json
"image": "/images/pumpkinPie.png"
```

- Webpack/Vite will resolve paths from `src/`, so make sure the folder and file names match.

## 🔧 Notes

- If you're using Vite, ensure that `server.allowedHosts` is correctly set in `vite.config.js` if you see a "Blocked request" error.
- For persistent storage (e.g., saving favorites), consider adding localStorage or connecting to a backend in future iterations.

## 📜 License

MIT License — feel free to use and modify for personal or commercial use.
