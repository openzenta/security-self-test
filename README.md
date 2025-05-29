# Security Self-Test: Privacy & Online Security

A comprehensive interactive quiz to assess your online security practices and privacy awareness. Test your knowledge across 15 key security domains and receive personalized feedback to improve your digital security posture.

## 🛡️ Features

- **15 Comprehensive Questions** covering essential security practices
- **Real-time Progress Tracking** with visual progress indicator
- **Dark/Light Mode Toggle** for comfortable viewing
- **Detailed Feedback System** with explanations for incorrect answers
- **Responsive Design** that works on desktop and mobile devices
- **Privacy-First Approach** - no data collection or external dependencies
- **Instant Results** with actionable security recommendations

## 📋 Security Areas Covered

The quiz evaluates your practices in these critical security domains:

- Password management and authentication
- Two-factor authentication (2FA) usage
- Software updates and device security
- VPN usage and network security
- Privacy protection while browsing
- Phishing awareness and email security
- Data encryption practices
- Backup strategies
- Social media privacy settings
- Website security verification
- USB/removable media handling
- WiFi router security
- Mobile device protection

## 🎯 Scoring System

- **20-30 Points**: Excellent security practices - you're well-protected!
- **10-19 Points**: Good foundation with room for improvement
- **0-9 Points**: Significant security gaps that need immediate attention

Each question offers multiple choice answers with different point values:
- Best practice (A): 2 points
- Partial implementation (B): 1 point
- Poor/no security (C): 0 points

## 🚀 Getting Started

### Option 1: Direct Use
Simply open the `index.html` file in any modern web browser. No installation or setup required!

### Option 2: Web Server
For a more robust experience, serve the file through a local web server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server package)
npx http-server

# Using PHP
php -S localhost:8000
```

Then navigate to `http://localhost:8000` in your browser.

## 💻 Technical Requirements

- **Browser Compatibility**: Modern browsers (Chrome 60+, Firefox 55+, Safari 12+, Edge 79+)
- **JavaScript**: Required for interactive functionality
- **No External Dependencies**: Self-contained HTML file with embedded CSS and JavaScript
- **Responsive Design**: Works on screens from 320px to 4K

## 📁 File Structure

```
security-self-test/
│
├── index.html          # Main application file
├── README.md           # This documentation
└── LICENSE             # GNU GPLv3 license
```

## 🔧 Customization

### Adding New Questions
To add additional security questions:

1. Update the HTML structure in the quiz container
2. Add the question text to the `questions` array in JavaScript
3. Add the correct answer to the `correctAnswers` array
4. Update the `totalQuestions` variable

### Modifying Scoring
Adjust the scoring system by modifying the `pointsMap` object:

```javascript
const pointsMap = {
    'A': 2,  // Best practice
    'B': 1,  // Partial implementation
    'C': 0   // Poor/no security
};
```

### Styling Changes
All CSS is embedded in the `<style>` section. Key classes:
- `.quiz-container` - Main quiz styling
- `.dark-mode` - Dark theme variations
- `.result-feedback` - Score feedback sections
- `.correct-answers` - Educational feedback styling

## 🎨 Features in Detail

### Dark Mode
- Toggle between light and dark themes
- Persistent during session (resets on page reload for privacy)
- Smooth transitions and consistent color scheme
- Accessible contrast ratios

### Progress Tracking
- Visual progress bar showing completion percentage
- Real-time updates as questions are answered
- Smooth animations for better user experience

### Educational Feedback
- Detailed explanations for suboptimal answers
- Best practice recommendations
- Color-coded feedback (red for user answer, green for correct answer)
- Only shows for questions answered incorrectly

## 🔒 Privacy & Security

- **No Data Collection**: No personal information is stored or transmitted
- **No External Requests**: Completely self-contained application
- **No Cookies**: No tracking or persistent storage
- **Client-Side Only**: All processing happens in your browser
- **Open Source**: Full transparency with GPL v3 license

## 🤝 Contributing

Contributions are welcome! Please feel free to:

1. **Report Issues**: Found a bug or have a suggestion? Open an issue
2. **Submit Pull Requests**: Improvements to questions, styling, or functionality
3. **Translate**: Help make this available in other languages
4. **Share Feedback**: Let us know how the quiz helped improve your security

### Development Guidelines
- Maintain browser compatibility
- Keep the application self-contained (no external dependencies)
- Follow existing code style and structure
- Test across different devices and browsers
- Ensure accessibility standards are met

## 📄 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Created by OpenZenta
- Inspired by the need for better digital security awareness
- Built with privacy and accessibility in mind

## 📞 Support

For questions, suggestions, or issues:
- Open an issue on GitHub

---

**Remember**: Good security is an ongoing process, not a destination. Regularly reassess your practices and stay informed about emerging threats!

## 🔄 Version History

- **v1.0.0** - Initial release with 15 security questions
- Full-featured quiz with dark mode and detailed feedback
- Responsive design and accessibility features
