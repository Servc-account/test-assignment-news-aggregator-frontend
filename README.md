# News Aggregator Frontend

A minimal Angular application that displays news from the backend API.

Use this repository as a [**template**](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) to generate repo in your account and make an assignment in it.

Create a **new** branch, make the task in it, then make a **Pull Request** to the **Master** branch, so we are able to review it and leave some comments if needed.

## Prerequisites

- Node.js 18+ and npm
- The backend service running on port 5000

## Quick Start

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start the development server:**
   ```bash
   npm start
   ```
   or
   ```bash
   ng s
   ```

3. **Access the application:**
   - Frontend: http://localhost:4200
   - Make sure backend is running on http://localhost:5000

## Project Structure

```
src/app/
├── app.module.ts                     # Main application module
├── app-routing.module.ts             # Route configuration
├── app.component.*                   # Root component
├── dtos/
│   └── news.ts                       # News interface
├── services/
│   └── news.service.ts               # API communication service
└── components/
    └── news-list/
        ├── news-list.component.ts    # News display component
        ├── news-list.component.html  # Template
        └── news-list.component.scss  # Styles
```

## Your Task

### Frontend Requirements:
1. **Complete news display** in `news-list.component.html` - show title, description, source, date, link, image(if present)
2. **Add two buttons**:
   - **Refresh**: Manually trigger API news fetch (same as scheduled job)
   - **Show Scraper News**: Display news fetched by web scraper
3. **Default view**: Show API news (fetched by scheduled job every 2 hours)

### Backend Requirements:
- Complete `NewsAggregatorServiceImpl.java` (API integration + web scraping)
- Add endpoints for manual fetching and filtering by source type

### Notes:
- Focus on functionality first, then styling
- Good UI appreciated but don't over-engineer

