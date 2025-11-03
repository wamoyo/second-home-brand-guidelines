# Second Home Vacation Rentals - Project Documentation

## Project Overview

**Client:** Second Home Vacation Rentals
**Website:** https://www.secondhomevacationrentals.com/
**Industry:** Vacation Rental Property Management
**Location:** Rocky Mountain region (Colorado) - Aspen, Fairplay, South Park

### Business Model
- **B2B2C Model**: Serve both property owners (B2B) and vacation renters (B2C)
- **Full-Service Management**: Handle everything from cleaning to marketing to maintenance
- **Local Focus**: Emphasize local, hands-on service vs. large national competitors

## Project Goals

### Phase 1: Brand Guidelines (COMPLETED)
Create comprehensive brand guidelines website documenting:
- Visual identity (colors, typography, logo)
- Design principles and patterns
- UI components and spacing systems
- Photography guidelines
- Tone of voice
- Do's and don'ts
- AI tools integration (markdown export, image prompts)

**Deliverable:** Single-page HTML brand guidelines with interactive features

### Phase 2: Revenue Estimator Tool (INPUT & OUTPUT MOCKUPS COMPLETE)
Build automated revenue estimation tool for prospective property owners to:
- Estimate earning potential based on property details
- Collect lead information (email, phone)
- Demonstrate Second Home's market expertise
- Replace manual estimation process
- Integrate with website

**Status:** Input form complete (slide-based chosen), 4 output mockup options complete
**Deliverable:** Slide-based form interface + 4 output design options + backend estimation system (pending)

---

## Completed Work

### 1. Revenue Estimator Options - Input Forms (4 Mockups Created)

**Decision:** Client selected **Slide-Based Estimator** as primary approach

#### Slide-Based Revenue Estimator (`slide-estimator.html`) - SELECTED ✓
**Status:** Input form complete, ready for output mockup

**Features:**
- **7 slides total:** Contact → Property Type → Location → Details → Quality → Amenities/Additional → Thank You
- **Progress bar:** 6 steps (excludes thank you page)
- **Mobile-optimized:** Minimal padding, clean spacing, readable progress steps
- **Half-star ratings:** Click left/right side of star for 0.5 increments (1.0 to 5.0)
- **Park County focus:** Autocomplete + interactive SVG map (Highway 9 corridor)
- **Quality assessment:** Star rating OR photo upload (3-10 images)
- **Privacy notice:** Clear statement about email usage on first slide
- **No SMS:** Client removed SMS opt-in (company no longer uses)

**Slide Details:**
1. **Contact Info** - Name, email, phone + privacy notice
2. **Property Type** - Visual cards (Cabin, House, Condo, Chalet, Townhome, Lodge)
3. **Location** - Single input with Park County autocomplete + clickable map
4. **Property Details** - Bedrooms, bathrooms, guest capacity, square footage
5. **Quality Assessment** - Star rating (with half-stars) OR photo upload
6. **Amenities & Additional** - Checkboxes for 12 amenities + free-text field
7. **Thank You** - Submission confirmation + company info

**Technical Implementation:**
- All JavaScript interactions work (star ratings, photo upload, map clicks, autocomplete)
- Form data collected client-side (ready for backend integration)
- Brand-compliant styling throughout
- Smooth animations and transitions

**Next Phase:** Design output/results page that will be emailed to property owners

#### Alternative Estimator Mockups (Demoted but Available)
- **Form-Based** (`revenue-estimator.html`) - Traditional multi-section form
- **Chat-Based** (`chat-estimator.html`) - Conversational interface
- **Interactive** (`interactive-estimator.html`) - Real-time calculator with sliders/toggles

All available via gray "Alternative" buttons on index.html

### 2. Revenue Estimator Output Designs (4 Mockups Created)

**Status:** All 4 output mockup options complete and available on brand guidelines page

Created 4 distinct output design approaches to display revenue estimates to property owners. Each design serves a different purpose and communication style. All use accurate Park County seasonality data.

#### Output Design 1: Minimalist Big Reveal (`output-minimalist.html`)
**Approach:** Clean, simple "big number" reveal with expandable details

**Features:**
- Large $87,500 annual revenue centered prominently
- Expandable details section (toggle to show/hide)
- Key sections when expanded:
  - Seasonal breakdown (Winter peak: $47.5K, Summer: $25K, etc.)
  - Key metrics (avg nightly rate, occupancy, revenue per bedroom)
  - Methodology transparency
  - Market comparison
- Dual CTAs in main white section: "List Your Property" (primary) + "Book A Meeting" (secondary)
- Mobile responsive with smooth transitions

