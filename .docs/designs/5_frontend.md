[<< Back](./../design.md)

# Frontend Design Specification

## Overview
This document captures the complete frontend application specification, design system, and architecture. It serves as the single source of truth for all UI/UX decisions and implementation details. This specification ensures the frontend is not just functional, but truly beautiful and modern.

## 🎨 Visual Inspiration & Design Direction

### Design References
- **Primary Inspiration**: `[LINKS_TO_SPECIFIC_APPS/WEBSITES]`
- **Secondary References**: `[ADDITIONAL_INSPIRATION_SOURCES]`
- **Target Aesthetic**: `[MODERN_MINIMALIST/RICH_DETAILED/CREATIVE_BOLD/ENTERPRISE_PROFESSIONAL/ETC]`

### Design Philosophy
- **Core Principle**: `[BEAUTY_THROUGH_SIMPLICITY/SOPHISTICATED_DETAIL/BOLD_CREATIVITY/ETC]`
- **User Experience Goals**: `[INTUITIVE_NAVIGATION/DELIGHTFUL_INTERACTIONS/EFFICIENT_WORKFLOWS/ETC]`
- **Brand Personality**: `[TRUSTWORTHY/INNOVATIVE/PLAYFUL/PROFESSIONAL/ETC]`

## Design System

### Color Palette
**Primary Colors** (Based on inspiration/brand):
- Primary: `#[HEX_CODE]` - Main brand color for CTAs and primary actions
- Primary Light: `#[HEX_CODE]` - Hover states and backgrounds
- Primary Dark: `#[HEX_CODE]` - Active states and emphasis
- Secondary: `#[HEX_CODE]` - Accent color for highlights and secondary actions
- Tertiary: `#[HEX_CODE]` - Supporting color for variety and interest

**Neutral Palette** (Modern, sophisticated neutrals):
- White: `#FFFFFF` - Pure white for backgrounds
- Gray 50: `#[HEX_CODE]` - Lightest gray for subtle backgrounds
- Gray 100: `#[HEX_CODE]` - Very light gray for disabled states
- Gray 200: `#[HEX_CODE]` - Light gray for borders
- Gray 300: `#[HEX_CODE]` - Medium-light gray for secondary text
- Gray 400: `#[HEX_CODE]` - Medium gray for placeholders
- Gray 500: `#[HEX_CODE]` - True gray for secondary text
- Gray 600: `#[HEX_CODE]` - Dark gray for primary text
- Gray 700: `#[HEX_CODE]` - Very dark gray for headings
- Gray 800: `#[HEX_CODE]` - Almost black for emphasis
- Gray 900: `#[HEX_CODE]` - Pure black for maximum contrast

**Semantic Colors** (Modern, accessible):
- Success: `#10B981` - Green for success states
- Success Light: `#D1FAE5` - Light green for success backgrounds
- Warning: `#F59E0B` - Amber for warning states  
- Warning Light: `#FEF3C7` - Light amber for warning backgrounds
- Error: `#EF4444` - Red for error states
- Error Light: `#FEE2E2` - Light red for error backgrounds
- Info: `#3B82F6` - Blue for informational states
- Info Light: `#DBEAFE` - Light blue for info backgrounds

### Typography (Modern, Readable, Beautiful)
**Font Families**:
- Primary: `[MODERN_FONT]` (e.g., Inter, SF Pro, Roboto) - For UI elements and body text
- Display: `[DISPLAY_FONT]` (e.g., Outfit, Manrope, Poppins) - For headings and marketing copy
- Monospace: `[MONO_FONT]` (e.g., JetBrains Mono, Fira Code) - For code and technical content

**Type Scale** (Harmonious, modern proportions):
- Display XL: `48px` / `600` / `1.1` (Hero headings)
- Display L: `36px` / `600` / `1.2` (Page titles)
- Display M: `30px` / `600` / `1.2` (Section titles)
- Heading XL: `24px` / `600` / `1.3` (Major headings)
- Heading L: `20px` / `600` / `1.3` (Sub-headings)
- Heading M: `18px` / `600` / `1.4` (Component titles)
- Heading S: `16px` / `600` / `1.4` (Small headings)
- Body L: `18px` / `400` / `1.6` (Large body text)
- Body M: `16px` / `400` / `1.6` (Default body text)
- Body S: `14px` / `400` / `1.5` (Small body text)
- Caption: `12px` / `400` / `1.4` (Captions and labels)
- Label: `14px` / `500` / `1.4` (Form labels and UI labels)

