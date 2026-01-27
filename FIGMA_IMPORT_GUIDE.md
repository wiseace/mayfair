# Figma Import Guide - Mayfair Hotel Management System

This guide explains how to import and edit the Hotel Management System designs in Figma.

## 📋 Overview

The Mayfair Hotel Management System includes **10+ complete screens** designed with a consistent design system. All designs are provided as HTML/CSS files that can be converted to Figma using multiple methods.

## 🚀 Import Methods

### Method 1: HTML to Figma Plugin (Recommended)

1. **Install the Plugin**
   - Open Figma → Plugins → Browse plugins
   - Search for "html.to" or "HTML to Figma"
   - Install the plugin

2. **Import Screens**
   - Open each HTML file in a web browser
   - Run the plugin in Figma
   - Paste the URL or HTML content
   - The plugin will convert the design to Figma layers

### Method 2: Screenshot + Auto Layout

1. Open each HTML screen in a browser at the correct dimensions
2. Take high-quality screenshots
3. Use Figma's "Paste to replace" or trace over with shapes
4. Apply Auto Layout to recreate responsive behavior

### Method 3: Manual Recreation (Best for Customization)

1. Use the design tokens from `design-system/tokens.css`
2. Set up Figma styles matching the CSS variables
3. Build components using the component styles
4. Assemble screens from the component library

## 🎨 Design System Setup in Figma

### Step 1: Create Color Styles

Create the following color styles in Figma:

```
Primary Colors:
- Primary/50: #f0f4f8
- Primary/100: #d9e2ec
- Primary/200: #bcccdc
- Primary/300: #9fb3c8
- Primary/400: #829ab1
- Primary/500: #627d98
- Primary/600: #4a6378
- Primary/700: #364a5f
- Primary/800: #1e3a5f (Main Primary)
- Primary/900: #0f1e2e

Accent Colors (Gold):
- Accent/500: #d4af37 (Main Accent)
- Accent/100: #fdeeb8
- Accent/600: #b39430

Neutral Colors:
- Neutral/0: #ffffff
- Neutral/50: #f8f9fa
- Neutral/100: #f1f3f5
- Neutral/200: #e9ecef
- Neutral/300: #dee2e6
- Neutral/400: #ced4da
- Neutral/500: #adb5bd
- Neutral/600: #6c757d
- Neutral/700: #495057
- Neutral/800: #343a40
- Neutral/900: #212529

Status Colors:
- Success/500: #4caf50
- Warning/500: #ffc107
- Error/500: #f44336
- Info/500: #2196f3

Room Status:
- Room/Available: #4caf50
- Room/Occupied: #2196f3
- Room/Reserved: #9c27b0
- Room/Checkout: #ff9800
- Room/Cleaning: #ffc107
- Room/Maintenance: #f44336
```

### Step 2: Create Text Styles

```
Headings:
- Heading/H1: Inter, 36px, Bold (700)
- Heading/H2: Inter, 24px, Bold (700)
- Heading/H3: Inter, 20px, Semibold (600)
- Heading/H4: Inter, 18px, Semibold (600)
- Heading/H5: Inter, 16px, Semibold (600)

Body:
- Body/Large: Inter, 18px, Regular (400)
- Body/Base: Inter, 16px, Regular (400)
- Body/Small: Inter, 14px, Regular (400)
- Body/XSmall: Inter, 12px, Regular (400)

Labels:
- Label/Medium: Inter, 14px, Medium (500)
- Label/Small: Inter, 12px, Medium (500)
```

### Step 3: Create Effect Styles

```
Shadows:
- Shadow/SM: 0px 1px 2px rgba(0,0,0,0.05)
- Shadow/MD: 0px 4px 6px rgba(0,0,0,0.1)
- Shadow/LG: 0px 10px 15px rgba(0,0,0,0.1)
- Shadow/XL: 0px 20px 25px rgba(0,0,0,0.1)
```

## 📐 Component Library

### Core Components to Create

