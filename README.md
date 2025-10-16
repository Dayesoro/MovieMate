# 🎬 MovieMate

<div align="center">
  <img src="./public/hero.png" alt="MovieMate Hero" width="600" />
  
  <p align="center">
    <strong>Find Movies You'll Enjoy Without the Hassle</strong>
  </p>
  
  <p align="center">
    <!-- Big, obvious live demo button -->
    <a href="https://your-deployment-url.example.com" target="_blank" rel="noopener noreferrer">
      <img alt="Live Demo - Click to open" src="https://img.shields.io/badge/Live%20Demo-CLICK%20TO%20OPEN-blue?style=for-the-badge" />
    </a>
  </p>

  <p align="center">
    👉 Click the blue button above to open the live project.
  </p>
  
  <p align="center">
    A modern, responsive movie discovery application built with React and powered by The Movie Database (TMDB) API.
  </p>
  
  <p align="center">
    <a href="#features">Features</a> •
    <a href="#tech-stack">Tech Stack</a> •
    <a href="#getting-started">Getting Started</a> •
    <a href="#api-setup">API Setup</a> •
    <a href="#screenshots">Screenshots</a>
  </p>
</div>

---

## ✨ Features

- 🔍 **Smart Search**: Real-time movie search with debounced input to optimize API calls
- 📈 **Trending Movies**: Discover the most searched movies based on user activity
- 🎨 **Modern UI**: Beautiful, responsive design built with Tailwind CSS
- ⚡ **Fast Performance**: Built with Vite for lightning-fast development and builds
- 📱 **Mobile-First**: Fully responsive design that works on all devices
- 🗄️ **Data Persistence**: Search analytics stored using Appwrite backend
- ⭐ **Movie Details**: View ratings, release year, language, and more
- 🖼️ **High-Quality Posters**: Crisp movie posters from TMDB

## 🛠️ Tech Stack

### Frontend

- **React 19** - Modern React with latest features
- **Vite** - Fast build tool and development server
- **Tailwind CSS** - Utility-first CSS framework
- **React Use** - Collection of essential React hooks

### Backend & Database

- **Appwrite** - Backend-as-a-Service for data persistence
- **The Movie Database (TMDB) API** - Movie data and images

## 🚀 Getting Started

### Prerequisites

- Node.js (version 16 or higher)
- npm or yarn package manager
- TMDB API key
- Appwrite account and project

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/moviemate.git
   cd moviemate
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Set up environment variables**

   Create a `.env` file in the root directory:

   ```env
   VITE_TMDB_API_KEY=your_tmdb_api_key_here
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
   VITE_APPWRITE_TABLE_ID=your_appwrite_table_id
   ```

4. **Start the development server**

   ```bash
   npm run dev
   ```

5. **Open your browser**

   Navigate to `http://localhost:5173` to view the application.

## 🔧 API Setup

### The Movie Database (TMDB) API

1. Visit [TMDB API](https://www.themoviedb.org/settings/api)
2. Create an account and request an API key
3. Add your API key to the `.env` file as `VITE_TMDB_API_KEY`

### Appwrite Setup

1. Create an account at [Appwrite](https://cloud.appwrite.io/)
2. Create a new project
3. Set up a database with a table containing these attributes:
   - `searchTerm` (String)
   - `count` (Integer)
   - `poster_url` (String)
   - `movie_id` (Integer)
4. Add your Appwrite credentials to the `.env` file

## 📱 Screenshots

<div align="center">
  <img src="./public/preview-bg.jpg" alt="MovieMate Interface" width="800" />
  
  *Beautiful, modern interface with trending movies and search functionality*
</div>

## 🏗️ Project Structure

```
moviemate/
├── public/
│   ├── hero-bg.png
│   ├── hero.png
│   ├── logo.png
│   ├── no-movie.png
│   ├── search.svg
│   └── star.svg
├── src/
│   ├── components/
│   │   ├── MovieCard.jsx
│   │   ├── Search.jsx
│   │   └── Spinner.jsx
│   ├── assets/
│   │   └── react.svg
│   ├── App.css
│   ├── App.jsx
│   ├── appwrite.js
│   ├── index.css
│   └── main.jsx
├── .env
├── package.json
├── vite.config.js
└── README.md
```

## 🎯 Key Components

- **App.jsx**: Main application component with state management and API calls
- **MovieCard.jsx**: Reusable component for displaying movie information
- **Search.jsx**: Search input component with real-time functionality
- **Spinner.jsx**: Loading indicator component
- **appwrite.js**: Backend integration for data persistence

## 🚀 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for providing the movie data API
- [Appwrite](https://appwrite.io/) for the backend-as-a-service platform

---

<div align="center">
  <p>⭐ Star this repo if you found it helpful!</p>
</div>
