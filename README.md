

# Meals Searching App

A simple web application that allows users to search for meals using the **TheMealDB API**. The app fetches meal data from the public API and displays meal names, images, and recipe details in a clean and responsive UI.

## 🍽️ Features

* ✅ Search meals by name
* ✅ Fetch results from **TheMealDB API**
* ✅ Displays meal image + title
* ✅ Shows recipe instructions on click
* ✅ Fully responsive design
* ✅ Clean and beginner-friendly JavaScript code

## 🛠️ Tech Stack

* **HTML5** – App structure
* **CSS3** – UI design
* **JavaScript (ES6+)** – API fetching & dynamic rendering
* **TheMealDB API** – Meal data source

## 🔗 API Used

**Base URL:**

```
https://www.themealdb.com/api/json/v1/1/search.php?s=
```

**Example:**

```
https://www.themealdb.com/api/json/v1/1/search.php?s=chicken
```

## 📂 Project Structure

```
meals-searching-app/
│── index.html
│── style.css
│── script.js
└── assets/
```

## 📦 How to Run

1. Clone the repository:

```bash
git clone https://github.com/Krishnakumar-14/searching-app.git
```

2. Open the project folder:

```bash
cd searching-app
```

3. Run the app by opening **index.html** in your browser.

## ✅ How the App Works

1. User types a meal name in the search bar
2. JavaScript sends a request to TheMealDB API
3. API returns a list of meals
4. Meals are displayed with:

   * Image
   * Name
   * “View Recipe” button
5. Clicking the recipe shows cooking instructions

## 📌 Sample JavaScript Code (API Fetch)

```javascript
async function searchMeal() {
    const query = document.getElementById("search").value;

    const res = await fetch(
        `https://www.themealdb.com/api/json/v1/1/search.php?s=${query}`
    );

    const data = await res.json();
    displayMeals(data.meals);
}
```

## 🚀 Future Enhancements

* Add category-based meal filtering
* Add video tutorials (YouTube links from API)
* Add favorites section using localStorage
* Add pagination for long results

## 🤝 Contributing

Feel free to contribute by opening a pull request or suggesting improvements.




