# Component Documentation

## Button Components

### Primary Button
```css
Background: #1e3a5f (Primary/800)
Color: #ffffff
Border-radius: 8px
Padding: 12px 24px
Font: Inter, 16px, Medium (500)
Hover: Background #364a5f
```

### Secondary Button
```css
Background: transparent
Color: #1e3a5f
Border: 2px solid #1e3a5f
Border-radius: 8px
Padding: 10px 22px
Hover: Background #1e3a5f, Color #ffffff
```

### Accent Button
```css
Background: #d4af37 (Accent/500)
Color: #ffffff
Border-radius: 8px
Padding: 12px 24px
Hover: Background #b39430
```

### Button Sizes
- **XS**: Padding 6px 12px, Font 12px
- **SM**: Padding 8px 16px, Font 14px
- **MD**: Padding 12px 24px, Font 16px (default)
- **LG**: Padding 16px 32px, Font 16px
- **XL**: Padding 20px 40px, Font 18px

---

## Form Components

### Text Input
```css
Background: #ffffff
Border: 1px solid #ced4da
Border-radius: 8px
Padding: 12px 16px
Font: Inter, 16px
Focus: Border #1e3a5f, Box-shadow 0 0 0 3px rgba(30,58,95,0.1)
Error: Border #f44336
```

### Select
```css
Same as Text Input
Arrow icon on right side
```

### Textarea
```css
Same as Text Input
Min-height: 120px
Resize: vertical
```

### Toggle Switch
```css
Width: 48px
Height: 24px
Background: #ced4da (off) / #1e3a5f (on)
Thumb: 18px circle, white
Border-radius: Full (9999px)
```

### Checkbox
```css
Size: 20px
Border: 2px solid #ced4da
Border-radius: 4px
Checked: Background #1e3a5f, Checkmark white
```

---

## Card Components

### Default Card
```css
Background: #ffffff
Border: 1px solid #e9ecef
Border-radius: 12px
Padding: 24px
```

### Elevated Card
```css
Same as Default
Box-shadow: 0 4px 6px rgba(0,0,0,0.1)
```

### Stat Card
```css
Icon: 48x48px, 12px radius, colored background
Value: 30px, Bold
Label: 14px, Neutral/500
Change: 14px, colored text with arrow
```

### Room Card
```css
Left border: 4px, status color
Room number: 18px Bold
Type: 12px Neutral/500
Guest info section with avatar
```

---

## Navigation Components

### Sidebar
```css
Width: 280px
Height: 100vh
Background: #1e3a5f
Position: Fixed left
```

### Sidebar Item
```css
Padding: 12px 24px
Margin: 4px 12px
Border-radius: 8px
Color: rgba(255,255,255,0.7)
Hover: Background rgba(255,255,255,0.1)
Active: Background #d4af37, Color #ffffff
```

### Topbar
```css
Height: 64px
Background: #ffffff
Border-bottom: 1px solid #e9ecef
Position: Sticky top
```

### Tabs
```css
Border-bottom: 1px solid #e9ecef
Tab Padding: 16px 24px
Active: Color #1e3a5f, Border-bottom 2px #1e3a5f
```

---

## Badge Components

### Status Badges
```css
Padding: 4px 10px
Border-radius: 9999px
Font: 12px, Medium

Success: Background rgba(76,175,80,0.15), Color #4caf50
Warning: Background rgba(255,193,7,0.15), Color #b8860b
Error: Background rgba(244,67,54,0.15), Color #f44336
Info: Background rgba(33,150,243,0.15), Color #2196f3
Neutral: Background #e9ecef, Color #495057
```

### Room Status Badges
```css
Available: Green (#4caf50)
Occupied: Blue (#2196f3)
Reserved: Purple (#9c27b0)
Due Checkout: Orange (#ff9800)
Cleaning: Yellow (#ffc107)
Maintenance: Red (#f44336)
```

---

## Avatar Components

### Sizes
- **XS**: 24px
- **SM**: 32px
- **MD**: 40px (default)
- **LG**: 48px
- **XL**: 64px
- **2XL**: 96px

### Style
```css
Border-radius: 50%
Object-fit: cover
Fallback: Initials on colored background
```

### Avatar Group
```css
Overlap: -8px margin-left
Border: 2px solid white
```

---

## Modal Components

### Modal Container
```css
Background: #ffffff
Border-radius: 16px
Box-shadow: 0 25px 50px rgba(0,0,0,0.25)
Max-width: 560px (default), 800px (lg), 1140px (xl)
```

### Modal Header
```css
Padding: 24px
Border-bottom: 1px solid #e9ecef
Title: 18px Semibold
Close button: 32x32px
```

### Modal Body
```css
Padding: 24px
Overflow-y: auto
```

### Modal Footer
```css
Padding: 16px 24px
Background: #f8f9fa
Border-top: 1px solid #e9ecef
Buttons aligned right
```

---

## Table Components

### Table Container
```css
Border: 1px solid #e9ecef
Border-radius: 12px
Overflow: hidden
```

### Table Header
```css
Background: #f8f9fa
Padding: 16px 24px
Font: 13px Semibold, Neutral/600
Border-bottom: 1px solid #e9ecef
```

### Table Row
```css
Padding: 16px 24px
Border-bottom: 1px solid #f1f3f5
Hover: Background #f8f9fa
```

---

## Alert Components

### Alert Container
```css
Display: flex
Padding: 16px
Border-radius: 12px
Border: 1px solid
Gap: 12px
```

### Alert Types
```css
Info: Background #e3f2fd, Border #bbdefb, Color #0d47a1
Success: Background #e8f5e9, Border #c8e6c9, Color #1b5e20
Warning: Background #fff8e1, Border #ffecb3, Color #ff6f00
Error: Background #ffebee, Border #ffcdd2, Color #b71c1c
```

---

## Progress Components

### Progress Bar
```css
Height: 8px
Background: #e9ecef
Border-radius: 9999px
Fill: Various colors based on type
```

### Circular Progress (Occupancy Ring)
```css
SVG-based
Stroke-width: 12
Background circle: #e9ecef
Progress circle: Primary or Accent color
Center text for percentage
```

---

## Spacing System

```css
--space-1: 4px
--space-2: 8px
--space-3: 12px
--space-4: 16px
--space-5: 20px
--space-6: 24px
--space-8: 32px
--space-10: 40px
--space-12: 48px
--space-16: 64px
```

## Border Radius

```css
--radius-sm: 4px
--radius-base: 8px
--radius-lg: 12px
--radius-xl: 16px
--radius-2xl: 24px
--radius-full: 9999px
```