#### 1. Buttons
- **Primary Button**: Primary/800 background, white text, 8px radius
- **Secondary Button**: Transparent, Primary/800 border and text
- **Accent Button**: Accent/500 background, white text
- **Ghost Button**: Transparent, neutral text
- **Danger Button**: Error/500 background, white text

#### 2. Form Inputs
- **Text Input**: White background, Neutral/300 border, 8px radius
- **Select**: Same as input with dropdown icon
- **Textarea**: Multi-line input
- **Checkbox/Radio**: 20px size, Primary/800 accent
- **Toggle Switch**: 48x24px, rounded pill

#### 3. Cards
- **Default Card**: White, Neutral/200 border, 12px radius
- **Stat Card**: With icon, value, label, change indicator
- **Room Card**: With status indicator stripe

#### 4. Badges/Tags
- **Status Badges**: Success, Warning, Error, Info variants
- **Room Status**: Available, Occupied, Reserved, etc.

#### 5. Navigation
- **Sidebar**: 280px width, Primary/800 background
- **Sidebar Item**: With icon, text, optional badge
- **Topbar**: 64px height, white background
- **Tabs**: Horizontal tab navigation

#### 6. Data Display
- **Table**: With header, rows, hover states
- **Avatar**: Circular, multiple sizes (24-96px)
- **Progress Bar**: Horizontal with fill

## 📱 Screen Specifications

| Screen | Desktop Size | Mobile Size |
|--------|-------------|-------------|
| Login | 1440 x 900 | - |
| Dashboard | 1440 x 900 | 375 x 812 |
| Reservations | 1440 x 900 | - |
| Room Management | 1440 x 900 | - |
| Guest Profile | 1440 x 900 | - |
| Housekeeping | 1440 x 900 | - |
| Billing | 1440 x 900 | - |
| Reports | 1440 x 900 | - |
| Settings | 1440 x 900 | - |
| Mobile Dashboard | - | 375 x 812 |

## 🔧 Customization Guide

### Changing Brand Colors

1. Update Primary/800 to your brand's main color
2. Update Accent/500 to your secondary/highlight color
3. Regenerate lighter shades using a color tool
4. Update all button and component styles

### Adding New Screens

1. Duplicate an existing screen as a template
2. Use components from the library
3. Follow the 8px spacing grid
4. Maintain consistent padding (24px for content areas)

### Creating Variants

1. Select a component
2. Create variants for: Default, Hover, Active, Disabled
3. Use Figma's interactive components for prototyping

## 📁 File Structure

```
Mayfair Hotel System/
├── README.md
├── FIGMA_IMPORT_GUIDE.md
├── design-system/
│   ├── tokens.css          # Design tokens (colors, spacing, etc.)
│   ├── components.css      # Component styles
│   └── utilities.css       # Utility classes
└── screens/
    ├── 01-login.html           # Authentication
    ├── 02-dashboard.html       # Main dashboard
    ├── 03-reservations.html    # Booking management
    ├── 04-rooms.html           # Room status board
    ├── 05-guests.html          # Guest profiles
    ├── 06-housekeeping.html    # Housekeeping kanban
    ├── 07-billing.html         # Invoice & payments
    ├── 08-reports.html         # Analytics
    ├── 09-mobile-dashboard.html # Mobile app
    └── 10-settings.html        # System settings
```

## 🎯 Best Practices

1. **Use Auto Layout** - All containers should use Auto Layout for responsiveness
2. **Component-First** - Build from components, not individual shapes
3. **Consistent Spacing** - Use 4px/8px grid for all spacing
4. **Name Layers** - Use clear, descriptive names for all layers
5. **Organize Pages** - Separate screens, components, and documentation

## 📞 Support

For questions about the design system or customization:
- Review the CSS files for exact values
- Check component styles for implementation details
- All colors and measurements are documented in tokens.css

---

*This design system is built for scalability and ease of customization. Start with the core components and expand as needed for your specific hotel management requirements.*