**Best For:** Property owners who want quick answers with option for deeper detail

#### Output Design 2: Adjustable Interactive Calculator (`output-adjustable.html`)
**Approach:** Interactive "what-if" scenarios with real-time calculations

**Features:**
- Base estimate displayed prominently
- Quality rating slider (1.0 to 5.0 stars) to adjust rating
- Pet-friendly toggle (+15% revenue)
- 4 realistic amenity toggles:
  - Hot Tub (+12%)
  - WiFi (+5%)
  - Washer/Dryer (+6%)
  - Large Deck/Patio (+7%)
- Real-time revenue updates as user adjusts values
- Shows impact of each change clearly
- Helps owners understand what improvements matter most

**Technical:**
- JavaScript with compounding multiplier calculations
- Smooth animations on value changes
- Mobile-friendly touch interactions

**Best For:** Property owners considering improvements or wanting to explore scenarios

#### Output Design 3: Charts & Visuals Heavy (`output-charts.html`)
**Approach:** Data visualization focused with multiple chart types

**Features:**
- Monthly revenue bar chart (12 months with accurate seasonality)
  - Shows winter peak (Jan/Feb: $10.5K)
  - Shows mud season drop (May: $2K)
  - Summer secondary peak (Jul: $9.5K)
- Seasonal donut chart showing revenue distribution:
  - Winter: 54% ($47.5K)
  - Summer: 29% ($25K)
  - Fall: 10% ($8.5K)
  - Spring: 7% ($6.5K) - mud season
- Market comparison horizontal bars
- Occupancy rate line chart
- Key metrics cards (total revenue, avg rate, occupancy, revenue/bedroom)

**Technical:**
- CSS-based bar charts
- SVG line charts
- Color-coded by season
- Fully responsive

**Best For:** Data-driven property owners who want detailed visual breakdowns

#### Output Design 4: Comparable Properties Focus (`output-comps.html`)
**Approach:** Trust-building through real comparable property data

**Features:**
- Your property card (green highlight) with:
  - $87,500 estimate
  - Horizontal bar chart showing seasonal breakdown
  - Visual representation with dollar amounts and percentages
- 3 comparable properties with actual performance:
  - 192 Gold Trail: $94,250 (3BR/2BA)
  - 169 Puma Place: $82,100 (2BR/2BA)
  - 2735 CR 14: $89,350 (3BR/2.5BA)
- Detailed comparison table (12 data points):
  - Property details, amenities, rates, occupancy, annual revenue
- Historical 4-year performance chart
- Key insights section explaining the estimate

**Technical:**
- Horizontal bar charts with white bars on dark background
- Responsive table design
- Based on Second Home's actual comp PDF format

**Best For:** Property owners who want proof/validation through market comparables

#### Park County Seasonality Data (Used Across All Outputs)

Accurate seasonality reflecting Alma/Park County vacation rental patterns:

**Winter (Nov-Mar): 54% of revenue** - THE PEAK SEASON
- January: $10,500
- February: $10,500
- November: $7,000
- December: $10,000
- Skiing, snowmobiling, winter sports

**Summer (Jun-Aug): 29% of revenue** - Secondary peak
- July: $9,500
- August: $9,000
- June: $6,000
- Hiking, fishing, mountain activities

**Spring/Mud Season (Apr-May): 7% of revenue** - DEAD PERIOD
- May: $2,000 (lowest month)
- April: $4,500
- Ski resorts closed, trails muddy, minimal tourism

**Fall (Sep-Oct): 10% of revenue**
- September: $6,000
- October: $3,000
- Shoulder season before ski season

#### Output Design Technical Standards

