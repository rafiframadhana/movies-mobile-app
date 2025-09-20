# 🎬 Movies Mobile App

A modern React Native mobile application for discovering and exploring movies, built with Expo, TypeScript, and Nativewind. Browse popular movies, search for your favorites, and get detailed information about any film - all in a beautifully designed dark-themed interface.

## ✨ Features

- **Browse Popular Movies**: Discover trending and popular movies on the home screen
- **Search Functionality**: Real-time search with debounced queries for optimal performance
- **Movie Details**: View comprehensive information including:
  - Movie overview and plot
  - Release date and runtime
  - User ratings and vote count
  - Genres and production companies
  - Budget and revenue information
- **Beautiful UI**: Dark-themed interface with purple accent colors and smooth animations
- **Bottom Tab Navigation**: Easy navigation between Home, Search, Saved, and Profile sections
- **Responsive Design**: Optimized grid layout for movie cards with 3-column display

## 🛠️ Tech Stack

- **Framework**: [React Native](https://reactnative.dev/) with [Expo](https://expo.dev/)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Navigation**: [Expo Router](https://docs.expo.dev/routing/introduction/) (file-based routing)
- **Styling**: [Nativewind](https://www.nativewind.dev/) (TailwindCSS for React Native)
- **API**: [The Movie Database (TMDB) API](https://www.themoviedb.org/documentation/api)
- **State Management**: React Hooks with custom `useFetch` hook
- **UI Components**: Custom components with Expo Image and Blur

## 📱 Screenshots

The app features:
- A home screen with the latest movies in a grid layout
- A search screen with real-time movie search capabilities
- Detailed movie information pages with poster images and comprehensive data
- A custom-styled bottom tab navigation with animated highlights

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Expo CLI
- iOS Simulator (for Mac) or Android Emulator

### Environment Setup

1. Clone the repository:
   ```bash
   git clone [your-repo-url]
   cd movies-mobile-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add your TMDB API key:
   ```
   EXPO_PUBLIC_MOVIE_API_KEY=your_tmdb_api_key_here
   ```

   You can get a free API key from [The Movie Database](https://www.themoviedb.org/settings/api)

### Running the App

Start the development server:
```bash
npx expo start
```

Then choose your preferred platform:
- Press `i` for iOS simulator
- Press `a` for Android emulator
- Scan QR code with Expo Go app on your physical device

## 📁 Project Structure

```
movies-mobile-app/
├── app/                    # App screens and navigation
│   ├── (tabs)/            # Tab navigation screens
│   │   ├── index.tsx      # Home screen
│   │   ├── search.tsx     # Search screen
│   │   ├── saved.tsx      # Saved movies (placeholder)
│   │   ├── profile.tsx    # User profile (placeholder)
│   │   └── _layout.tsx    # Tab navigation layout
│   ├── movies/
│   │   └── [id].tsx       # Dynamic movie details screen
│   └── _layout.tsx        # Root layout
├── components/            # Reusable components
│   ├── MovieCard.tsx      # Movie card component
│   └── SearchBar.tsx      # Search input component
├── constants/             # App constants
│   ├── icons.ts          # Icon assets
│   └── images.ts         # Image assets
├── services/             # API and data services
│   ├── api.ts           # TMDB API integration
│   └── useFetch.ts      # Custom fetch hook
├── interfaces/           # TypeScript interfaces
└── tailwind.config.js   # Nativewind/Tailwind configuration
```

## 🎨 Design System

### Color Palette
- **Primary**: `#030014` (Deep navy background)
- **Secondary**: `#151312` (Dark elements)
- **Accent**: `#AB8BFF` (Purple highlights)
- **Light shades**: `#D6C7FF`, `#A8B5DB`, `#9CA4AB`
- **Dark shades**: `#221F3D`, `#0F0D23`

### Typography
The app uses system fonts with various weight classes:
- Regular text: `font-normal`
- Emphasized text: `font-semibold`
- Headers: `font-bold`

## 🔧 Available Scripts

- `npm start` - Start the Expo development server
- `npm run android` - Run on Android emulator
- `npm run ios` - Run on iOS simulator
- `npm run web` - Run in web browser
- `npm run lint` - Run ESLint

## 🚧 Future Enhancements

- [ ] Implement movie saving/favoriting functionality
- [ ] Add user profile and authentication
- [ ] Include movie trailers and video playback
- [ ] Add movie reviews and cast information
- [ ] Implement filtering by genre, year, and rating
- [ ] Add offline support with data caching
- [ ] Include social features (share movies, create lists)

## 📄 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- Movie data provided by [The Movie Database (TMDB)](https://www.themoviedb.org/)
- Built with [Expo](https://expo.dev/) and [React Native](https://reactnative.dev/)
- Styled with [Nativewind](https://www.nativewind.dev/)
