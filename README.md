# PassX Password Manager

A simple, lightweight web-based password manager that allows you to securely store and manage all your website passwords in one convenient place.

## Features

✨ **Core Features:**
- 🔐 Add and store website credentials (website URL, username, password)
- 🗑️ Delete stored passwords when no longer needed
- 👁️ Masked password display for security
- 📋 Copy passwords to clipboard with one click
- 💾 Local storage - all data stored securely in your browser
- 🎨 Modern, dark-themed user interface
- 📱 Responsive design for desktop use

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge, etc.)
- No server or installation required

### Installation

1. Clone or download this repository
2. Open `index.html` in your web browser
3. Start managing your passwords!

```bash
# Simply open the file in your browser
# Or use a simple HTTP server
python -m http.server 8000
# Then navigate to http://localhost:8000/index.html
```

## Usage

### Adding a Password

1. Navigate to the **"Add a Password"** section
2. Enter the following information:
   - **Website**: The name or URL of the website
   - **Username**: Your username or email for that website
   - **Password**: Your password (displayed as dots for security)
3. Click the **"Submit"** button
4. Your password will appear in the table above

### Viewing Passwords

- All stored passwords are displayed in the table with:
  - **Website** name
  - **Username**
  - **Password** (masked with asterisks for security)
  - A **Delete** button for each entry

### Copying Passwords

1. Click on any password in the table
2. The password will be copied to your clipboard
3. A confirmation message "*(Copied!)*" will appear for 2 seconds
4. Paste the password wherever you need it

### Deleting Passwords

1. Click the **"Delete"** button next to any password entry
2. Confirm the deletion when prompted
3. The password will be permanently removed from your storage

## Technology Stack

- **HTML5** - Semantic markup for the structure
- **CSS3** - Modern styling with custom fonts (Poppins, Noto Sans)
- **Vanilla JavaScript** - Core functionality and interactions
- **Browser localStorage API** - Local data persistence

## File Structure

```
Password manager/
├── index.html      # Main HTML interface
├── script.js       # JavaScript logic and functionality
├── style.css       # Styling and layout
└── README.md       # Documentation (this file)
```

## Security Considerations

⚠️ **Important Security Notes:**

- Passwords are stored in **browser localStorage**, which is **client-side only**
- This is suitable for **personal use** and non-sensitive passwords only
- Do **NOT** use this for storing highly sensitive credentials or passwords
- Clearing your browser data will **permanently delete** all stored passwords
- Anyone with access to your computer can view your stored passwords
- For production use, consider using professional password managers like Bitwarden, 1Password, or LastPass

## Browser Support

This application works on all modern browsers that support:
- HTML5
- ES6 JavaScript
- localStorage API

**Tested on:**
- Google Chrome
- Mozilla Firefox
- Safari
- Microsoft Edge

## How It Works

1. **Add Password**: Form data is collected and stored in browser's localStorage as JSON
2. **Display Passwords**: Data is retrieved from localStorage and rendered in a table
3. **Copy Function**: Uses the Clipboard API to copy passwords
4. **Delete Function**: Filters out the selected entry and updates localStorage
5. **Mask Password**: Password display is masked with asterisks for on-screen security

## Limitations

- Data only persists in the current browser (not synced across devices)
- No encryption of stored data (stored as plain text in localStorage)
- No user authentication or login system
- No backup or recovery mechanism
- Browser-specific storage (different browsers have separate storage)

## Future Enhancements

Potential features for future versions:
- [ ] Add encryption/decryption for stored passwords
- [ ] Export/Import functionality
- [ ] Password strength indicator
- [ ] Search/Filter passwords
- [ ] Categories or tags for passwords
- [ ] Master password protection
- [ ] Cloud sync capability
- [ ] Dark/Light theme toggle

## Contributing

Feel free to fork this project and submit pull requests for any improvements.

## License

This project is open source and available under the MIT License.

## Contact

For questions, suggestions, or issues, please feel free to reach out through the contact section in the application.

---

**Disclaimer**: This password manager is provided as-is for educational and personal use. Use at your own discretion. For storing sensitive or critical passwords, use established password management solutions with professional security standards.

Made with ❤️ by Hiralal
