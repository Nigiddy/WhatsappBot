# WhatsApp Bot 🤖

A Python-based WhatsApp automation bot that provides multiple messaging capabilities through a graphical user interface. This bot allows users to send messages automatically, schedule birthday greetings, send bulk messages, and set timed messages.

## 🎯 Project Description

WhatsApp Bot is a desktop application that automates WhatsApp messaging tasks using Selenium WebDriver. It provides a user-friendly GUI built with Tkinter and offers four main functionalities for different messaging scenarios. The bot interacts with WhatsApp Web to send messages automatically, making it useful for personal reminders, birthday greetings, and bulk messaging needs.

## ✨ Features

### 1. **Send Message X Times** (Blue Option)
- Send the same message multiple times to a single contact
- Configurable message count
- Phone number validation with country code support
- Real-time message delivery through WhatsApp Web

### 2. **Celebrate Birthday** (Orange Option)
- Automated birthday message scheduling
- Store contact information and birthday details in JSON format
- Automatic message delivery on matching dates
- Add new birthday entries through the interface

### 3. **Send Message to Multiple People** (Red Option)
- Bulk messaging to multiple contacts
- Dynamic contact list management
- Single message broadcast to multiple recipients
- Useful for announcements and group communications

### 4. **Scheduled Messaging** (Green Option)
- Time-based message scheduling
- Hour and minute precision
- Automatic message delivery at specified times
- Perfect for reminders and scheduled communications

## 🛠️ Tech Stack

### **Frontend**
- **Tkinter** - Python's standard GUI toolkit
- **Canvas-based UI** - Custom graphical interface design

### **Backend**
- **Python 3.x** - Core programming language
- **Selenium WebDriver** - Web automation framework
- **ChromeDriver/GeckoDriver** - Browser automation drivers

### **Libraries & Dependencies**
- **selenium==4.2.0** - Web automation
- **tkinter** - GUI framework (built-in)
- **json** - Data serialization (built-in)
- **datetime** - Date/time handling (built-in)
- **socket** - Network connectivity (built-in)
- **time** - Time utilities (built-in)

### **External Services**
- **WhatsApp Web** - Primary messaging platform
- **Chrome/Firefox Browser** - Web automation target

## 📁 Folder Structure Overview

```
WhatsappBots/
├── WhatsappBot.py          # Main application file
├── requirements.txt         # Python dependencies
├── birthdays.json          # Birthday contact database
├── chromedriver            # Chrome WebDriver executable
├── geckodriver             # Firefox WebDriver executable
├── images/                 # Application screenshots and assets
│   ├── Main.jpeg          # Main interface screenshot
│   ├── Option1.jpeg       # Option 1 interface
│   ├── Option1R.jpeg      # Option 1 result
│   ├── Option2.jpeg       # Option 2 interface
│   ├── Option3.jpeg       # Option 3 interface
│   └── Option4.jpeg       # Option 4 interface
├── executable/             # Additional executable files
└── .gitignore             # Git ignore patterns
```

## 📋 Requirements

### **System Requirements**
- **Operating System**: Windows, macOS, or Linux
- **Python Version**: Python 3.7 or higher
- **RAM**: Minimum 4GB (8GB recommended)
- **Storage**: 100MB free space

### **Browser Requirements**
- **Google Chrome** (recommended) or **Mozilla Firefox**
- **ChromeDriver** or **GeckoDriver** (included in project)

### **Python Dependencies**
```
selenium==4.2.0
```

### **Environment Variables**
- **TODO**: No specific environment variables required
- **TODO**: WhatsApp Web session management handled locally

## 🚀 Setup Instructions

### **Prerequisites**
1. Ensure Python 3.7+ is installed on your system
2. Download and install Google Chrome or Firefox browser
3. Verify internet connectivity for WhatsApp Web access