### Spacing System (8pt Grid for Perfect Alignment)
**Base Unit**: `8px` (All spacing is multiples of 8px for visual harmony)
**Scale**: 
- XS: `4px` (0.5 units) - Tight spacing within components
- S: `8px` (1 unit) - Default component padding
- M: `16px` (2 units) - Standard spacing between elements
- L: `24px` (3 units) - Larger spacing between sections
- XL: `32px` (4 units) - Major section spacing
- 2XL: `48px` (6 units) - Large layout spacing
- 3XL: `64px` (8 units) - Page-level spacing
- 4XL: `96px` (12 units) - Hero section spacing

**Component-Specific Spacing**:
- Button Padding: `12px 24px` (S + M)
- Card Padding: `24px` (L)
- Form Field Spacing: `16px` (M)
- Section Spacing: `48px` (2XL)

### Modern Shadows & Elevation System
**Shadow Levels** (Subtle, layered depth):
- Level 0: `none` (Flat elements)
- Level 1: `0 1px 2px 0 rgba(0, 0, 0, 0.05)` (Subtle lift)
- Level 2: `0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0.06)` (Card level)
- Level 3: `0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06)` (Elevated elements)
- Level 4: `0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05)` (Modals)
- Level 5: `0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04)` (Floating panels)

### Border Radius (Soft, Modern Feel)
**Scale**:
- None: `0px` (Sharp edges for specific design needs)
- SM: `4px` (Small components like badges)
- DEFAULT: `8px` (Standard buttons and inputs)
- MD: `12px` (Cards and larger components)
- LG: `16px` (Large cards and sections)
- XL: `24px` (Hero sections and major components)
- FULL: `9999px` (Pills and circular elements)

## Modern Layout & Grid System

### Responsive Breakpoints (Mobile-First)
- **Mobile**: `0px` to `767px` (Mobile phones)
- **Tablet**: `768px` to `1023px` (Tablets and small laptops)
- **Desktop**: `1024px` to `1439px` (Standard desktop)
- **Large Desktop**: `1440px+` (Large monitors and widescreen)

### Container System (Centered, Responsive)
- **Max Width**: `1440px` (Large screens)
- **Container Padding**: 
  - Mobile: `16px` (Comfortable mobile margins)
  - Tablet: `24px` (More breathing room)
  - Desktop: `32px` (Desktop margins)
  - Large Desktop: `48px` (Wide screen margins)

### Grid System (CSS Grid/Flexbox Hybrid)
- **Grid Columns**: `12` columns (Flexible layout options)
- **Gutter Width**: `24px` (Consistent spacing)
- **Grid Type**: CSS Grid for page layout, Flexbox for components

## 🎨 Beautiful Component Specifications

### Navigation (Modern, Clean Header)
**Header/Navbar**:
- Height: `64px` (Standard comfortable height)
- Background: `White/Gray-50` with `border-bottom: 1px solid Gray-200`
- Logo: Left-aligned, `32px` height, `medium` font weight
- Navigation Items: 
  - Font: `Body M` with `500` weight
  - Color: `Gray-600` default, `Primary` active, `Gray-800` hover
  - Spacing: `32px` between items
  - Active indicator: `2px` bottom border in `Primary` color
- Mobile: Hamburger menu transforms to slide-out drawer
- Search: Integrated search bar (when needed) with `Level 1` shadow
- Profile: Avatar `32px` with dropdown menu
- CTA Button: Primary button style in top right

### Modern Button System
**Primary Button** (Main actions):
- Background: `Primary` color
- Text: `White` color, `Label` typography
- Border: `none`
- Padding: `12px 24px` (comfortable click target)
- Border Radius: `DEFAULT (8px)`
- Height: `44px` minimum (accessible touch target)
- Hover: `Primary-Dark` background, `Level 2` shadow
- Active: `Primary-Dark` background, `Level 1` shadow
- Disabled: `Gray-200` background, `Gray-400` text
- Focus: `2px` outline in `Primary` color with `2px` offset

