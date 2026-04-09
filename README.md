# VegEats – Smart Recipe Recommendation iOS App

## Overview
VegEats is an iOS application designed to help users discover healthy recipes based on ingredients available in their kitchen. The app promotes sustainable food consumption by reducing waste and encouraging balanced eating habits.

## Objective
- Suggest recipes based on user-selected ingredients  
- Reduce food waste by utilizing available resources  
- Provide a simple and intuitive cooking experience  

## Key Features

### 🍽 Recipe Discovery
- Browse recipes with images and key details  
- Search functionality to filter recipes dynamically  
- Ingredient-based recipe selection  

### ❤️ Favorites System
- Save recipes using a like (heart) feature  
- Access saved recipes in a dedicated profile section  

### 👥 User Interaction
- Input ingredients manually  
- Select number of people for meal preparation  
- Navigate through a guided cooking flow  

### 📱 UI/UX Design
- Tab-based navigation (Recipes & Profile) :contentReference[oaicite:0]{index=0}  
- Clean card-based layout for recipes  
- Smooth navigation using SwiftUI NavigationStack  

## Architecture

### Data Management
- Used **ObservableObject pattern** for state management  
- Centralized data using shared instances:
  - `RecipeData` for recipes and favorites :contentReference[oaicite:1]{index=1}  
  - `SharedData` for user-related data :contentReference[oaicite:2]{index=2}  

### Models
- `Recipe` model stores:
  - Ingredients, preparation time, nutritional values :contentReference[oaicite:3]{index=3}  
- `Learner` and `Team` models for user-related features :contentReference[oaicite:4]{index=4}  

### Views & Components
- **RecipeCardView** → Displays list of recipes with search functionality :contentReference[oaicite:5]{index=5}  
- **RecipeDetailView** → Shows detailed recipe information and allows saving :contentReference[oaicite:6]{index=6}  
- **ProfileView** → Displays saved and suggested recipes :contentReference[oaicite:7]{index=7}  
- **IngredientView** → Allows users to input ingredients dynamically :contentReference[oaicite:8]{index=8}  

### Navigation Flow
- Tab-based navigation using `TabView`  
- NavigationStack used for hierarchical navigation  
- Modal sheets used for additional views (e.g., recipe details)

## Technologies Used
- Swift  
- SwiftUI  
- Xcode  
- MVVM-like architecture  

## Implementation Highlights
- Dynamic filtering of recipes using search bar  
- Real-time UI updates using `@Published` and `@State`  
- Modular view structure for scalability  
- Reusable components for UI consistency  

## Impact
- Encourages sustainable food usage  
- Helps users make quick and healthy meal decisions  
- Improves user experience with intuitive design  

## Future Improvements
- AI-based recipe recommendation system  
- Integration with grocery delivery services  
- Nutritional tracking and personalization  

## Author
Sudip Kishan Sarker  
Apple Developer Academy – University of Naples Federico II
