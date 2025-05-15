# Penal Code Comparison Website

This website allows users to compare different penal codes side by side.

## Website Structure

The website consists of two main parts:
1. A selection page where users choose which codes to compare
2. A comparison view that shows two codes side by side

## File Structure

```
penal_code_compare/
├── index.html              # The main webpage file
└── codes/                  # Folder containing all penal codes
    ├── california/         # Each code has its own folder
    ├── federalCriminal/
    ├── federalSentencing/
    ├── german/
    ├── model/
    ├── newJersey/
    ├── newYork/
    ├── northDakota/
    ├── israel/
    ├── pennsylvania/
    ├── proposedFederal/
    ├── sampleDraft/
    ├── texas/
    └── ucmj/              # Uniform Code of Military Justice
```

Each code folder (like `california/`, `texas/`, etc.) contains 7 HTML files:
- `contents.html` - Table of contents
- `part1.html` - Part I (General Part)
- `preliminary.html` - Preliminary section
- `generalPrinciplesOfLiability.html` - General Principles of Liability
- `generalPrinciplesOfJustification.html` - General Principles of Justification
- `responsibility.html` - Responsibility section
- `inchoateCrimes.html` - Inchoate Crimes section

## How to Update Content

### Step 1: Find the File to Update
1. Go to the `codes` folder
2. Open the folder for the code you want to update (e.g., `newYork` for New York Penal Law)
3. Open the specific section file you want to update (e.g., `preliminary.html`)

### Step 2: Edit the Content
1. Find the line that looks like this:
   ```html
   <p>[Content for New York Penal Law Preliminary goes here]</p>
   ```
2. Replace everything between `<p>` and `</p>` with your content
3. You can use these HTML tags for formatting:
   - For paragraphs: `<p>Your text here</p>`
   - For headings: `<h3>Smaller heading</h3>`
   - For lists:
     ```html
     <ul>
       <li>First item</li>
       <li>Second item</li>
     </ul>
     ```
   - For numbered lists:
     ```html
     <ol>
       <li>First item</li>
       <li>Second item</li>
     </ol>
     ```

### Important Notes
- Don't change anything outside the `<p>...</p>` tags
- Keep the file names exactly as they are
- Don't rename the folders
- Don't delete any files

## Testing Your Changes Locally

Before pushing changes to GitHub, you should always test them on your computer first:

### Opening the Website Locally
1. Find the `index.html` file in your project folder
2. Double-click it (or right-click and select "Open with" → choose your web browser)
3. The website should open in your browser
4. Use it just like you would the live site:
   - Select different codes to compare
   - Check that your new content appears correctly
   - Make sure formatting looks right

### Tips for Testing
1. After making any changes:
   - Save the file you edited
   - Refresh the browser page to see your changes
2. Test on different browsers if possible (Chrome, Safari, Firefox)
3. Check both the selection page and comparison view
4. Common issues to watch for:
   - Missing content
   - Broken formatting
   - Text that runs together
   - Lists that don't format correctly

### If Something Looks Wrong
1. Make sure you saved your changes
2. Check that you only modified text between `<p>` and `</p>` tags
3. Verify your HTML formatting (use Cursor's AI help or VS Code)
4. Compare with other files that work correctly
5. Try closing and reopening the browser

## How to Update the Website on GitHub Pages

### First Time Setup
1. Create a GitHub account if you don't have one
2. Install GitHub Desktop from: https://desktop.github.com/
3. Clone this repository using GitHub Desktop:
   - Click "File" → "Clone Repository"
   - Select this repository
   - Choose where to save it on your computer

### Making Updates
1. Open GitHub Desktop
2. Make sure you're on the main branch
3. Click "Fetch origin" to get the latest changes
4. Make your changes to the files using any text editor
5. In GitHub Desktop:
   - You'll see your changes listed
   - Add a summary of what you changed (e.g., "Updated New York Penal Code preliminary section")
   - Click "Commit to main"
   - Click "Push origin"

### If Something Goes Wrong
- Don't panic! GitHub keeps all previous versions
- You can always go back to a previous version:
  1. Go to the repository on GitHub.com
  2. Click "History"
  3. Find the version you want
  4. Click "Browse files" at that point in history
  5. Download or view the old files

## Getting Help
If you run into technical issues:
1. Check this README file first
2. Look at other code files as examples
3. Contact the website maintainer
4. Consider using ChatGPT or similar AI tools for HTML formatting help

## Recommended Text Editors

While you can use any text editor to modify the HTML files, we recommend using one of these modern editors that make the job easier:

### Option 1: Cursor
Cursor is a free editor that comes with built-in AI assistance, which can be extremely helpful for non-programmers:
1. Download Cursor from https://cursor.sh
2. Install and open it
3. Open the folder containing this project
4. Use the AI chat feature (Cmd+L or Ctrl+L) to ask questions like:
   - "How do I format this text as a numbered list?"
   - "How do I add a new section to this file?"
   - "What's wrong with my HTML formatting?"

### Option 2: Visual Studio Code
VS Code is a popular, free editor with helpful features:
1. Download VS Code from https://code.visualstudio.com
2. Install and open it
3. Open the folder containing this project
4. Helpful features:
   - Syntax highlighting shows HTML tags in different colors
   - Auto-completion helps with HTML tags
   - Preview extensions let you see how your HTML looks
   - Built-in file explorer makes navigation easy

### Tips for Using Either Editor
1. Use "Open Folder" to open the entire project, not just single files
2. The file explorer on the left helps navigate between files
3. Both editors will highlight HTML syntax errors
4. Both support search across all files (Cmd+Shift+F or Ctrl+Shift+F)
5. Both have integrated Git support

## Best Practices
1. Always make one change at a time
2. Write clear commit messages describing what you changed
3. Double-check your changes on the live site after pushing
4. Keep formatting consistent with existing content
5. Back up your content in a separate document before making changes

Remember: The website is designed to be simple and maintainable. If something seems too complicated, there's probably an easier way to do it! 