**All outputs follow:**
- Brand colors (Sage Green #00BF8F, Russet Red #b3503e)
- Sharp corners (border-radius: 0)
- Arial typography with bold russet headings
- Mobile-responsive design
- CTAs in main content area (not separated footer-like sections)
- Accurate Park County seasonality throughout
- Professional yet approachable tone

**Links on Brand Guidelines Page:**
- Russet red button styling (#b3503e)
- Solid background with hover effects
- Grouped in dedicated section

### 3. Brand Guidelines Website (`index.html`)

**Features:**
- Single-page HTML with all CSS/JS inline (no external dependencies except Google Fonts)
- Fully responsive (mobile-first design)
- Interactive click-to-copy features
- Floating navigation menu
- Self-contained and deployable to GitHub Pages

**Sections:**
1. Hero (with logo and introduction)
2. Brand Overview
3. Color Palette (primary, neutrals, grays, utility, overlays)
4. Typography (Arial primary, Work Sans alternative)
5. Logo Usage (light/dark backgrounds)
6. UI Components (buttons, forms, spacing)
7. Photography Guidelines
8. Image Usage (inline images, overlays, specifications)
9. Design Principles
10. Tone of Voice
11. Do's & Don'ts
12. AI Tools & Export (markdown + image generation prompts)

**Interactive Features:**
- Click color swatches to copy hex codes
- Click-to-copy markdown guidelines (for AI tools)
- Click-to-copy AI image generation prompts (6 style-focused prompts)
- Floating navigation button (bottom-right) with dropdown menu
- Smooth scrolling to sections
- Centered "Copied!" overlay feedback

### 3. Key Decisions Made (Phase 2)

**Estimator Selection:**
- Created 4 different approaches for client review
- Client selected slide-based (one question at a time, progress bar)
- Demoted other 3 to "Alternative" options

**Input Form Decisions:**
1. **Privacy First:** Added clear privacy notice on first slide
2. **Local Focus:**
   - Park County-specific locations (Alma, Fairplay, Blue River, etc.)
   - Interactive Highway 9 corridor map
   - Only serves areas within Second Home's service region
3. **Quality Options:** Property owners choose star rating OR upload photos
4. **No SMS:** Removed SMS opt-in (company policy change)
5. **Combined Slides:** Merged amenities + additional info to reduce steps
6. **Simplified Progress:** 6-step progress bar (excludes thank you page)
7. **Mobile Optimization:** Removed unnecessary containers/padding

**Technical Approach:**
- Client-side form data collection
- Ready for backend integration
- Email-based delivery (no in-app results display)
- Thank you page after submission with company info

### 3. Supporting Documentation

**Files Created:**
- `README.md` - Comprehensive project documentation, GitHub Pages deployment instructions
- `.gitignore` - Clean repository setup
- `research.md` - Detailed brand research and analysis
- `colors-reference.txt` - Quick color palette reference
- `COMPARISON-CHECKLIST.md` - Verification checklist for brand accuracy
- `CLAUDE.md` - This file (project memory/documentation)

---

## Brand Standards

### Color Palette

**Primary Colors:**
- **Sage Green:** `#00BF8F` (RGB: 0, 191, 143)
  - Usage: Primary brand color, links, CTAs, accents, focus states
  - Represents: Nature, mountains, growth, tranquility

- **Russet Red:** `#b3503e` (RGB: 179, 80, 62)
  - Usage: ALL headings (h2, h3, h4), secondary buttons, warm accents
  - Weight: Bold (700) for all headings
  - Represents: Warmth, lodge/cabin aesthetic

**Neutral Colors:**
- **Charcoal:** `#333333` - Body text, headers
- **Near Black:** `#232323` - Text shadows
- **Black:** `#000000` - Footer, strong emphasis
- **White:** `#ffffff` - Backgrounds, text on dark

**Gray Scale:**
- **Light Gray:** `#f7f7f7` - Section backgrounds
- **Off-White Gray:** `#efefef` - Form backgrounds
- **Very Light Gray:** `#eeeeee` - Disabled states
- **Lighter Gray:** `#dddddd` - Button backgrounds
- **Medium Gray:** `#cccccc` - Borders, placeholders, form elements
- **Dark Gray:** `#999999` - Secondary text, footer

**Utility Colors:**
- **Orange:** `#ff9900` - Error messages and alerts

**Overlay Colors (for text over images):**
- `rgba(0, 0, 0, 0.2)` - 20% black for homepage header
- `rgba(0, 0, 0, 0.4)` - 40% black for search widgets
- `rgba(0, 0, 0, 0.5)` - 50% black for hero images
- `rgba(0, 0, 0, 0.65)` - 65% black for gradient overlays
- `rgba(0, 0, 0, 0.8)` - 80% black for fixed header when scrolled

### Typography

**Current Font Stack:**
```css
font-family: Arial, Helvetica, sans-serif;
```

**Alternative (in CSS but overridden):**
- Work Sans (Google Fonts) - Available for consideration
- Found in child.css but overridden by style.css

**Font Specifications:**
- **Section Headings (h2):** Arial Bold (700), 40px, #b3503e (Russet Red)
- **Subheadings (h3):** Arial Bold (700), 28px, #b3503e (Russet Red)
- **Sub-subheadings (h4):** Arial Bold (700), 20px, #333 (Charcoal)
- **Body Text:** Arial, 16px, weight 300 or normal, line-height 1.75, #333
- **Hero Titles:** Arial Light (300), 48px, #fff

**Important Note:**
- Work Sans is loaded from Google Fonts for comparison in guidelines
- Decision pending: Should brand fully switch to Work Sans for modern look?

### Logo Specifications

**Logo Files:**
- `logo-500.png` - Original full color (79KB)
- `logo-charcoal-500.png` - Charcoal (#333) for light backgrounds (12KB, optimized)
- `logo--black-500.png` - Pure black version (12KB)
- `favicon.jpg` - Website favicon

**Usage Rules:**
- **Light Backgrounds:** Use charcoal logo directly
- **Dark Backgrounds:** Use charcoal logo with CSS filter: `brightness(0) invert(1)`
- **Clear Space:** Minimum space equal to height of "S" in "Second"
- **Minimum Size:** 210px width mobile, 300px+ desktop
- **Maximum Size:** 500px for hero sections
- **Positioning:** Centered on hero/banners, left-aligned in navigation
- **Never:** Distort, rotate, change colors, add effects, place on busy backgrounds without overlay

### UI Components

**Buttons:**
- **Display:** `inline-block` (NOT full width unless in mobile forms)
- **Border Radius:** `0` (sharp corners - NEVER rounded)
- **Padding:** `12px 30px` (standard), `15px 40px` (hero CTAs)
- **Font:** Arial, 16-18px, weight 700
- **Transition:** `0.3s ease` on hover
- **Primary:** #00BF8F background → #00a077 on hover, white text
- **Secondary:** #b3503e background → #9a4434 on hover, white text
- **Outline:** Transparent background, #333 border (2px), inverts on hover

**Form Elements:**
- **Border:** `2px solid #ccc`
- **Border Radius:** `0` (sharp corners)
- **Focus State:** Border changes to `#00BF8F`
- **Padding:** `10px` (inputs), `12px` (larger forms)
- **Font:** Arial, Helvetica, sans-serif, 16px
- **Background:** White (#fff) or transparent on dark
- **Placeholder Color:** `#ccc`

**Spacing System:**
- **Section Padding:** 50px vertical
- **Container Max Width:** 1200px
- **Container Padding:** 20px horizontal
- **Element Margins:** 20px between major elements
- **Grid Gap:** 30px between grid items
- **Form Field Margin:** 20px to 30px bottom spacing

### Design Principles

1. **Sharp Corners:** `border-radius: 0` throughout - NEVER use rounded corners
2. **Mountain Aesthetic:** Natural color palette, landscape photography, earthy tones
3. **Modern & Clean:** Ample whitespace, clear hierarchy
4. **Professional Yet Welcoming:** Balance expertise with approachability
5. **Image-Forward:** Large, high-quality property and landscape photos
6. **Mobile-First:** Design for mobile, enhance for desktop
7. **Functional:** Clear CTAs, intuitive navigation, accessible

### Photography Guidelines

**Subject Matter:**
- Mountain landscapes and vistas
- Property exteriors with natural settings
- Interiors with natural light
- Outdoor activities (hiking, skiing)
- Families/groups enjoying properties
- Premium amenities (hot tubs, game rooms)

**Style:**
- Natural lighting preferred
- Warm, inviting color tones
- Wide shots showing context
- High resolution for web
- Authentic, not overly staged
- Showcase mountain environment

**Technical Requirements:**
- **Format:** JPEG for photos, PNG for transparency
- **Resolution:** 1920px wide minimum for heroes, 800px for content
- **Optimization:** Under 500KB per image
- **Aspect Ratios:** 16:9 for hero/banners, 4:3 or 3:2 for properties
- **Alt Text:** Always include for accessibility

**Overlay Best Practices:**
- Always use dark overlays when placing text over images
- Hero sections: 50% overlay standard
- Search widgets: 40% overlay
- Fixed headers (scrolled): 80% overlay
- Ensure white text has sufficient contrast

### Tone of Voice

**Brand Personality:**
- **Clear & Direct:** Straightforward communication
- **Informative:** Provide valuable local knowledge
- **Friendly:** Approachable without being casual
- **Confident:** Expert-driven but not boastful
- **Helpful:** Focus on solving customer needs

**Example Phrases:**
- "Vacation rentals offer travelers a unique lodging experience"
- "Seclusion and privacy with a home-like feel"
- "Almost every outdoor activity imaginable"
- "7 days a week support"

---

## Technical Patterns

### HTML/CSS/JS Standards

**Architecture:**
- Single-file HTML with inline CSS and JavaScript
- No external dependencies except Google Fonts (for font comparison)
- Vanilla JavaScript (no frameworks)
- Mobile-first responsive design
- Semantic HTML5

**CSS Patterns:**
```css
/* Sharp corners throughout */
border-radius: 0;

/* Brand color variables (conceptual - not using CSS vars) */
Primary: #00BF8F
Secondary: #b3503e
Text: #333
Background: #fff
Gray: #f7f7f7

/* Typography */
font-family: Arial, Helvetica, sans-serif;
font-size: 16px; /* base */
line-height: 1.75; /* body text */
font-weight: 700; /* all headings */
color: #b3503e; /* all h2, h3, h4 */

/* Spacing */
padding: 50px 0; /* sections */
margin-bottom: 20px; /* elements */
gap: 30px; /* grids */

/* Transitions */
transition: all 0.3s ease;
```

**JavaScript Patterns:**
- Use `var` for variable declarations (per user's coding standards)
- Use `function` keyword for functions (not arrow functions except single-line returns)
- Add space between function name and parenthesis: `function toggleNav ()`
- No semicolons at end of lines (only where syntactically required)
- querySelector/querySelectorAll for DOM selection
- addEventListener for event handling
- Pure functions where possible

**Responsive Breakpoints:**
```css
@media (max-width: 768px) {
    /* Mobile styles */
}
```

### Address Autocomplete & Map Pattern

**Address Autocomplete Implementation:**
```javascript
// Load 6,977 Park County addresses from JSON
fetch('./park-county-addresses.json')
  .then(response => response.json())
  .then(data => {
    addresses = data
    initializeAutocomplete()
  })

// Configure Fuse.js for fuzzy search
var fuse = new Fuse(addresses, {
  keys: [
    { name: 'address', weight: 2 },
    { name: 'street', weight: 1.5 },
    { name: 'number', weight: 1 },
    { name: 'city', weight: 1 }
  ],
  threshold: 0.4,
  minMatchCharLength: 2
})

// Search and display results
var results = fuse.search(query, { limit: 10 })
```

**Leaflet.js Map Integration:**
```javascript
// Initialize map only when slide 3 is shown (prevents sizing issues)
function initMap() {
  var breckenridgeCoords = [39.4817, -106.0384]
  map = L.map('propertyMap').setView(breckenridgeCoords, 11)

  // OpenStreetMap tiles (free, no ads)
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; OpenStreetMap contributors'
  }).addTo(map)
}

// Add custom sage green marker
var greenIcon = L.divIcon({
  className: 'custom-marker',
  iconSize: [20, 20],
  iconAnchor: [10, 10]
})

propertyMarker = L.marker([lat, lng], { icon: greenIcon }).addTo(map)
propertyMarker.bindPopup('<strong>Your Property</strong><br>' + address)
map.setView([lat, lng], 14, { animate: true })
```

**CSS for Map Integration:**
```css
/* High z-index for autocomplete above map */
.location-suggestions {
  z-index: 9999;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

/* Custom marker styling */
.custom-marker {
  background-color: #00BF8F;
  border-radius: 50%;
  border: 3px solid #fff;
  box-shadow: 0 2px 8px rgba(0,0,0,0.3);
}

/* Minimal map attribution */
.leaflet-control-attribution {
  font-size: 8px !important;
  opacity: 0.5;
}
```

### Interactive Features Pattern

**Click-to-Copy Implementation:**
```javascript
function showCopiedOverlay(containerId, textareaId) {
    var container = document.getElementById(containerId)
    var textarea = document.getElementById(textareaId)

    // Create centered overlay
    var overlay = document.createElement('div')
    overlay.style.position = 'absolute'
    overlay.style.top = '50%'
    overlay.style.left = '50%'
    overlay.style.transform = 'translate(-50%, -50%)'
    overlay.style.background = '#00BF8F'
    overlay.style.color = '#fff'
    overlay.style.padding = '15px 30px'
    overlay.style.fontSize = '18px'
    overlay.style.fontWeight = '700'
    overlay.style.borderRadius = '0'
    overlay.textContent = 'Copied!'

    container.appendChild(overlay)

    // Flash textarea border and background
    textarea.style.borderColor = '#00BF8F'
    textarea.style.background = '#f0fff0'

    // Remove after 1.5s
    setTimeout(function() {
        container.removeChild(overlay)
        textarea.style.borderColor = '#ccc'
        textarea.style.background = '#fff'
    }, 1500)
}
```

**Floating Navigation Pattern:**
- Fixed bottom-right position
- Dropdown opens upward
- Closes on outside click or link click
- Smooth scroll to sections
- Mobile responsive sizing

**Form Validation:**
- HTML5 required attributes
- Custom JavaScript validation as needed
- Focus state styling (#00BF8F border)
- Error messages in orange (#f90)

### File Upload Pattern
```javascript
// Drag-and-drop support
// File preview with remove capability
// Multiple file handling
// Image type validation
```

---

## File Structure

```
brand-guidelines/
├── index.html                      # Main brand guidelines page
│
├── slide-estimator.html            # Revenue estimator input (SELECTED)
├── revenue-estimator.html          # Alternative: form-based estimator
├── chat-estimator.html             # Alternative: chat-based estimator
├── interactive-estimator.html      # Alternative: interactive calculator
│
├── output-minimalist.html          # Output Option 1: Big reveal design
├── output-adjustable.html          # Output Option 2: Interactive calculator
├── output-charts.html              # Output Option 3: Charts & visuals heavy
├── output-comps.html               # Output Option 4: Comparable properties
│
├── park-county-addresses.json      # Address autocomplete data (6,977 addresses)
│
├── README.md                       # Project documentation
├── CLAUDE.md                       # This file - project memory
├── .gitignore                      # Git ignore rules
├── research.md                     # Detailed brand research
├── colors-reference.txt            # Quick color reference
├── COMPARISON-CHECKLIST.md         # Brand verification checklist
│
├── logo-500.png                    # Original full color logo (79KB)
├── logo-charcoal-500.png           # Charcoal logo for light BG (12KB) - PRIMARY
├── logo--black-500.png             # Pure black logo (12KB)
├── favicon.jpg                     # Website favicon (192x192)
│
├── photo1.jpg                      # Mountain landscape
├── photo2.jpg                      # Property exterior
├── photo3.jpg                      # Mountain property
├── photo4.jpg                      # Winter property
│
├── theme-style.css                 # Reference: main theme CSS (downloaded)
└── child-theme.css                 # Reference: child theme CSS (downloaded)
```

---

## Key Decisions & Changes Made

### Design Decisions

1. **No Navigation Bar Initially**
   - User feedback: Remove nav bar, they didn't want it
   - Solution: Added floating navigation button (bottom-right) later

2. **Logo Placement**
   - Moved from separate header to hero section
   - Max width: 500px at top of page
   - Inverted to white on dark backgrounds using CSS filter

3. **Heading Styles**
   - Initially: Light weight, sage green
   - **CORRECTED:** Bold (700), russet red (#b3503e)
   - User inspected actual website to verify
   - Applied to ALL h2, h3, h4 elements

4. **Border-Left Styling**
   - Initially used `border-left: 4px solid #00BF8F` on boxes
   - **REMOVED:** User feedback - not part of actual brand
   - Website never uses this pattern

5. **Button Width**
   - Initially unclear
   - **CLARIFIED:** Buttons are `inline-block`, NOT full width
   - Exception: Mobile forms may use full width

6. **Font Override Issue**
   - child.css declares Work Sans
   - style.css overrides with Arial
   - **Current State:** Arial is used
   - Added comparison section showing both options
   - Decision pending: Consider switching to Work Sans

7. **Logo Files**
   - User provided resized, optimized versions
   - logo-charcoal-500.png for light backgrounds (PRIMARY)
   - CSS filter for dark background inversion
   - Original logo kept for reference

8. **Spacing Examples**
   - Initially: 4 identical green boxes
   - **IMPROVED:** Varied examples (heading, text, image, button)
   - Uses real content and different colors

9. **AI Image Prompts**
   - Initially: Specified content and aspect ratios
   - **REVISED:** Style-focused only (lighting, color palette, mood)
   - User decides content and dimensions

10. **Copy Feedback Consistency**
    - Initially: Different feedback for markdown vs prompts
    - **UNIFIED:** Centered "Copied!" overlay for all click-to-copy features
    - Green border flash + light green background on textarea

11. **Section Alignment (AI Tools)**
    - Initially: Mixed left/center alignment
    - **FIXED:** All h3 section titles centered to match instructions

### Content Decisions

1. **Real Images from Website**
   - Downloaded 4 property/mountain photos
   - Used in spacing examples and image usage section
   - Demonstrates actual brand aesthetic

2. **Interactive Features Added**
   - Click color swatches to copy hex
   - Click textareas to copy (no separate buttons)
   - Floating navigation for section jumping
   - All with consistent visual feedback

3. **AI Tools Integration**
   - Full markdown export of guidelines
   - 6 AI image generation prompts (style-focused)
   - Both click-to-copy enabled
   - Helps users paste into ChatGPT, Claude, etc.

---

## Second Home Business Context

### Property Owner Value Propositions

**Key Differentiators:**
- Local, hands-on management vs. "big name" competitors
- 7 days a week staffed office
- Immediate problem resolution (local team)
- Full-service: cleaning, maintenance, marketing, financials

**Services Provided:**
1. **Rental Management:** Advertising, payments, check-in/out
2. **Marketing:** $20K+ annual spend, 15+ websites, radio/print
3. **Property Maintenance:** Weekly inspections, utilities, security
4. **Cleaning:** In-house team, full-time manager, 3-sheet linen system
5. **Guest Experience:** Welcome amenities (flowers, cookies, gifts)
6. **Financial Management:** Monthly statements/payments, tax filing, 1099s
7. **Owner Portal/App:** View bookings, finances, personal stays, photos

**Notably Absent:**
- NO pricing/fees disclosed publicly
- NO commission structure listed
- NO revenue estimates provided
- Suggests consultation-based sales approach
- **This is the gap we're filling with Revenue Estimator**

### Target Audiences

**Property Owners (B2B):**
- Homeowners in Rocky Mountain region
- Seeking professional management
- Value reliability, revenue generation, peace of mind
- Want technology-enabled tools

**Vacation Renters (B2C):**
- Families, groups, travelers
- Seeking authentic experiences
- Value privacy, amenities, location
- Budget-conscious to luxury

### Competitive Positioning
- Local accountability vs. phone-list service
- Quality control through inspections
- Consolidated services (saves owners money)
- Premium presentation
- Transparent reporting

---

## Next Steps: Revenue Estimator - Backend Development

### Current Status
✅ Slide-based input form completed (`slide-estimator.html`)
✅ All interactive features working (star ratings, photo upload)
✅ Address autocomplete with 6,977 Park County addresses
✅ Interactive Leaflet.js map with OpenStreetMap tiles
✅ Auto-zoom to selected property with custom markers
✅ Brand-compliant design and mobile-optimized
✅ Client approved approach
✅ 4 output design mockups completed (minimalist, adjustable, charts, comps)
✅ Accurate Park County seasonality data integrated
⏳ Backend implementation - FUTURE

### Recently Completed: Address Autocomplete & Interactive Map

**Address Autocomplete** ✅
- Implemented Fuse.js-powered fuzzy search
- 6,977 Park County addresses (ALMA, COMO, FAIRPLAY)
- Real-time search as user types (2+ characters)
- Dropdown shows up to 10 matching results
- Two-line display: address (bold) + city/zip (gray)
- Click to select and auto-populate coordinates
- High z-index (9999) to appear above map

**Interactive Map** ✅
- Leaflet.js with OpenStreetMap tiles (100% free, no ads)
- Centered on Breckenridge, CO at zoom level 11
- Shows Park County terrain and context
- Initializes only when user reaches slide 3 (prevents sizing issues)
- Custom sage green marker (#00BF8F) with white border
- Popup shows selected property address
- Auto-zoom to level 14 when address selected
- Minimized attribution (8px, 50% opacity)

**Integration:**
- Selecting address from autocomplete → marker appears on map
- Map pans and zooms to selected location
- Coordinates stored in `selectedAddress` variable for backend use

### Remaining Backend Work

**Backend Development Needed:**
1. **Data Collection & Storage**
   - Form submission endpoint
   - Database schema for submissions
   - File upload handling (photos to S3/cloud storage)
   - Lead capture system integration

2. **Revenue Estimation Engine**
   - Historical booking data analysis
   - Market rate comparison algorithm
   - Seasonal trend calculations
   - Property feature scoring (amenities impact)
   - Location-based pricing factors
   - Competitor analysis data

3. **AI/ML Components**
   - Photo quality assessment (using LLM vision API)
   - Property condition scoring
   - Comparable property matching
   - Dynamic pricing recommendations

4. **Email Delivery System**
   - Template design (brand-compliant)
   - Estimate report generation (PDF or HTML email)
   - 10-minute delivery timing
   - Personalization based on property details

5. **SMS Integration** (if opted in)
   - SMS service provider integration
   - Compliance with opt-in/opt-out regulations
   - Message templates

6. **CRM Integration**
   - Lead scoring
   - Follow-up automation
   - Owner portal account creation (optional)

7. **Analytics & Tracking**
   - Form submission tracking
   - Conversion metrics
   - Revenue estimate accuracy tracking
   - A/B testing capability

### Technical Architecture Recommendations

**Stack Suggestions:**
- **Frontend:** Already completed (vanilla HTML/CSS/JS)
- **Backend:** Node.js/Express or Python/Flask
- **Database:** PostgreSQL or MongoDB
- **File Storage:** AWS S3 or Cloudflare R2
- **Email:** SendGrid or AWS SES
- **SMS:** Twilio
- **AI/ML:** OpenAI GPT-4 Vision API for photo assessment
- **Hosting:** Vercel, Netlify, or AWS
- **Analytics:** Google Analytics + Mixpanel

**Data Sources Needed:**
1. Historical booking rates (from Second Home's systems)
2. Occupancy rates by season/property type
3. Market comparables (competitor pricing)
4. Amenity value multipliers
5. Location desirability scores

### Integration Points

**With Second Home's Existing Systems:**
- Owner Portal (ResortPro/Streamline VRS)
- CRM/Lead Management
- Property Management System
- Marketing automation
- Financial reporting

---

## Deployment Instructions

### GitHub Pages Deployment

```bash
# Initialize repository
cd "/path/to/brand-guidelines"
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Second Home brand guidelines and revenue estimator"

# Create main branch
git branch -M main

# Add remote
git remote add origin https://github.com/USERNAME/REPO.git

# Push
git push -u origin main
```

**Enable GitHub Pages:**
1. Repository Settings → Pages
2. Source: Deploy from branch
3. Branch: main, folder: / (root)
4. Save

**Live at:** `https://USERNAME.github.io/REPO/`

### Custom Domain (Optional)
1. Add CNAME file with domain
2. Configure DNS at domain registrar
3. Enable HTTPS in GitHub Pages settings

---

## Questions & Decisions Pending

### For Client Discussion

1. **Font Decision:**
   - Stick with Arial (current, universal)
   - Switch to Work Sans (modern, distinctive)
   - Impact: Would require updating actual website CSS

2. **Revenue Estimator Data Sources:**
   - What historical data is available?
   - Access to booking system?
   - API integration possibilities?
   - Manual data export acceptable?

3. **Lead Follow-up Process:**
   - Who receives notifications?
   - How quickly should someone follow up?
   - CRM integration requirements?
   - Automated nurture sequences?

4. **Estimate Accuracy Goals:**
   - How accurate should estimates be?
   - Legal disclaimers needed?
   - Show as ranges or specific numbers?
   - Include assumptions/methodology?

5. **SMS Compliance:**
   - Current SMS provider?
   - Opt-in/opt-out process?
   - Message frequency expectations?
   - Compliance with TCPA regulations?

6. **Photo Analysis:**
   - What quality factors matter most?
   - How to score property condition?
   - Impact on estimate calculation?
   - Feedback to property owner?

---

## Version History

**v2.0** (October 2024)
- Complete brand guidelines with verified colors
- Interactive features (click-to-copy, navigation)
- AI tools integration
- Revenue estimator form interface
- Full responsive design
- GitHub Pages deployment ready

**v1.0** (October 2024)
- Initial research and documentation
- Basic brand guidelines structure

---

## Contact & Resources

**Client Website:** https://www.secondhomevacationrentals.com/
**Phone:** (970) 546-7336
**Key Sections:**
- Home Owners: /home-owners/
- Why Choose Us: /home-owners/why-choose-us/
- Our Services: /home-owners/our-services/

**Project Repository:** TBD (to be deployed)
**Live Brand Guidelines:** TBD (after deployment)
**Live Revenue Estimator:** TBD (after backend development)

---

## Notes for Future Development

1. **Keep brand guidelines updated** as decisions are made (e.g., font choice)
2. **Test revenue estimator** form on mobile devices before launch
3. **Backend security:** Validate all inputs, sanitize uploads, rate limit submissions
4. **Photo storage:** Implement automatic cleanup of old uploaded photos
5. **GDPR/Privacy:** Add privacy policy link, data retention policy
6. **Analytics:** Track form abandonment, most common property types, conversion rates
7. **A/B Testing:** Test different CTAs, form lengths, estimate delivery times
8. **Integration:** Plan for eventual integration with Second Home's website
9. **Performance:** Optimize images, consider lazy loading for brand guidelines page
10. **Accessibility:** Run WCAG audit, ensure keyboard navigation, screen reader compatibility

---

**Last Updated:** November 3, 2024
**Status:**
- Phase 1 Complete: Brand Guidelines
- Phase 2 Input Form Complete: Slide-based estimator with autocomplete and map
- Phase 2 Output Mockups Complete: 4 design options
- Phase 2 Address System Complete: Autocomplete + interactive map
- Phase 2 Pending: Backend development and integration