### **Installation Steps**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/aydinnyunus/WhatsappBOT.git
   cd WhatsappBOT
   ```

2. **Create Virtual Environment**
   ```bash
   python3 -m venv venv
   ```

3. **Activate Virtual Environment**
   - **Windows:**
     ```cmd
     venv\Scripts\activate
     ```
   - **macOS/Linux:**
     ```bash
     source venv/bin/activate
     ```

4. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

5. **WebDriver Setup**
   - **Chrome**: Ensure `chromedriver` is in the project root
   - **Firefox**: Ensure `geckodriver` is in the project root
   - **Note**: Update WebDriver paths in `WhatsappBot.py` if needed

6. **Run the Application**
   ```bash
   python WhatsappBot.py
   ```

### **First-Time Setup**
1. Launch the application
2. Click on any option to start
3. Scan WhatsApp Web QR code when prompted
4. Wait for WhatsApp Web to load completely
5. Begin using the bot features

## 📱 Usage Guide

### **Getting Started**
1. **Launch**: Run `python WhatsappBot.py`
2. **Interface**: The main window displays four colored options
3. **Selection**: Click on any colored option to access its features

### **Feature Usage**

#### **Send Message X Times (Blue)**
1. Click the blue "Send Message X Times" option
2. Enter your message in the "Message" field
3. Specify the number of times to send
4. Enter the phone number with country code (e.g., 90500000000)
5. Click "Send" and scan QR code if prompted

#### **Celebrate Birthday (Orange)**
1. Click the orange "Celebrate Birthday" option
2. **Add New Contact**: Use "Add" button to store birthday information
3. **Auto-Send**: Messages are automatically sent on matching dates
4. **Data Storage**: Information is saved in `birthdays.json`

#### **Send to Multiple People (Red)**
1. Click the red "Send Message to X Person" option
2. Enter your message
3. Use "Add" to add phone numbers to the list
4. Click "Send" to broadcast to all contacts

#### **Scheduled Messaging (Green)**
1. Click the green "Send Message at Specific Time" option
2. Enter your message
3. Set the hour (0-23) and minutes (0-59)
4. Enter the phone number
5. Click "Send" to schedule the message

### **Important Notes**
- **QR Code**: Scan WhatsApp Web QR code when prompted
- **Timing**: Allow 15 seconds for WhatsApp Web to load
- **Validation**: Phone numbers must include country code
- **Scheduling**: Time-based messages use system clock

## 🤝 Contributing Guide

### **Getting Started**
1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Commit your changes: `git commit -m 'Add feature'`
5. Push to the branch: `git push origin feature-name`
6. Submit a Pull Request

### **Development Setup**
1. Clone your forked repository
2. Set up the development environment (see Setup Instructions)
3. Install development dependencies if needed
4. Make changes and test locally
5. Ensure code follows Python PEP 8 standards

### **Code Style**
- Use meaningful variable and function names
- Add comments for complex logic
- Follow Python PEP 8 formatting guidelines
- Include error handling for user inputs

### **Testing**
- Test all four main features before submitting
- Verify WebDriver compatibility
- Test with different phone number formats
- Validate error handling and user feedback

## 🔧 Possible Improvements

### **Security Enhancements**
- **TODO**: Implement input sanitization for phone numbers
- **TODO**: Add rate limiting to prevent abuse
- **TODO**: Secure storage of contact information
- **TODO**: Add user authentication system

### **Performance Optimizations**
- **TODO**: Implement async message sending
- **TODO**: Add message queue management
- **TODO**: Optimize WebDriver initialization
- **TODO**: Reduce sleep times for faster operation

### **Feature Enhancements**
- **TODO**: Add message templates
- **TODO**: Implement contact groups management
- **TODO**: Add message delivery confirmation
- **TODO**: Support for media messages (images, files)
- **TODO**: Add message history and logging
- **TODO**: Implement backup and restore functionality

### **User Experience**
- **TODO**: Improve error messages and validation
- **TODO**: Add progress bars for bulk operations
- **TODO**: Implement dark/light theme toggle
- **TODO**: Add keyboard shortcuts
- **TODO**: Create system tray integration

## 📚 Learning Resources

### **Core Technologies**
- [Python Official Documentation](https://docs.python.org/)
- [Selenium WebDriver Documentation](https://selenium-python.readthedocs.io/)
- [Tkinter Tutorial](https://docs.python.org/3/library/tkinter.html)
- [WhatsApp Web API](https://web.whatsapp.com/)

### **Related Tools & Libraries**
- [ChromeDriver Downloads](https://chromedriver.chromium.org/)
- [GeckoDriver Downloads](https://github.com/mozilla/geckodriver/releases)
- [Python Virtual Environments](https://docs.python.org/3/library/venv.html)
- [Git Version Control](https://git-scm.com/doc)

### **Web Automation Resources**
- [Selenium Best Practices](https://selenium-python.readthedocs.io/getting-started.html)
- [Web Scraping Ethics](https://www.scraperapi.com/blog/web-scraping-ethics/)
- [Browser Automation Patterns](https://www.selenium.dev/documentation/webdriver/)

## 🎯 Next Steps

### **Priority Tasks for Production Readiness**

1. **High Priority**
   - **Input Validation**: Implement comprehensive input sanitization
   - **Error Handling**: Add robust error handling and user feedback
   - **Rate Limiting**: Implement message sending rate limits
   - **Logging**: Add comprehensive logging for debugging

2. **Medium Priority**
   - **Configuration File**: Create config file for customizable settings
   - **Database**: Replace JSON storage with proper database (SQLite/PostgreSQL)
   - **Testing**: Add unit tests and integration tests
   - **Documentation**: Create API documentation and user manual

3. **Low Priority**
   - **Docker**: Containerize the application for easy deployment
   - **CI/CD**: Set up automated testing and deployment pipeline
   - **Monitoring**: Add application health monitoring
   - **Backup**: Implement automated backup and recovery

### **Suggested Optimizations & Extensions**

1. **Performance Improvements**
   - Implement message queuing system
   - Add connection pooling for WebDriver
   - Optimize memory usage for large contact lists
   - Add caching for frequently accessed data

2. **Feature Extensions**
   - **API Integration**: Create REST API for external integrations
   - **Web Dashboard**: Build web-based management interface
   - **Mobile App**: Develop companion mobile application
   - **Plugin System**: Allow third-party extensions

3. **Scalability Enhancements**
   - **Multi-Instance Support**: Handle multiple WhatsApp accounts
   - **Load Balancing**: Distribute message load across instances
   - **Database Scaling**: Implement database sharding and replication
   - **Microservices**: Break down into smaller, focused services

4. **Enterprise Features**
   - **User Management**: Multi-user access control
   - **Audit Logging**: Track all message activities
   - **Compliance**: GDPR and data protection compliance
   - **Integration**: Connect with CRM and business tools

---

## 📄 License

This project is open source. Please check the repository for specific licensing information.

## 👨‍💻 Author

**Yunus Aydın**
- [LinkedIn](https://linkedin.com/in/yunus-ayd%C4%B1n-b9b01a18a/)
- [GitHub](https://github.com/aydinnyunus/WhatsappBOT)
- [Instagram](https://instagram.com/aydinyunus_/)
- [Twitter](https://twitter.com/aydinnyunuss)

---

**Note**: This bot is for educational and personal use. Please respect WhatsApp's Terms of Service and use responsibly. The developers are not responsible for misuse of this tool.





