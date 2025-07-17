# Web Archive Bookmarklet

A simple JavaScript bookmarklet that allows you to archive the current webpage to the Wayback Machine (web.archive.org) with a single click.

## Description

This bookmarklet redirects the current webpage's URL to `https://web.archive.org/save/{URL}`, triggering the Wayback Machine to archive the page. It's a lightweight tool for quickly preserving webpages for future reference.

## Installation

1. Copy the following JavaScript code:

   ```javascript
   javascript:(function() { window.location = 'https://web.archive.org/save/' + encodeURIComponent(window.location.href); })();
   ```

2. Create a new bookmark in your browser:
   - In the bookmark's name field, enter a name (e.g., `Archive This Page`).
   - In the URL field, paste the JavaScript code above.

3. Save the bookmark.

## Usage

1. Navigate to any webpage you want to archive.
2. Click the bookmarklet from your browser's bookmarks menu.
3. You will be redirected to the Wayback Machine, where the page will be archived (if the service is available and the page allows archiving).

## Notes

- **Dependencies**: None. This is a standalone JavaScript bookmarklet.
- **Limitations**: Archiving success depends on the Wayback Machine's server status and whether the target website allows archiving (e.g., some sites may block crawlers via robots.txt).
- **Browser Compatibility**: Works on all modern browsers that support JavaScript bookmarklets.

## License

This project is licensed under the MIT License.
