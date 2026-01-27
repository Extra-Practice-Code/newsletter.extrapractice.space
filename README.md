# Extra Practice Newsletter Archive

This is the archive website for Extra Practice newsletters. It displays all past newsletters in a browsable format.

## How to Add a New Newsletter

Follow these steps to add a newly sent newsletter to the archive:

### 1. Install the SingleFile Extension

If you haven't already, install the [SingleFile Chrome extension](https://chromewebstore.google.com/detail/singlefile/mpiodijhokgodhhofbcjdecpffjipkle?hl=en). This extension allows you to save a complete webpage as a single HTML file.

### 2. Access the Newsletter in MailerLite

1. Go to [MailerLite](https://www.mailerlite.com/)
2. Navigate to the Campaigns section
3. Find the newsletter that was recently sent
4. Open the preview of the newsletter

### 3. Save the Newsletter with SingleFile

1. With the newsletter preview open in your browser, click the SingleFile extension icon
2. Select "Save page with SingleFile"
3. The extension will process and download a complete HTML file of the newsletter

### 4. Add the File to the Archive

1. Move the downloaded HTML file to the appropriate year folder in `archive/[YEAR]/`
2. Rename the file to a number corresponding to the month it was sent
   - For single-month newsletters: use the month number (e.g., `1.html` for January, `12.html` for December)
   - For combined newsletters: use a hyphenated format (e.g., `1-2.html` for January/February, `9-10.html` for September/October)

**Example file paths:**
- `archive/2025/7.html` for December 2025
- `archive/2024/9-10.html` for September/October 2024

### 5. Update the Index

Open [index.html](index.html) and add a new entry to the newsletter list:

1. Find the appropriate year section (e.g., `<!-- 2025 -->`)
2. Add a new list item at the top of that year's `<ul>` with the format:
   ```html
   <li><a href="archive/YEAR/NUMBER.html">Month - Newsletter Title</a></li>
   ```

**Example:**
```html
<li><a href="archive/2025/7.html">Dec - Got Stability?</a></li>
```

### 6. Test and Deploy

1. Open [index.html](index.html) in a browser to verify the new link works
2. Click the link to ensure the archived newsletter displays correctly
3. Commit and push your changes to deploy the update

---

That's it! The newsletter is now archived and accessible on the website.
