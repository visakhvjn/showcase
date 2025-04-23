# Showcase

This is a personal showcase website to highlight my skills, projects, and blogs. It includes sections for web services, apps, packages, and the latest blogs fetched from Medium.

## Features

- **Web Services**: Displays a list of web services with demo and repository links.
- **Apps**: Highlights web apps with descriptions, demo links, and repository links.
- **Packages**: Lists packages with details and links to npm or repositories.
- **Blogs**: Fetches and displays random blogs from my Medium RSS feed.

## Project Structure

```
/showcase
├── index.html       # Main HTML file for the showcase
├── data.json        # JSON file containing project data
├── README.md        # Documentation for the project
```

## How to Run

1. Clone the repository or copy the files to your local machine.
2. Open `index.html` in your browser to view the showcase.

## Data Configuration

- Update `data.json` to add or modify the web services, apps, and packages displayed on the site.
- The `data.json` file structure:
  ```json
  {
  	"webservices": [],
  	"apps": [
  		{
  			"name": "App Name",
  			"description": "App description.",
  			"version": "1.0.0",
  			"demoLink": "https://example.com",
  			"repositoryLink": "https://github.com/example"
  		}
  	],
  	"packages": [
  		{
  			"name": "Package Name",
  			"description": "Package description.",
  			"version": "1.0.0",
  			"demoLink": "https://npmjs.com/package/example",
  			"repositoryLink": "https://github.com/example"
  		}
  	]
  }
  ```

## Blog Integration

- Blogs are fetched from the Medium RSS feed using a CORS proxy.
- The RSS feed URL is: `https://medium.com/feed/@vjnvisakh`.

## Notes

- Ensure you have an active internet connection to fetch blogs from Medium.
- The project uses the free CORS proxy `https://api.allorigins.win` to bypass CORS restrictions.

## License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).
