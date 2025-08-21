# MealMate 🍽️

Hi! I'm Abdelrahman Ashraf Lasheen, and this is **MealMate**, an Android app I developed to make discovering, saving, and managing recipes simple and enjoyable. The app follows Material Design principles for a clean, intuitive, and responsive user experience.

---

## Table of Contents
1. [About the App](#about-the-app)  
2. [Features](#features)  
3. [Screens & Navigation](#screens--navigation)  
4. [Tech Stack](#tech-stack)  
5. [Architecture](#architecture)  
6. [Storage & APIs](#storage--apis)  
7. [Testing](#testing)  
8. [Future Improvements](#future-improvements)  
9. [References](#references)  

---

## About the App
MealMate allows users to:

- Discover a wide variety of recipes
- Save favorite recipes for easy access
- Geotag grocery stores or locations
- Access recipes offline

I built this app for Android using Kotlin, Room Database, Firebase, and TheMealDB API. The design is responsive, intuitive, and user-friendly.

---

## Features
- **Recipe Management:** Add, view, and save favorite recipes  
- **Geotagging:** View stores and locations on a map  
- **Offline Access:** Local storage via Room Database  
- **Cloud Storage:** Media stored in Firebase Cloud Storage  
- **API Integration:** Fetch recipes, ingredients, and meal categories from TheMealDB API  
- **User Accounts:** Sign-up, login, and profile customization  

---

## Screens & Navigation
- **Home Screen:** Displays recipes, favorites, and popular meals  
- **Recipe Detail Screen:** Shows recipe instructions and images  
- **Favorites Screen:** Lists saved favorite recipes  
- **Search Screen:** Search recipes by name or ingredients  
- **MapActivity:** Geotag and view grocery stores  
- **Profile & Settings:** Manage account preferences  

**Navigation:** Bottom navigation bar for easy access across all screens.

---

## Tech Stack
- **Language:** Kotlin  
- **Database:** Room (local) & Firebase Realtime Database (cloud)  
- **Media Storage:** Firebase Cloud Storage  
- **Architecture:** MVC pattern  
- **APIs:** TheMealDB API  
- **UI Design:** Material Design Principles  

---

## Architecture
I organized the app using the MVC pattern for clarity and maintainability:

- **Packages:** Separate packages for models, views, repositories, and database management  
- **Adapters & Fragments:** HorizontalRecipeAdapter, RecipeAdapter, HomeFragment, FavouritesFragment, ProfileFragment, SearchFragment  
- **Activities:** LoginActivity, SignUpActivity, AddRecipeActivity, AllRecipesActivity, DetailActivity, MapActivity, SettingActivity, SplashActivity  

This structure ensures modular, testable, and maintainable code.

---

## Storage & APIs
- **Room Database:** Stores favorite recipes for offline access  
- **Firebase Realtime Database:** Stores structured recipe data  
- **Firebase Cloud Storage:** Stores images and media  
- **TheMealDB API:** Fetches recipes, ingredients, and meal categories  

---

## Testing
I implemented both unit and UI tests:

| Test Case                 | Expected Result                           | Status  |
|----------------------------|-------------------------------------------|---------|
| Insert Recipe              | Recipe added to the database              | Passed  |
| Delete Recipe              | Recipe removed from database              | Passed  |
| Get All Favorite Recipes   | Retrieves all saved recipes correctly     | Passed  |
| Search Recipe              | Recipes correctly filtered                | Passed  |
| Favorite Recipe UI Update  | UI updates to reflect favorited recipes   | Passed  |

---

## Future Improvements
- Enhance recipe search with ingredient and category filters  
- Meal planning and calendar features  
- Add nutritional information for meals  
- Use AI to suggest meals based on user preferences and past choices  

---

## References
1. Martinez, D., et al. (2020). *An agile-based integrated framework for mobile application development considering ilities.* IEEE Access.  
2. Delía, L. N., et al. (2017). *Approaches to mobile application development: comparative performance analysis.* Computing Conference.  
3. Biørn-Hansen, A., et al. (2019). *An empirical study of cross-platform mobile development in industry.* Wireless Communications and Mobile Computing.  
4. Huynh, M., & Ghimire, P. (2017). *Browser app approach: can it be an answer to the challenges in cross-platform app development?* JITE: Innovations in Practice.  
5. Latif, M., et al. (2016). *Cross platform approach for mobile application development: a survey.* IT4OD.  
6. Malavolta, I. (2016). *Web-based hybrid mobile apps.* ICSE Proceedings.  
