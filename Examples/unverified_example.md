Create a single-file, responsive financial dashboard using Nextjs and TailwindCSS. This application should demonstrate a sophisticated "Neumorphic" (soft UI) design system.
Core Requirements:
Stateful Portfolio Overview: Display a main balance card that calculates a total from three different cryptocurrency accounts (BTC, ETH, and SOL).
Dynamic SVG Sparklines: Each asset row must include an inline SVG line chart representing a "7-day trend." These charts must be generated programmatically based on an array of mock price data in the state, not static images.
Interactive Transaction Form: Build a "Quick Transfer" component. It must include a segmented control (tab switcher) to toggle between "Send" and "Request" modes. The UI must visually update the button color and icon based on the active tab state.
Advanced Layout: Implement a two-column grid for desktop that collapses to a single column on mobile. Use CSS glassmorphism for a "Recent Activity" sidebar.
Micro-interactions: Buttons should have distinct :active states that simulate being "pressed" into the surface using inset box-shadows.
Technical Constraints:
All logic (React hooks), styles (Tailwind), and structure must be in one HTML file.
No external assets except for Lucide icons or Google Fonts.
The initial render must show the "BTC" row as 'selected' with a distinct highlighted border.
