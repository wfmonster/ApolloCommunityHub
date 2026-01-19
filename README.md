# Apollo Community Hub 🚀

A retro-futuristic, offline-first community information hub designed for off-grid living. Built with pure HTML and CSS for maximum reliability, minimal power consumption, and easy maintenance.

## Overview

Apollo Community Hub provides essential information and resources for local communities operating independently from the internet. Named after the Apollo missions that united humanity in wonder, this hub serves as a digital beacon for sustainable, connected living—even when disconnected from the grid.

## Features

- **🏠 Homepage** - Emergency contacts, daily schedule, important locations, quick links
- **📦 Resources** - Food, water, tools, energy, communications, medical, education
- **📅 Events** - Weekly schedule, special events, regular programming
- **📖 Guides** - Solar power, radio comms, water purification, first aid, food preservation
- **ℹ️ About** - Mission, values, coordinators, community agreements

## Design Philosophy

- **Offline-First**: Works entirely without internet connection
- **Low Power**: Pure HTML/CSS, no JavaScript overhead
- **Mobile-Ready**: Responsive design for all screen sizes
- **Print-Friendly**: Guides can be printed for field reference
- **Easy to Edit**: Simple HTML that anyone can modify

## Getting Started

### Viewing Locally

Simply open `index.html` in any web browser:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

### Hosting on Local Network

To make the hub accessible to other devices on your local network:

**Using Python (if available):**
```bash
# Python 3
python -m http.server 8080

# Then access at http://your-ip:8080
```

**Using a Raspberry Pi or similar:**
1. Install a lightweight web server (nginx, lighttpd, or Apache)
2. Copy these files to the web root (usually `/var/www/html/`)
3. Access via the device's local IP address

**mDNS/Bonjour (optional):**
Configure your server to respond to `apollo.local` for easier access.

## File Structure

```
solarpunk/
├── index.html          # Homepage
├── resources.html      # Community resources
├── events.html         # Schedule & events
├── guides.html         # Practical how-to guides
├── about.html          # Community info
├── styles.css          # Shared styling
├── README.md           # This file
├── CLAUDE.MD           # AI assistant context
├── project-roadmap.md  # Development log
└── .gitignore          # Git ignore rules
```

## Customization

### Updating Content

All pages use simple HTML. To update:

1. Open any `.html` file in a text editor
2. Find the section you want to change
3. Edit the text between the HTML tags
4. Save and refresh your browser

### Changing Colors

Edit the CSS variables at the top of `styles.css`:

```css
:root {
    --apollo-gold: #F4A020;      /* Primary accent */
    --apollo-orange: #E85D04;    /* Secondary accent */
    --space-black: #0D1117;      /* Background dark */
    --space-navy: #161B22;       /* Background medium */
    /* ... etc */
}
```

### Adding New Pages

1. Copy an existing page as a template
2. Update the `<title>` and content
3. Set the correct nav link as `active`
4. Link to it from other pages

## Power Considerations

This hub is designed for solar-powered, battery-backed systems:

- **No JavaScript** = Lower CPU usage = Less power draw
- **Small file sizes** = Fast loading = Less network/storage activity
- **Static files** = No database = No background processes

Estimated power savings vs. dynamic CMS: 50-80% less server power consumption.

## Contributing

This is a community resource. To contribute:

1. Suggest changes at the weekly Council Meeting
2. Contact the Site Coordinator
3. Submit updates via the physical bulletin board

For technical contributions, edit files directly and test in a browser before deploying.

## Credits

- Created during **Solarpunk Automation Workshop**, January 2026
- Site Coordinator: Phyllis J. Beck
- Design aesthetic: Retro-Futuristic / NASA-Punk

## License

This project is shared freely for community use. Adapt it for your own community hub.

---

*"Where the light gathers"* ✨
