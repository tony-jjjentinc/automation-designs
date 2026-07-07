This repository will feature the following:
- comprehensive design rules to be followed
- design snippets

Design Rules:
1. Technologies: Dashboards and Portals are expected to be built and deployed as Web Applications via Google Apps Scripts. It is important to build pages strictly on a single html file
2. Styling Library - The project will use Bootstrap 5 as the styling library for the layout and interfaces of the project. It is important to use the bootstrap's CDN as web apps are deployed via a single HTML file
3. Optional Technologies: It is also an option to use React via CDN to handle component-based web applications

Repository will feature the following:
- Design templates for the Dashboards, Portals, Management Pages, etc. (Pages related to manage dashboards and portals)
- Design templates for the UI Components (Components related to manage dashboards and portals)




# General
- **Unified Ecosystem**: All dashboards and portals must be unified under a consistent design language to ensure seamless navigation for users across different tools.
- **User Experience (UX)**: Prioritize intuitive navigation, fast load times, and clear data presentation.
- **Accessibility**: Ensure high contrast ratios and proper labeling for all interactive elements to maintain accessibility standards.

# Technologies
- **Deployment Platform**: Dashboards and Portals are strictly built and deployed as Web Applications via Google Apps Scripts.
- **Single-File Architecture**: Pages MUST be built strictly as a single `.html` file. All CSS must be inside `<style>` tags and JavaScript inside `<script>` tags. No external local asset loading is allowed.
- **Styling Library**: Bootstrap 5 must be used via CDN for all layouts and interfaces.
- **Icons**: Utilize Font Awesome via CDN for consistent iconography across all projects.
- **Optional Advanced Framework**: React may be used via CDN (along with Babel standalone) to handle complex, component-based web applications, provided it still adheres to the single-file architecture constraint.

# Design
- **Premium Aesthetics**: Implement modern web design best practices. Interfaces should feel state-of-the-art and premium. Utilize smooth micro-animations, clean card layouts with subtle drop-shadows, and rounded corners (e.g., `border-radius: 8px` or `10px`).
- **Typography**: Rely on modern, clean sans-serif typography such as 'Inter', 'Roboto', 'Segoe UI', or system defaults. Avoid outdated browser default fonts.
- **Responsiveness**: All pages must be fully responsive, utilizing Bootstrap's grid system to ensure usability on mobile, tablet, and desktop devices.
- **Component Reusability**: Rely on standard Bootstrap 5 classes combined with the predefined snippets in `templates/components`. Avoid creating custom CSS for standard components when a Bootstrap utility exists.
- **Sub-Department Color Coding**: The organization utilizes different shades of blue to visually distinguish between the 6 sub-departments. The assigned color should be used as the primary accent color (headers, primary buttons, active links, and key icons) for that sub-department's pages:
  - **Sub-department 1 (Executive/Admin)**: Deep Navy Blue (`#0A2540`)
  - **Sub-department 2 (IT/Engineering)**: Royal Blue (`#1D4ED8`)
  - **Sub-department 3 (Human Resources)**: Cobalt Blue (`#0059B3`)
  - **Sub-department 4 (Sales/Marketing)**: Cerulean Blue (`#0284C7`)
  - **Sub-department 5 (Finance/Operations)**: Steel Blue (`#4682B4`)
  - **Sub-department 6 (Customer Support)**: Bright Sky Blue (`#38BDF8`)

# Setup
- **Templating**: When initiating a new project, always start by duplicating the relevant template from the `templates/pages/` directory (e.g., `dashboard.html`, `portal.html`, or `dashboard_react.html`).
- **Component Integration**: Copy necessary UI components from `templates/components/ui_components.html` to ensure visual consistency.
- **Color Customization**: Upon creating a new file from a template, immediately update the CSS root variables or primary inline styles to match the specific sub-department's blue shade.
