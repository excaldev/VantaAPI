📘 README.md
🧩 Overview

This project provides a backend API built with FastAPI to support a Roblox Studio plugin designed for developer productivity.

The plugin connects to this API to:

Track usage of external libraries (e.g., networking modules, utility packages)
Scan code comments for actionable tasks like --TODO, --FIX, etc.
Notify users when libraries they use may require updates
✨ Features
📦 Library Tracking
Collects and manages metadata about libraries used in Roblox projects
Helps developers maintain consistency across projects
Enables future update notifications
✅ TODO / FIX Scanner
Parses scripts for comment patterns such as:
--TODO
--FIX
--BUG
Automatically aggregates them into a clean task list inside the plugin
🔄 Update Reminder System
Detects comments like:
--UPDATE LIB_NAME
--CHECK VERSION
Cross-references with API data to notify users when updates are available
⚙️ Customizable Settings
UI customization (themes, colors)
File/directory ignore rules
Scan behavior configuration
🏗️ Tech Stack
Backend: FastAPI
Language: Python
Client: Roblox Studio Plugin (Luau)
🔐 Authentication (Planned / Optional)
API Key-based authentication
OAuth integration (future consideration)
Token-based user identification per plugin owner
📡 API Responsibilities
Receive and store library usage data
Process update metadata
Serve plugin configuration and responses
Support scalable user requests

The Roblox plugin communicates with the API to:

Send detected libraries
Fetch update info
Sync TODO/FIX tracking data
🛠️ Future Improvements
Real-time update notifications
Version comparison system
Team collaboration features
Web dashboard
🤝 Contributing

Pull requests are welcome! Please open an issue first to discuss major changes.

📄 License

MIT License