**Secondary Button** (Secondary actions):
- Background: `White`
- Text: `Primary` color, `Label` typography
- Border: `1px solid Primary`
- Padding: `12px 24px`
- Hover: `Primary-Light` background, `Primary-Dark` text
- Focus: Same as primary button

**Ghost Button** (Tertiary actions):
- Background: `transparent`
- Text: `Gray-600` color, `Label` typography
- Border: `none`
- Padding: `12px 16px`
- Hover: `Gray-100` background, `Gray-800` text
- Border Radius: `DEFAULT (8px)`

### Beautiful Form Components
**Input Fields**:
- Height: `44px` (Accessible touch target)
- Padding: `12px 16px`
- Border: `1px solid Gray-300`
- Border Radius: `DEFAULT (8px)`
- Font: `Body M`
- Background: `White`
- Focus State: 
  - Border: `2px solid Primary`
  - Shadow: `0 0 0 3px Primary` with `0.1` opacity
- Error State:
  - Border: `2px solid Error`
  - Background: `Error-Light`
- Placeholder: `Gray-400` color
- Labels: `Label` typography, `Gray-700` color, `8px` margin-bottom

**Select Dropdowns**:
- Same styling as inputs
- Dropdown icon: `Gray-400` chevron-down
- Options: `White` background, `Gray-800` text
- Option hover: `Gray-50` background
- Option selected: `Primary-Light` background

### Card System (Elegant, Layered)
**Default Card**:
- Background: `White`
- Border: `none` (shadow provides definition)
- Border Radius: `MD (12px)`
- Padding: `24px` (L spacing)
- Shadow: `Level 2` (Card level)
- Hover State: `Level 3` shadow with smooth transition

**Elevated Card** (For important content):
- Same as default but with `Level 3` shadow
- Hover: `Level 4` shadow

**Flat Card** (For dense layouts):
- Border: `1px solid Gray-200`
- Shadow: `none`
- Hover: `Level 1` shadow

### Modal/Dialog System
**Modal Overlay**:
- Background: `rgba(0, 0, 0, 0.5)` (Semi-transparent backdrop)
- Backdrop blur: `4px` (Modern glass effect)

**Modal Container**:
- Background: `White`
- Border Radius: `LG (16px)`
- Shadow: `Level 5` (Maximum elevation)
- Max Width: `500px` (Comfortable reading width)
- Padding: `32px` (XL spacing)
- Animation: Scale in from `0.95` to `1.0` with opacity fade

### Data Display Components
**Tables**:
- Header: `Gray-50` background, `Label` typography, `Gray-700` text
- Rows: Alternating `White` and `Gray-25` backgrounds
- Cell Padding: `16px` vertical, `12px` horizontal
- Border: `1px solid Gray-200` between rows
- Hover: `Gray-50` background on row

**Status Badges**:
- Padding: `4px 12px`
- Border Radius: `FULL (9999px)`
- Font: `Caption` with `500` weight
- Success: `Success` background, `White` text
- Warning: `Warning` background, `White` text
- Error: `Error` background, `White` text
- Info: `Info` background, `White` text

## ✨ Modern Animations & Micro-interactions

### Timing & Easing (Smooth, Natural Feel)
**Transition Durations**:
- **Instant**: `0ms` (Immediate feedback)
- **Fast**: `150ms` (Quick hover states, small UI changes)
- **Medium**: `250ms` (Default for most interactions)
- **Slow**: `400ms` (Page transitions, complex animations)
- **Very Slow**: `600ms` (Special emphasis animations)

**Easing Functions** (Natural, physics-based):
- **Default**: `cubic-bezier(0.4, 0, 0.2, 1)` (Material Design standard)
- **Entrance**: `cubic-bezier(0, 0, 0.2, 1)` (Ease out - elements coming in)
- **Exit**: `cubic-bezier(0.4, 0, 1, 1)` (Ease in - elements going out)
- **Sharp**: `cubic-bezier(0.4, 0, 0.6, 1)` (Quick, snappy movements)
- **Bounce**: `cubic-bezier(0.68, -0.55, 0.265, 1.55)` (Playful bounce effect)

