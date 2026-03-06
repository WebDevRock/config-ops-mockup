# Configuration Ops - HTML Mockup

A modern, responsive HTML mockup for the Configuration Ops reactive application - a centralized configuration management system for OutSystems applications.

## Overview

This mockup demonstrates a hierarchical configuration management system that allows multiple OutSystems applications to share and manage configuration data.

## Features

### 🏗️ Hierarchical Structure
- **Applications** → Logical groupings (e.g., Customer Portal, Order Management)
- **Sections** → Categorized config groups (e.g., API Configuration, Security Settings)
- **Options** → Individual configuration entries with values and metadata

### ✨ Key Functionality

- **Configuration Management**
  - View, add, edit, and delete configuration options
  - Support for multiple data types (Text, Integer, Boolean, Secret, JSON, etc.)
  - Active/Inactive status toggles
  - Rich descriptions and friendly names

- **OutSystems App References**
  - Link multiple OutSystems applications to configuration groupings
  - Track which apps consume which configurations
  - Manage app GUIDs and descriptions

- **Search & Filter**
  - Filter by application
  - Search by option name, value, or description
  - Status filtering (Active/Inactive)

- **Visual Organization**
  - Color-coded sections for easy identification
  - Clean card-based layout
  - Responsive design for mobile and desktop

### 📊 Dashboard Statistics
- Total configuration options
- Number of sections
- Number of applications
- Supported data types

## Database Schema

Based on the OutSystems traditional web app structure:

- **ConfigApplication** - Application groupings
- **ConfigSection** - Configuration sections
- **ConfigOptions** - Individual configuration entries
- **ConfigDataTypes** - Available data types
- **ConfigApplicationMapping** - Many-to-many relationship between applications and OutSystems apps
- **ConfigSectionToRole** - Role-based access control

## Usage

Simply open `config-ops-mockup.html` in any modern web browser.

### Modal Interactions

1. **Add/Edit Configuration** - Click "New Config Option" or edit icons
2. **Manage OutSystems Apps** - Click "Manage OutSystems Apps" button on any application header
3. **Filter & Search** - Use toolbar filters to narrow down options

## Technology Stack

- Pure HTML5
- CSS3 with Flexbox and Grid
- Vanilla JavaScript (no frameworks)
- Fully responsive design

## Future Implementation

This mockup serves as a design reference for building the actual OutSystems reactive application with:
- Server-side data bindings
- Real CRUD operations
- Authentication and authorization
- Audit logging
- Role-based access control

## Project Structure

```
configOps/
├── config-ops-mockup.html   # Main HTML mockup file
├── IMG_4550.jpg              # Database schema reference image
└── README.md                 # This file
```

## Mock Data

The mockup includes sample data for:
- 3 Applications (Customer Portal, Order Management, Notification Service)
- 6 Sections (API Configuration, Security Settings, Feature Flags, etc.)
- 16+ Configuration options with various data types

## License

For internal use - OutSystems Configuration Management

---

**Created:** March 2026  
**Purpose:** Design reference for Configuration Ops reactive app migration
