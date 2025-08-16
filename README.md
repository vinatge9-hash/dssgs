# Starlit Bistro — Reviews Website

A modern, interactive multi-page demo website showcasing a restaurant review experience. Built with Tailwind CSS utility classes (via CDN) and vanilla JavaScript for animations and interactions. The server is a simple Express static server for quick deployment.

Project structure

my-project/
├── public/
│   ├── index.html          # Main landing page with reviews, carousel, modal
│   ├── about.html          # About / team / story
│   └── contact.html        # Contact & reservation form
├── server/
│   └── index.js            # Express server to serve the public folder
├── package.json            # NPM scripts & dependencies
├── render.yaml             # Render.com deployment configuration
└── README.md               # This file

Key features

- Full-width, fluid layout using w-full and max-w-none patterns.
- Tailwind CSS classes used inline for all styling.
- Glassmorphism cards, gradient CTAs, dark-mode support, and micro-animations.
- Reviews list with star rating, progress bars showing rating distribution.
- Review submission modal with client-side validation and preview behavior.
- Testimonials carousel, FAQ accordion, and interactive CTAs.
- Accessibility: keyboard support for accordion and modal (Esc to close), ARIA attributes in places.
- Performance: images set to lazy-load, minimal dependencies.

Fonts

At the top of each HTML file you will find comments that indicate Google Fonts used for the project. Example:

<!-- {{font: Poppins}} -->
<!-- {{font: Merriweather}} -->

Include those fonts in your production build or your own hosting if desired for exact typographic fidelity.

Images

- Images use placeholders like: https://pixabay.com/get/gebe9369f39219a59ced0f3d745adf2c1528f7ea689f1fd1509177b00912f61596525fc4e28dea97b669c1b52b30313fe2b3f1f248fddb8968438ed959fd43747_640.jpg. The deployment system (or your designer) can replace these with real assets or the system in your environment may fetch matching images.
- If you have real images, replace the src attributes directly with either local paths (e.g., /public/img/your.jpg) or data URIs.

Local setup

1. Requirements: Node.js 16+ and npm.
2. Install dependencies:

   npm install

3. Run locally:

   npm start

4. For development auto-reload (if you have nodemon installed):

   npm run dev

Deployment

This project includes a render.yaml for Render.com. The start command is npm start. Ensure environment variables are set in your deployment provider if required.

Customization

- Replace placeholder images with your restaurant photography.
- Hook the review submission form up to a backend or third-party service (e.g., a headless CMS or an API) to persist reviews.
- Adjust the Tailwind CDN configuration or switch to a build-time Tailwind config for production control over colors and utilities.

Accessibility & SEO notes

- Basic SEO meta tags are included for social sharing and description.
- Provide alt text for all real images and consider server-side rendering of dynamic review content for better SEO.

Why this layout works

The design uses immersive hero imagery, strong typographic hierarchy, and social proof through reviews and testimonials to build trust. The review modal lowers friction — users can quickly leave feedback — and visual progress bars and rating summaries make the reviews section scannable.

If you want a customized review copy (a single feature review or multiple review variations tuned for a specific restaurant), tell me the restaurant name, cuisine, and tone (e.g., intimate, upscale, family-friendly) and I will generate tailored review texts you can paste into the reviews array in public/index.html.

Enjoy!
