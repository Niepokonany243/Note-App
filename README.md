# Elegant Rich Dark Notes ✨

A self-contained, single-file HTML notes application featuring a rich text editor, image embedding, persistent local storage, and a refined dark theme.

## Description

This project provides a functional and aesthetically pleasing note-taking experience entirely within a single `.html` file. It leverages modern web technologies (HTML5, CSS3, ES6+ JavaScript) and integrates the Quill.js library for rich text editing capabilities and DOMPurify for security. Notes, including embedded images, are saved directly in your browser's `localStorage`.

The focus is on providing rich content creation within a simple, elegant dark interface, suitable for quick notes, drafts, or snippets.

## Features

*   **Rich Text Editing:** Powered by Quill.js, supporting:
    *   Bold, Italic, Underline, Strikethrough
    *   Blockquotes, Code Blocks
    *   Headers (H1, H2)
    *   Ordered and Bullet Lists
    *   Subscript/Superscript
    *   Text Alignment
    *   Text Color and Background Color
    *   Font Size
    *   Links
*   **Image Embedding:** Upload local images directly into your notes (stored as base64).
*   **Persistent Storage:** Notes are automatically saved to the browser's `localStorage`.
*   **Elegant Dark Theme:** Default dark mode designed for comfortable viewing.
*   **Note Coloring:** Assign a background color tag to each note for visual organization.
*   **Search:** Filter notes by title or content keywords.
*   **Sorting:** Sort notes by modification date (newest/oldest) or title (A-Z/Z-A).
*   **CRUD Operations:** Add, Edit, and Delete notes.
*   **Responsive Design:** Adapts to different screen sizes.
*   **Single File:** All HTML, CSS, and JavaScript (including embedded library links via CDN) are in one file.
*   **Secure Content:** Uses DOMPurify to sanitize HTML content from the editor before displaying or saving, mitigating XSS risks.

## Technology Stack

*   **HTML5**
*   **CSS3:** (Utilizing CSS Variables for theming)
*   **Vanilla JavaScript (ES6+)**
*   **Quill.js:** (Loaded via CDN) - Rich Text Editor library.
*   **DOMPurify:** (Loaded via CDN) - HTML Sanitizer library for security.
*   **Browser `localStorage`:** For data persistence.

## How to Use

1.  **Download:** Download the `[your-filename].html` file (e.g., `rich-dark-notes.html`).
2.  **Open:** Open the downloaded file directly in a modern web browser (like Chrome, Firefox, Edge, Safari).
3.  **Start Noting:** The application is ready to use immediately. Notes will be saved in the `localStorage` of the browser you are using.

## ⚠️ Important Limitations

*   **Storage Limit (`localStorage`):** Browsers typically limit `localStorage` to 5-10MB per domain. Embedding **many or large images** (which are stored as lengthy base64 strings) **will quickly exceed this limit**, causing saving to fail. This application is **not suitable** for heavy image usage. For robust image storage, server-side solutions or IndexedDB would be required.
*   **Local Data Only:** Notes are stored *only* within the specific browser profile on the computer where you use the file. There is no cloud sync or backup. Clearing your browser's data will erase your notes.
*   **Performance:** While optimized, extremely long notes or notes with numerous large embedded images might impact performance.
*   **Quill Deprecation Warning:** You may see a deprecation warning in the browser console related to `DOMNodeInserted` originating from the Quill.js library. This is an issue within Quill and should not currently affect the app's functionality but indicates the library uses older browser APIs.

## Potential Future Enhancements

*   Implement IndexedDB for larger storage capacity, better handling large notes/images.
*   Add optional cloud sync features (e.g., using Firebase, Supabase, or other backend services).
*   Re-introduce Tags/Labels for better organization.
*   Re-introduce Archiving functionality.
*   Add code syntax highlighting within code blocks.

## License

This project is open source and available under the [MIT License](LICENSE). 

---

Enjoy your elegant note-taking experience!
