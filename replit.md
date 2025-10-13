# Pillar Bank - Liferay DXP Fragments Demo

## Overview

This project is a demonstration of Liferay DXP fragments for Pillar Bank, showcasing a modern banking website built using component-based architecture. The application serves as a preview environment for custom Liferay fragments, displaying various sections of a professional banking website including hero, services, security, history, and footer components. The project is designed to demonstrate how Liferay DXP fragments can be developed and previewed in isolation before being deployed to a Liferay environment.

The banking website features a complete professional design with sections for account opening, services showcase, security features, company history, and comprehensive footer navigation, all styled with a modern blue-themed banking aesthetic.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
The application uses a component-based architecture where each banking website section is implemented as an independent Liferay fragment. Each fragment contains its own HTML structure, CSS styling, and maintains separation of concerns. The main index.html serves as a preview showcase that loads and displays all fragments together, simulating how they would appear in a complete Liferay DXP site.

### Fragment Structure
Each fragment follows the Liferay DXP fragment standard with individual package.json files and organized src directories containing index.html and index.css files. The fragments include:
- Hero section with call-to-action
- Services grid displaying banking products
- Security features highlight
- Company history and brand story
- Footer with navigation links

### Development Server
A simple Node.js HTTP server provides static file serving capabilities with CORS headers and cache prevention. The server handles multiple file types including HTML, CSS, JavaScript, and various image formats, making it suitable for fragment development and testing.

### Styling Approach
The application uses vanilla CSS with modern features including CSS Grid, Flexbox, and CSS custom properties. Each fragment maintains its own styling in isolated CSS files, preventing style conflicts while ensuring consistent branding through shared color schemes and typography.

## External Dependencies

### Liferay DXP Integration
- **liferay-fragments-toolkit**: Development dependency used across all fragments for Liferay DXP integration and deployment
- Fragment structure follows Liferay DXP standards for seamless deployment to Liferay environments
- **Headless Admin User API**: Agent lookup widget integrates with Liferay's headless API for real-time user search

### Asset Management
- **Image Assets**: External image hosting through Liferay cloud infrastructure (webserver-lctfsidemocam-prd.lfr.cloud)
- Images include brand logos, icons, and marketing assets stored in Liferay's document library

### Runtime Environment
- **Node.js**: Minimal HTTP server for local development and preview
- No external databases or complex backend services required
- Static file serving with MIME type support for web assets

### Development Tools
- Standard web technologies (HTML5, CSS3, vanilla JavaScript)
- No frontend frameworks or build tools beyond the Liferay fragments toolkit
- Simple package.json structure for each fragment component
- Modern browser APIs (Fetch, AbortController) for API integration with race condition prevention