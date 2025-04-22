# Sunset Challenge

This repository contains the Sunset Challenge project, which consists of two main components:

- `sunset-challenge-web`: The frontend application
- `sunset-challenge-api`: The backend API

## Project Structure

```
sunset-challenge/
├── sunset-challenge-web/    # Frontend application
└── sunset-challenge-api/    # Backend API
```

## Getting Started

### Cloning the Repository

To clone this repository with all submodules:

```bash
git clone --recursive git@github.com:brunownk/sunset-challenge.git
```

If you've already cloned the repository without submodules, you can initialize them with:

```bash
git submodule update --init --recursive
```

### Working with Submodules

Each submodule is a separate Git repository. To update submodules to their latest commits:

```bash
git submodule update --remote
```

To work on a specific submodule:

```bash
cd sunset-challenge-web  # or sunset-challenge-api
# Make your changes
git add .
git commit -m "Your changes"
git push
```

Then, in the parent repository:

```bash
git add sunset-challenge-web  # or sunset-challenge-api
git commit -m "Update submodule"
git push
```

## Individual Repositories

Each component can be accessed independently:

- Frontend: [sunset-challenge-web](https://github.com/brunownk/sunset-challenge-web)
- Backend: [sunset-challenge-api](https://github.com/brunownk/sunset-challenge-api) 