### Component Animations
**Button Interactions**:
- Hover: `transform: translateY(-1px)` + shadow increase over `150ms`
- Active: `transform: translateY(0px)` + shadow decrease over `100ms`
- Loading: Spinner or pulse animation
- Success: Brief scale animation `scale(1.05)` then back to `1.0`

**Card Animations**:
- Hover: `transform: translateY(-4px)` + shadow elevation over `250ms`
- Load-in: Fade in with `translateY(20px)` to `translateY(0)` over `400ms`
- Stagger: Cards animate in sequence with `100ms` delays

**Modal Animations**:
- Entrance: 
  - Backdrop: Fade in over `250ms`
  - Modal: Scale from `0.95` to `1.0` + fade in over `300ms`
- Exit: Reverse of entrance over `200ms`

**Page Transitions**:
- Route changes: Fade + slight slide (`translateX(20px)`) over `400ms`
- Loading states: Skeleton screens with subtle shimmer animations

### Micro-interactions (Delightful Details)
**Interactive Feedback**:
- **Form Focus**: Smooth border color transition + subtle scale of focus ring
- **Checkbox/Radio**: Checkmark draw-in animation over `200ms`
- **Toggle Switches**: Smooth slide animation with bounce easing
- **Dropdown Expand**: Height expansion with opacity fade-in
- **Progress Indicators**: Smooth bar fill or circular progress
- **Success Actions**: Subtle confetti or checkmark animation

**Hover States**:
- **Links**: Underline animation from left to right
- **Images**: Subtle scale (`scale(1.05)`) with overflow hidden
- **Icons**: Color transition + optional rotation/bounce
- **Navigation Items**: Background slide-in animation

### Loading & State Animations
**Loading States**:
- **Skeleton Screens**: Shimmer animation across placeholder content
- **Spinners**: Smooth rotation with appropriate sizing
- **Progress Bars**: Smooth fill animation with optional pulse
- **Lazy Loading**: Fade-in as content loads

**Data Animations**:
- **Chart Transitions**: Smooth data updates with eased transitions
- **Number Counters**: Count-up animations for statistics
- **Sort/Filter**: Smooth reordering with translate animations

## 📱 Modern Responsive Design

### Mobile-First Strategy
**Mobile Layout Patterns** (320px+):
- Single column layouts
- Collapsible navigation (hamburger menu)
- Touch-friendly 44px+ button heights
- Swipe gestures for carousels/navigation
- Bottom-aligned primary actions

**Tablet Adaptations** (768px+):
- Two-column layouts where appropriate
- Expanded navigation (visible menu items)
- Side-by-side forms
- Larger touch targets maintained

**Desktop Enhancements** (1024px+):
- Multi-column layouts (up to 3-4 columns)
- Hover states and micro-interactions
- Larger imagery and more whitespace
- Advanced navigation patterns
- Keyboard shortcuts and accessibility

### Touch & Interaction Targets
**Minimum Sizes** (Accessibility compliant):
- Touch targets: `44px × 44px` minimum
- Spacing between targets: `8px` minimum
- Text links: `44px` height clickable area
- Form inputs: `44px` height minimum

## ♿ Accessibility & Inclusion

### Color & Contrast (WCAG AA+)
**Contrast Ratios**:
- Normal text: `4.5:1` minimum (WCAG AA)
- Large text (18px+): `3:1` minimum
- UI components: `3:1` minimum
- Focus indicators: `3:1` minimum

**Color Independence**:
- Never rely solely on color to convey information
- Use icons, text, or patterns as alternatives
- Support colorblind users with distinct patterns

### Keyboard & Screen Reader Support
**Focus Management**:
- Visible focus indicators with `2px` outline + `2px` offset
- Logical tab order following content flow
- Focus trapping in modals and dropdowns
- Skip links for main content areas

**ARIA & Semantic HTML**:
- Proper heading hierarchy (h1 → h2 → h3)
- ARIA labels for icon buttons and complex components
- Live regions for dynamic content updates
- Semantic landmarks (nav, main, aside, footer)

**Screen Reader Optimization**:
- Descriptive alt text for images
- Form labels explicitly associated with inputs
- Error messages linked to form fields
- Loading states announced to screen readers

## 🚀 Modern Technology Stack

### Core Framework & Build Tools
**Frontend Framework**:
- **React**: `18.x` with TypeScript for type safety and modern hooks
- **Next.js**: `14.x` for SSR/SSG, routing, and performance optimization (when applicable)
- **Vite**: `5.x` for lightning-fast development and optimized builds

