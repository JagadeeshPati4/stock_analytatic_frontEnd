# Frontend - Vite + React with Material UI

This project is a frontend application built using Vite, React, and Material UI. It fetches and displays transaction data using APIs and provides various charts and tables to visualize the data.

## Features
- Displays a transactions table with search and pagination.
- Allows selection of a month to filter transactions.
- Displays statistics including total sales, sold items, and unsold items.
- Provides bar and pie charts for transaction analysis.

## Tech Stack
- **Vite** - Fast build tool for React projects.
- **React.js** - Frontend framework for UI development.
- **Material UI (MUI)** - For styling and pre-built UI components.
- **Axios** - For API requests.
- **Recharts** - For data visualization (charts and graphs).

## Installation

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Steps
1. Clone the repository:
   ```sh
   git clone <repository_url>
   cd <project_directory>
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the development server:
   ```sh
   npm run dev
   ```
4. Open the app in your browser at `http://localhost:5173`.

## Project Structure
```
├── src
│   ├── components        # Reusable components
│   ├── pages             # Main pages
│   ├── services          # API calls
│   ├── App.js            # Main application file
│   ├── main.jsx          # Entry point
│   ├── styles.css        # Global styles
│   └── ...
├── public                # Static assets
├── package.json          # Project dependencies
├── vite.config.js        # Vite configuration
└── README.md             # Project documentation
```

## API Endpoints Used
- `GET /transactions?month=<month>&search=<query>&page=<page>` - Fetch transactions
- `GET /statistics?month=<month>` - Fetch sales statistics
- `GET /bar-chart?month=<month>` - Fetch price range distribution
- `GET /pie-chart?month=<month>` - Fetch category-wise item count

## Deployment
To build for production, run:
```sh
npm run build
```
This will create a `dist/` folder with optimized assets ready for deployment.

## Contributing
1. Fork the repository.
2. Create a new branch (`feature-branch`).
3. Commit your changes.
4. Push and create a Pull Request.

## License
This project is open-source and available under the [MIT License](LICENSE).

