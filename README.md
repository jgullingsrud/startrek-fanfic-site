# Star Trek Encyclopedia

A comprehensive reference guide to the Star Trek universe, featuring detailed articles about characters, technologies, species, ships, and more from across all Star Trek series and films.

## Features

- **Markdown-based articles**: Easy-to-write and maintain content
- **LCARS-inspired design**: Clean, responsive interface inspired by Star Trek's iconic LCARS interface
- **Category browsing**: Organized by Characters, Technology, Species, Ships, Planets, Organizations, Events, and Science
- **Featured articles**: Highlighted content on the homepage
- **Client-side rendering**: Fast, static site using marked.js for Markdown parsing

## Getting Started

Simply open `index.html` in your web browser to view the site.

For development with live reload:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server
```

Then navigate to `http://localhost:8000` in your browser.

## Project Structure

```
.
├── index.html              # Main homepage
├── article.html            # Article viewer page
├── css/
│   ├── styles.css         # Main site styling
│   └── article.css        # Article-specific styling
├── articles/               # Markdown articles organized by category
│   ├── characters/
│   ├── technology/
│   ├── species/
│   ├── ships/
│   ├── planets/
│   ├── organizations/
│   ├── events/
│   └── science/
└── README.md              # This file
```

## Writing Articles

Articles are written in Markdown and stored in the `articles/` directory, organized by category.

### Creating a New Article

1. Create a new `.md` file in the appropriate category folder
2. Write your article using Markdown syntax
3. Add the article to the `articleMap` in `article.html`

Example article mapping:
```javascript
const articleMap = {
    'picard': 'articles/characters/picard.md',
    'warp-drive': 'articles/technology/warp-drive.md',
    // Add your article here
};
```

### Markdown Tips

- Use `#` for main heading (article title)
- Use `##` for major sections
- Use `###` for subsections
- Tables, lists, links, and images are all supported
- Code blocks and blockquotes render with custom styling

## Sample Articles

The site includes sample articles to demonstrate the format:

- **Jean-Luc Picard**: Character biography and career highlights
- **Warp Drive**: Comprehensive overview of FTL propulsion technology
- **Vulcans**: Species profile including culture, history, and abilities
- **USS Enterprise NCC-1701**: Ship specifications and service history

## Future Enhancements

- Search functionality across all articles
- Article navigation and related links
- Category index pages
- Article history and revision tracking
- Mobile app version
- Offline support
- User contributions and editing workflow

## Contributing

This is a personal project, but suggestions and corrections are welcome! Feel free to submit pull requests or open issues for bugs and feature requests.

## License

MIT License - Feel free to use this project as a template for your own encyclopedia or wiki site.

---

*Live long and prosper* 🖖