**Package Management**:
- **pnpm**: Preferred for faster installs and efficient disk usage
- **npm**: Alternative if team preference or constraints require it

### Styling & Design Implementation
**CSS Strategy**:
- **Tailwind CSS**: `3.x` for utility-first styling with custom design system
- **CSS Modules**: For component-specific styles when needed
- **PostCSS**: For CSS processing and autoprefixing

**Component Libraries** (Choose based on project needs):
- **Headless UI**: For accessible, unstyled components
- **Radix UI**: For complex, accessible components
- **Custom Components**: Built with design system specifications

### State Management & Data Fetching
**State Management**:
- **Zustand**: Lightweight, modern state management for simple-medium projects
- **Redux Toolkit**: For complex state management needs
- **React Context**: For simple shared state

**Data Fetching**:
- **TanStack Query**: For server state management and caching
- **SWR**: Alternative for data fetching
- **Axios**: For HTTP client with interceptors

### Additional Libraries
**UI Enhancement**:
- **React Hook Form**: For performant, flexible forms
- **Framer Motion**: For beautiful animations and page transitions
- **React Hot Toast**: For elegant notification system
- **React Icons**: Comprehensive icon library
- **Date-fns**: For date manipulation and formatting

**Charts & Visualization** (when needed):
- **Recharts**: For React-native charts
- **Chart.js**: For advanced charting needs
- **D3.js**: For custom data visualizations

## 📁 Modern File Structure

```
src/
├── app/                    # Next.js app directory (if using App Router)
│   ├── globals.css        # Global styles and Tailwind imports
│   ├── layout.tsx         # Root layout component
│   └── page.tsx           # Home page
├── components/
│   ├── ui/                # Base design system components
│   │   ├── Button.tsx     # Button variants
│   │   ├── Input.tsx      # Form inputs
│   │   ├── Card.tsx       # Card component
│   │   ├── Modal.tsx      # Modal/dialog system
│   │   └── index.ts       # Component exports
│   ├── forms/             # Form-specific components
│   │   ├── LoginForm.tsx
│   │   ├── ContactForm.tsx
│   │   └── index.ts
│   ├── layout/            # Layout components
│   │   ├── Header.tsx     # Main navigation
│   │   ├── Sidebar.tsx    # Side navigation
│   │   ├── Footer.tsx     # Footer component
│   │   └── index.ts
│   └── features/          # Feature-specific components
│       ├── dashboard/
│       ├── profile/
│       └── settings/
├── hooks/                 # Custom React hooks
│   ├── useAuth.ts        # Authentication logic
│   ├── useLocalStorage.ts
│   └── useDebounce.ts
├── lib/                   # Utility libraries and configurations
│   ├── auth.ts           # Authentication utilities
│   ├── api.ts            # API client setup
│   ├── utils.ts          # General utilities
│   └── validations.ts    # Form validation schemas
├── stores/               # State management
│   ├── authStore.ts     # Authentication state
│   ├── uiStore.ts       # UI state (modals, loading, etc.)
│   └── index.ts
├── styles/               # Styling files
│   ├── globals.css      # Global styles
│   ├── components.css   # Component-specific styles
│   └── tailwind.css     # Tailwind configuration
├── types/                # TypeScript type definitions
│   ├── auth.ts          # Authentication types
│   ├── api.ts           # API response types
│   └── global.ts        # Global type definitions
└── constants/            # Application constants
    ├── routes.ts        # Route definitions
    ├── api.ts           # API endpoints
    └── ui.ts            # UI constants (colors, sizes, etc.)
```

## 🎯 Implementation Best Practices

### Performance Optimization
**Bundle Optimization**:
- Code splitting at route and component levels
- Dynamic imports for heavy components
- Tree shaking for unused code elimination
- Asset optimization (images, fonts, CSS)

**Runtime Performance**:
- React.memo for expensive components
- useMemo and useCallback for expensive calculations
- Virtual scrolling for large data sets
- Image optimization with Next.js Image component

**Loading Strategies**:
- Skeleton screens for better perceived performance
- Progressive loading for images and content
- Lazy loading for below-the-fold content
- Service workers for caching (when appropriate)

