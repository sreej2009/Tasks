# Tasks

**Overview**

This project is an interactive pricing and bundle selection webpage built using HTML, CSS, and JavaScript.
It allows users to:

View multiple bundle plans (Starter, Premium Duo, and Elite Trio)

Expand and view details of each plan

Select options such as size and color

See the total price update dynamically

Switch between light and dark mode

**1. HTML Structure**

The HTML defines the layout of the page:

A main .container that holds all elements.

A heading, multiple plan cards, and a summary section.

Each plan includes:

A radio button for selection.

A title, short description, and discount badge.

An expandable body (.plan-body) that reveals details when opened.

Pricing information and dropdown selectors (for Premium Duo).

Each .plan has a data-price attribute so JavaScript can easily read and display the total price.

**2. CSS Styling**

The CSS provides a modern, premium look and handles both light and dark themes.

Key features:

Gradient background: smooth blend of purple and pink for premium feel.

Box shadows and rounded corners to create depth.

Hover effects: plans glow slightly when hovered.

Dark mode styles: activated by toggling the .dark class on the body.

Responsive design using @media (max-width: 480px) for mobile.

Badges like “10% OFF” and “MOST POPULAR” use custom shapes with small triangles for decoration.

**3. JavaScript Functionality**

The JavaScript makes the page interactive and dynamic.

Main features:

Plan Selection & Expansion:

When a plan is clicked, it expands to show details.

All other plans collapse.

The selected plan’s radio button is checked.

The total price updates automatically using the data-price attribute.

Prevent Dropdown Closing:

The <select> elements inside Premium Duo originally caused the plan to close when clicked.

This was fixed by using e.stopPropagation() to stop event bubbling.

Dark Mode Toggle:

A button (#toggleMode) switches between light and dark mode by toggling a class on the <body>.

The button text updates to show the current mode (🌞 Light / 🌙 Dark).


**4. Responsiveness**

The layout automatically adjusts for smaller screens:

The plan header rearranges vertically.

Font sizes and paddings scale down for better readability.

**5. Key Learnings / Concepts Used**

Event handling and propagation (stopPropagation()).

DOM selection and manipulation.

Data attributes (data-price) for dynamic updates.

Responsive design with media queries.

Theme switching using class toggles.

Smooth transitions with CSS animations.
