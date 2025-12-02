🛠️ Newb Data Generator
A streamlined, offline-first web tool designed to empower developers and contributors to effortlessly generate JSON data snippets for the Newb Shaders Hub app.
Say goodbye to manual JSON syntax errors! This tool provides an intuitive interface to create shader and developer profiles that strictly adhere to the app's data schema.
✨ Key Features
🔄 Dual Mode: seamlessly switch between generating JSON for Shaders (shader-list-testing.json) and Developers (developers/X.json).
➕ Dynamic Inputs: Add unlimited download links and screenshot URLs with a single click.
🌗 Dark Mode Support: Features a beautiful, high-contrast UI that respects your system theme (with a manual toggle).
⚡ Instant Preview: Watch your JSON update in real-time as you type.
📋 One-Click Copy: Instantly copy the perfectly formatted JSON snippet to your clipboard.
🔒 Zero Dependencies: Runs entirely in your browser. No server, no installation, no fuss.
🚀 Getting Started
1. Setup
This is a single-file tool, so you don't need npm, node, or a local server.
Download the index.html file from this repository.
Double-click the file to open it directly in your web browser (Chrome, Edge, Firefox, etc.).
2. Generating a Shader Entry
Use this mode to add a new shader to the main application list.
Select "Add Shader" at the top of the page.
Fill in the required details:
ID: A unique numeric identifier for the shader.
Creator ID: This must match the filename of a developer (e.g., 0_devendrn).
Download Links: Add multiple mirrors (MCPACK, ZIP, etc.).
Screenshots: Add URLs for the image gallery.
Platforms: Select all supported devices.
Copy the generated JSON from the right-hand panel.
Paste it into the main array inside your shader-list-testing.json file.
3. Generating a Developer Profile
Use this mode when introducing a new creator to the ecosystem.
Select "Add Developer" at the top.
Fill in the details:
Dev ID: This determines the filename (e.g., 0_devendrn).
Socials: Add links for GitHub, YouTube, or Discord.
Copy the generated JSON.
Create a new file in the developers/ folder named exactly as your Dev ID (e.g., 0_devendrn.json) and paste the content there.
📂 File Structure
This tool supports the following data architecture:
/ (Root)
├── index.html                   # 🛠️ This Generator Tool
├── shader-list-testing.json     # 📄 Main array of all shaders
├── developer-list-testing.json  # 🗺️ Mapping of Dev IDs to filenames
└── developers/                  # 👤 Individual developer profiles
    ├── 0_devendrn.json
    └── 1_xenon.json


🤝 Contributing
Want to improve this tool? Contributions are welcome!
Edit index.html directly.
The tool uses Tailwind CSS via CDN, so you can use standard utility classes right away.
Icons are provided by Lucide Icons.
<p align="center">
Made with ❤️ for the <b>Newb Shaders Community</b>.
</p>
