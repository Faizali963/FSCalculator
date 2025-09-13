# Calculator.net Design Guidelines

## Design Approach
**System-Based Approach**: Following Material Design principles for the clean, functional interface that prioritizes usability and information density. The site is utility-focused with extensive navigation and data entry requirements.

## Core Design Elements

### Color Palette
**Light Mode:**
- Primary: 220 25% 15% (deep blue-gray for headers)
- Background: 0 0% 98% (off-white)
- Surface: 0 0% 100% (pure white cards)
- Text: 220 15% 20% (dark gray)
- Accent: 210 100% 50% (bright blue for CTAs)

**Dark Mode:**
- Primary: 220 15% 85% (light blue-gray)
- Background: 220 15% 8% (very dark blue-gray)
- Surface: 220 10% 12% (dark cards)
- Text: 220 10% 90% (light gray)
- Accent: 210 80% 60% (softer blue)

### Typography
- **Headers**: Inter, 600-700 weight
- **Body**: Inter, 400-500 weight
- **Calculator Display**: JetBrains Mono, 500 weight
- **Sizes**: Text-sm to text-xl range

### Layout System
**Spacing**: Tailwind units of 2, 4, 6, and 8 (p-4, m-6, gap-8, etc.)
- Consistent 4-unit padding for cards
- 6-unit gaps between sections
- 8-unit margins for major layout divisions

### Component Library

**Scientific Calculator:**
- Grid-based button layout with larger display area
- Button variants: primary (operators), secondary (numbers), accent (functions)
- Monospace font for display with right alignment
- Clear visual hierarchy between basic and advanced functions

**Category Cards:**
- Clean card design with subtle shadows
- Consistent 16:9 aspect ratio for category images
- Hover states with gentle elevation increase
- Grid layout: 2 columns mobile, 4 columns desktop

**Navigation:**
- Simple header with logo and search
- Breadcrumb navigation for calculator pages
- Sidebar navigation for calculator categories (desktop)
- Mobile hamburger menu

**Calculator Forms:**
- Grouped input sections with clear labels
- Consistent form styling across all calculators
- Results displayed in highlighted cards
- Clear "Calculate" buttons with loading states

**Data Display:**
- Tables for amortization schedules and detailed breakdowns
- Charts for visual data representation (loan progress, BMI ranges)
- Summary cards for key results

## Images
**Category Images:** Each calculator category needs a representative image (financial charts, fitness icons, math symbols, utility tools). These should be clean, modern illustrations or photos with consistent styling and color treatment.

**No Hero Image:** The site focuses on immediate utility access rather than marketing appeal.

## Key Design Principles
1. **Clarity Over Style**: Function trumps form - every element serves a clear purpose
2. **Consistent Interactions**: Standardized button styles, form patterns, and navigation
3. **Efficient Scanning**: Clear visual hierarchy helps users quickly find their needed calculator
4. **Trust Through Simplicity**: Clean, professional appearance builds confidence in calculations
5. **Mobile-First**: Responsive design ensuring full functionality on all devices