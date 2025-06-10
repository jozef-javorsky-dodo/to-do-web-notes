# [https://to-do-web-notes.web.app/](https://to-do-web-notes.web.app/)

## 📝 To-Do List SPA

* **Framework:** [Vue.js 3](https://vuejs.org/) (via CDN)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via CDN)

A definitive Single-Page Application for managing tasks, meticulously crafted for clarity, performance, and security. This project is an exploration of minimalist, high-excellence web engineering, delivered in a single, self-contained `index.html` file.

### Abstract

This is not just another to-do application. It is a testament to the philosophy that true sophistication is found in simplicity. The entire application—logic, styling, and structure—is encapsulated in a single file, yet it compromises nothing on modern features, security, or user experience. It is designed to be a flawless tool that is both powerful and unobtrusive, respecting the user's focus and privacy.

### Features

* **Full CRUD Functionality:** Add, edit (on double-click), complete, and delete tasks.
* **Stateful Filtering:** Dynamically filter tasks by `All`, `Active`, and `Completed` states.
* **Persistent State:** Your session is automatically saved to your browser's Local Storage and restored on your next visit.
* **Elegant UI:** A clean, responsive interface with smooth UX.
* **Light & Dark Modes:** Automatically adapts to your system's preferred color scheme, with a manual toggle for user preference.
* **Fully Accessible:** Built with ARIA attributes, keyboard navigability, and screen-reader announcements for all actions.
* **Cross-Browser Compatible:** Works flawlessly on all modern web browsers.

### 1. Simplicity and Portability

The entire application is a single `index.html` file. This demonstrates a "zero build" approach, eliminating the need for complex toolchains, package managers, or transpilers. The result is a universally portable, transparent, and easily deployable artifact.

### 2. Uncompromising Security

Security is not an afterthought; it is a foundational requirement.

* **Strict Content Security Policy (CSP):** A robust CSP is implemented via `<meta>` tag to prevent a wide range of injection attacks, including XSS. It specifies exactly which resources are trusted, blocking all others.
* **Subresource Integrity (SRI):** All external assets loaded from a CDN (Vue.js, Tailwind CSS) include an integrity hash. This guarantees that the files have not been tampered with, preventing supply-chain attacks.
* **OWASP Compliance:** Adheres to the principles of the OWASP Top 10 by mitigating common web vulnerabilities at the source.

### 3. Performance by Design

The application is engineered to be exceptionally fast.

* **Minimal Footprint:** By using lightweight libraries and a single file, the initial load is near-instantaneous.
* **Pre-compiled Assets:** It uses a pre-compiled version of Tailwind CSS, avoiding the performance overhead of the Just-in-Time (JIT) compiler in the browser.
* **Efficient Rendering:** Vue.js 3's highly optimized virtual DOM ensures that UI updates are fast and efficient, even with a large number of tasks.

### 4. Universal Accessibility

The application is built to be usable by everyone, regardless of their abilities.

* **Semantic HTML:** Correct use of HTML5 tags (`<main>`, `<header>`, `<nav>`) provides a clear structure.
* **ARIA Roles & Attributes:** All interactive elements have appropriate ARIA labels and roles, providing a rich experience for screen reader users.
* **Focus Management:** Logical focus order and keyboard navigability ensure the application can be operated entirely without a mouse.
* **Live Announcements:** A visually hidden `aria-live` region announces the result of actions, providing crucial feedback for non-visual users.

#### Author

github.com/jozef-javorsky-dodo

#### License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