### Developer Experience
**Type Safety**:
- Strict TypeScript configuration
- API response typing with Zod or similar
- Component prop interfaces
- Custom hook typing

**Code Quality**:
- ESLint with React and TypeScript rules
- Prettier for consistent formatting
- Husky for pre-commit hooks
- Conventional commits for better git history

### Testing Strategy
**Unit Testing**:
- **Vitest**: Fast unit testing framework
- **React Testing Library**: Component testing
- **MSW**: API mocking for tests

**Integration Testing**:
- **Playwright**: End-to-end testing
- **Storybook**: Component development and visual testing

## 🎨 Design System Implementation

### Tailwind Configuration
```javascript
// tailwind.config.js - Custom design system
module.exports = {
  content: ['./src/**/*.{js,ts,jsx,tsx}'],
  theme: {
    extend: {
      colors: {
        primary: {
          50: '#[PRIMARY_LIGHT]',
          500: '#[PRIMARY_BASE]',
          900: '#[PRIMARY_DARK]',
        },
        gray: {
          50: '#F9FAFB',
          100: '#F3F4F6',
          // ... rest of gray scale
        },
      },
      fontFamily: {
        sans: ['Inter', 'system-ui', 'sans-serif'],
        display: ['Outfit', 'system-ui', 'sans-serif'],
      },
      spacing: {
        '18': '4.5rem',
        '88': '22rem',
      },
      boxShadow: {
        'level-1': '0 1px 2px 0 rgba(0, 0, 0, 0.05)',
        'level-2': '0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0.06)',
        // ... rest of shadow levels
      },
    },
  },
  plugins: [
    require('@tailwindcss/forms'),
    require('@tailwindcss/typography'),
  ],
}
```

### Component Implementation Example
```typescript
// components/ui/Button.tsx - Type-safe, accessible button
interface ButtonProps extends React.ButtonHTMLAttributes<HTMLButtonElement> {
  variant?: 'primary' | 'secondary' | 'ghost'
  size?: 'sm' | 'md' | 'lg'
  loading?: boolean
  children: React.ReactNode
}

export const Button: React.FC<ButtonProps> = ({
  variant = 'primary',
  size = 'md',
  loading = false,
  children,
  className,
  disabled,
  ...props
}) => {
  const baseClasses = 'inline-flex items-center justify-center font-medium rounded-lg transition-all duration-150 focus:outline-none focus:ring-2 focus:ring-offset-2'
  
  const variantClasses = {
    primary: 'bg-primary-500 text-white hover:bg-primary-600 focus:ring-primary-500',
    secondary: 'bg-white text-primary-500 border border-primary-500 hover:bg-primary-50 focus:ring-primary-500',
    ghost: 'bg-transparent text-gray-600 hover:bg-gray-100 hover:text-gray-800 focus:ring-gray-500'
  }
  
  const sizeClasses = {
    sm: 'px-3 py-2 text-sm',
    md: 'px-6 py-3 text-base',
    lg: 'px-8 py-4 text-lg'
  }

  return (
    <button
      className={cn(
        baseClasses,
        variantClasses[variant],
        sizeClasses[size],
        (disabled || loading) && 'opacity-50 cursor-not-allowed',
        className
      )}
      disabled={disabled || loading}
      {...props}
    >
      {loading && <Spinner className="mr-2" />}
      {children}
    </button>
  )
}
```

## 📊 Success Metrics & Quality Gates

### Performance Targets
- **First Contentful Paint**: < 1.5s
- **Largest Contentful Paint**: < 2.5s
- **Cumulative Layout Shift**: < 0.1
- **First Input Delay**: < 100ms
- **Lighthouse Score**: 90+ for all categories

### Accessibility Goals
- **WCAG AA Compliance**: 100% for all interactive elements
- **Keyboard Navigation**: Full functionality without mouse
- **Screen Reader Support**: Comprehensive ARIA implementation
- **Color Contrast**: Minimum 4.5:1 for all text

---

**Note**: This comprehensive specification ensures the frontend will be not just functional, but truly beautiful, modern, and user-friendly. All placeholder values should be replaced with project-specific details during requirements gathering, with particular attention to the visual inspiration and design direction sections.

[<< Back](./../design.md)