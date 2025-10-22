# Sharevolume

## Overview

This project was automatically generated based on the following brief:

> Your assigned company: Booking Holdings (BKNG), CIK 0001075531.

Fetch https://data.sec.gov/api/xbrl/companyconcept/CIK0001075531/dei/EntityCommonStockSharesOutstanding.json (set a descriptive User-Agent per SEC guidance).
Read `.entityName`. Filter `.units.shares[]` for entries whose `fy` > "2020" and
includes a numeric `val`.
Save `data.json` with this structure:
`{"entityName": "Booking Holdings", "max": {"val": ..., "fy": ...}, "min": {"val": ..., "fy": ...}}`
where `max` and `min` refer to the highest and lowest `.val`. Break ties however you like.

Render a visually appealing `index.html` where:
- `<title>` and `<h1>` must include the live `entityName`.
- The max/min figures are clearly marked with these IDs:
  `share-entity-name`,
  `share-max-value`, `share-max-fy`,
  `share-min-value`, `share-min-fy`.

If the page is opened as `index.html?CIK=0001018724` (or any other 10-digit CIK),
`fetch()` from the SEC endpoint for that CIK using any proxy, e.g. AIPipe,
replace every ID listed above and the title and H1 without reloading the page.

Also commit the attachment uid.txt as-is.

## Description

This is a web application that implements the requirements specified in the project brief. The application is built using modern web technologies and follows best practices for web development.

## Setup and Usage

This is a static web application that can be run directly in any modern web browser.

### Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/poshikababu/sharevolume.git
   cd sharevolume
   ```

2. Open `index.html` in your web browser:
   ```bash
   # On macOS
   open index.html
   
   # On Linux
   xdg-open index.html
   
   # On Windows
   start index.html
   ```

### Live Demo

The application is automatically deployed to GitHub Pages and can be accessed at:
https://poshikababu.github.io/sharevolume/

## Code Structure

- `index.html` - Main application file containing HTML, CSS, and JavaScript
- `README.md` - This documentation file
- `LICENSE` - MIT License file

## Implementation Details

The application is implemented as a single HTML file that includes:

- **HTML Structure**: Semantic markup for the user interface
- **CSS Styling**: Embedded styles for responsive design and visual presentation
- **JavaScript Logic**: Client-side functionality and interactivity

The code follows modern web development best practices including:
- Responsive design principles
- Accessibility considerations
- Error handling and user feedback
- Clean, maintainable code structure

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Auto-Generated

This project was automatically generated using an LLM-based code deployment system.
