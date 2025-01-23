# documention

# Node.js and React with Vite: Overview and Setup

## Latest Node.js Versions (As of January 22, 2025)

- **Current Version:** Node.js v23.6.1  
- **Long-Term Support (LTS) Version:** Node.js v22.13.1 (Jod)

The Current version includes the latest features and improvements, suitable for testing and development environments. The LTS version is recommended for production applications due to its stability and extended support.

### Checking Your Node.js Version
To check your installed Node.js version, run the following command:
```bash
node -v
```

---

## What is Node.js Used For?
Node.js is a powerful, open-source runtime environment that allows you to execute JavaScript code on the server side. It enables developers to build scalable, high-performance web applications and tools. Below is a breakdown of its uses:

### 1. Server-Side Web Applications
- Build dynamic, fast, and scalable server-side applications.
- Handle multiple client requests efficiently using its non-blocking, event-driven architecture.
- **Example:** RESTful APIs for web and mobile applications.

### 2. Real-Time Applications
- Ideal for apps requiring real-time interaction, such as:
  - Chat applications
  - Online gaming platforms
  - Collaboration tools (e.g., Google Docs-like apps)
- Technologies like Web Sockets enable real-time communication.

### 3. API Development
- Create lightweight and efficient REST APIs or GraphQL APIs.
- Popular frameworks like **Express.js** simplify API development.

### 4. Microservices
- Well-suited for a microservices architecture where applications are split into smaller, independently deployable services.
- Improves scalability and maintainability.

### 5. Command-Line Tools
- Build CLI tools to automate tasks or simplify workflows.
- **Example:** Tools like ESLint or npm itself are built with Node.js.

### 6. Static File Servers
- Serve static files such as images, HTML, and CSS without needing a separate web server like Apache or Nginx.

### 7. Streaming Applications
- Handle data streams efficiently, making Node.js great for video and audio streaming platforms.
- **Example:** Implementing file uploads or media streaming services.

### 8. IoT Applications
- Manage real-time data processing for Internet of Things (IoT) devices.
- Asynchronous nature helps handle data from numerous devices simultaneously.

### 9. Data-Intensive Applications
- Process large volumes of data in real-time, such as stock trading apps or analytics platforms.

---

## Why Use Node.js?
1. **Performance:** Built on Chrome’s V8 engine, Node.js offers exceptional speed.
2. **Non-Blocking I/O:** Handles multiple requests simultaneously without waiting for processes to complete.
3. **Scalability:** Ideal for handling large-scale, high-traffic applications.
4. **Rich Ecosystem:** npm provides access to a vast library of open-source packages.
5. **JavaScript Everywhere:** Enables full-stack development using a single language (JavaScript) for both client and server sides.

### Key Points:
1. **Environment Variables:** Use `process.env.PORT` so the port can be configured dynamically, especially in production environments like cloud platforms.
2. **Default Port:** If no environment variable is provided, set a default port like 3000 or any other suitable number.
3. **Common Ports:**
   - 3000, 8080, and 5000 are commonly used for development servers.
   - Ensure the port you choose is not already in use by another service.

---

## Why Use React with Vite?

1. **Blazing Fast Development:** Vite leverages native ES modules and modern tooling for near-instant dev server startup.
2. **Optimized Builds:** Vite ensures optimized production builds with minimal configuration.
3. **Hot Module Replacement (HMR):** Changes in your code reflect instantly in the browser without a full reload.
4. **Minimal Boilerplate:** Setting up a React app with Vite is fast and straightforward.

---

## Setting Up React with Vite

1. **Install Vite**
   Run the following command to create a Vite-powered React project:
   ```bash
   npm create vite@latest my-react-app --template react
   ```
   Alternatively, for TypeScript:
   ```bash
   npm create vite@latest my-react-app --template react-ts
   ```

2. **Navigate to Your Project**
   ```bash
   cd my-react-app
   ```

3. **Install Dependencies**
   ```bash
   npm install
   ```

4. **Start Development Server**
   ```bash
   npm run dev
   ```

---

## About `package.json`

A `package.json` file is a fundamental component in Node.js projects. It serves as a metadata file for the project and contains important information about the project, including dependencies, scripts, and other configurations.

### Key Uses of `package.json`

1. **Project Metadata:**
   - **Name:** The name of your project or application.
   - **Version:** The version number of your project.
   - **Description:** A short description of your project.
   - **Author:** The person or organization responsible for the project.
   - **License:** Specifies the license under which the project is released.

2. **Dependencies:**
   - **Dependencies:** External libraries or packages required to run the application.
   - **DevDependencies:** Libraries needed only for development (e.g., testing frameworks, bundlers).
   - **PeerDependencies:** Specifies versions of other packages your package is compatible with.

3. **Scripts:**
   Define custom scripts that can be run using `npm run <script-name>`. Examples:
   ```json
   "scripts": {
     "start": "node server.js",
     "test": "jest"
   }
   ```

4. **Package Management:**
   - Running `npm install` uses the `package.json` file to install the listed dependencies.
   - Ensures consistency of dependencies across environments.

5. **Version Control:**
   - Tracks versions of dependencies, ensuring consistency across environments.

### Key Commands Involving `package.json`:
- `npm init`: Initializes a new Node.js project and creates a `package.json` file.
- `npm install`: Installs dependencies listed in the `package.json` file.
- `npm run <script>`: Executes the script defined in `package.json`.

---

## Dependencies

<table>
  <thead>
    <tr>
      <th>Package Name</th>
      <th>Version</th>
    </tr>
  </thead>
  <tbody>
   <tr>
    <tr><td> ## @ant-design/icons </td><td>^5.5.2</td></tr>
    <tr><td>@emotion/react</td><td>^11.13.3</td></tr>
    <tr><td>@emotion/styled</td><td>^11.13.3</td></tr>
    <tr><td>@fortawesome/fontawesome-svg-core</td><td>^11.13.0</td></tr>
    <tr><td>@fortawesome/free-regular-svg-icons</td><td>^6.5.2</td></tr>
    <tr><td>@fortawesome/free-solid-svg-icons</td><td>^6.5.2</td></tr>
    <tr><td>@fortawesome/react-fontawesome</td><td>^0.2.2</td></tr>
    <tr><td>@mui/material</td><td>^6.1.5</td></tr>
    <tr><td>@mui/x-date-pickers</td><td>^7.21.0</td></tr>
    <tr><td>@popperjs/core</td><td>^2.11.8</td></tr>
    <tr><td>@react-pdf-viewer/core</td><td>^3.12.0</td></tr>
    <tr><td>@react-pdf-viewer/default-layout</td><td>^3.12.0</td></tr>
    <tr><td>@react-pdf/renderer</td><td>^3.4.5</td></tr>
    <tr><td>@reduxjs/toolkit</td><td>^2.5.0</td></tr>
    <tr><td>@stomp/stompjs</td><td>^7.0.0</td></tr>
    <tr><td>Antd</td><td>^5.21.5</td></tr>
    <tr><td>Aos</td><td>^2.3.4</td></tr>
    <tr><td>Axios</td><td>^1.6.8</td></tr>
    <tr><td>Bootstrap</td><td>^5.3.3</td></tr>
    <tr><td>canvas-confetti</td><td>^1.9.3</td></tr>
    <tr><td>chart.js</td><td>^4.4.7</td></tr>
    <tr><td>chroma-js</td><td>^3.1.1</td></tr>
    <tr><td>Colormap</td><td>^2.3.2</td></tr>
    <tr><td>crypto-js</td><td>^4.2.0</td></tr>
    <tr><td>date-fns</td><td>^2.30.0</td></tr>
    <tr><td>Dayjs</td><td>^1.11.13</td></tr>
    <tr><td>Formic</td><td>^2.4.6</td></tr>
    <tr><td>Fortawesome</td><td>^0.0.1-security</td></tr>
    <tr><td>html2canvas</td><td>^1.4.1</td></tr>
    <tr><td>html2pdf.js</td><td>^0.10.2</td></tr>
    <tr><td>Io</td><td>1.5.0</td></tr>
    <tr><td>Jspdf</td><td>^2.5.1</td></tr>
    <tr><td>jspdf-autotable</td><td>^3.8.2</td></tr>
    <tr><td>pdf-lib</td><td>^1.17.1</td></tr>
    <tr><td>Pdfmake</td><td>^0.2.10</td></tr>
    <tr><td>React</td><td>^18.2.0</td></tr>
    <tr><td>react-big-calendar</td><td>^1.12.1</td></tr>
    <tr><td>react-bootstrap</td><td>^2.10.2</td></tr>
    <tr><td>react-calendar</td><td>^5.0.0</td></tr>
    <tr><td>react-chartjs-2</td><td>^5.2.0</td></tr>
    <tr><td>react-color</td><td>^2.19.3</td></tr>
    <tr><td>react-confetti</td><td>^6.1.0</td></tr>
    <tr><td>react-datepicker</td><td>^6.9.0</td></tr>
    <tr><td>react-dom</td><td>^18.2.0</td></tr>
    <tr><td>react-flatpickr</td><td>^3.10.13</td></tr>
    <tr><td>react-fontawesome</td><td>^1.7.1</td></tr>
    <tr><td>react-hook-form</td><td>^7.52.1</td></tr>
    <tr><td>react-icon</td><td>^1.0.0</td></tr>
    <tr><td>react-icons</td><td>^5.2.1</td></tr>
    <tr><td>react-modal</td><td>^3.16.1</td></tr>
    <tr><td>react-pdf</td><td>^9.1.0</td></tr>
    <tr><td>react-phone-number-input</td><td>^3.4.3</td></tr>
    <tr><td>react-qr-code</td><td>^2.0.15</td></tr>
    <tr><td>react-redux</td><td>^9.2.0</td></tr>
    <tr><td>react-router-dom</td><td>^6.23.1</td></tr>
    <tr><td>react-spinner</td><td>^0.2.7</td></tr>
    <tr><td>react-spinners</td><td>^0.13.8</td></tr>
    <tr><td>react-stomp</td><td>^5.1.0</td></tr>
    <tr><td>react-time-picker</td><td>^7.0.0</td></tr>
    <tr><td>react-to-print</td><td>^2.15.1</td></tr>
    <tr><td>react-toastify</td><td>^10.0.5</td></tr>
    <tr><td>react-tooltip</td><td>^5.27.1</td></tr>
    <tr><td>react-web-share</td><td>^2.0.2</td></tr>
    <tr><td>Recharts</td><td>^2.12.6</td></tr>
    <tr><td>socket.io-client</td><td>^4.8.1</td></tr>
    <tr><td>Sockjs</td><td>^0.3.24</td></tr>
    <tr><td>sockjs-client</td><td>^1.6.1</td></tr>
    <tr><td>Stompjs</td><td>^2.3.3</td></tr>
    <tr><td>svg-to-img</td><td>^2.0.9</td></tr>
    <tr><td>theme-change</td><td>^2.5.0</td></tr>
    <tr><td>Xlsx</td><td>^0.18.5</td></tr>
    <tr><td>Yup</td><td>^1.4.0</td></tr>
  </tbody>
</table>

## DevDependencies

<table>
  <thead>
    <tr>
      <th>Package Name</th>
      <th>Version</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>@types/react</td><td>^18.2.66</td></tr>
    <tr><td>@types/react-dom</td><td>^18.2.22</td></tr>
    <tr><td>@vitejs/plugin-react</td><td>^4.2.1</td></tr>
    <tr><td>Autoprefixer</td><td>^10.4.19</td></tr>
    <tr><td>Eslint</td><td>^8.57.0</td></tr>
    <tr><td>eslint-plugin-react</td><td>^8.57.0</td></tr>
    <tr><td>eslint-plugin-react-hooks</td><td>^4.6.0</td></tr>
    <tr><td>eslint-plugin-react-refresh</td><td>^0.4.6</td></tr>
    <tr><td>Postcss</td><td>^8.4.39</td></tr>
    <tr><td>Tailwindcss</td><td>^3.4.4</td></tr>
    <tr><td>Vite</td><td>^5.3.3</td></tr>
  </tbody>
</table>

## Usage
Clone the repository and run the following commands to install the dependencies:

```bash
npm install
```

## Dependencies Overview

### Core Dependencies
- [@ant-design/icons](@ant-design/icons): Provides Ant Design icons for UI components.
- **@emotion/react & @emotion/styled**: Used for CSS-in-JS styling, allowing you to style React components directly.
- **@fortawesome/***: Font Awesome icon library for React, offering scalable vector icons.
- **@mui/material**: Material UI framework components, enabling easy and consistent design patterns for React apps.
- **@react-pdf-viewer/core & default-layout**: Libraries for rendering and displaying PDF documents in React.
- **@reduxjs/toolkit**: Simplifies Redux development, providing utilities and a standard approach for managing state.
- **axios**: Promise-based HTTP client for making API requests to communicate with external services.
- **react**: Main React library for building user interfaces with reusable components.
- **react-router-dom**: For handling routing in the app, allowing users to navigate between different views.
- **react-toastify**: Toast notifications for easy feedback to users.
- **socket.io-client**: Used for real-time WebSocket communication between the client and server.
- **tailwindcss**: Utility-first CSS framework for building custom designs with minimal effort.



---

## DevDependencies

- **eslint**: A linter for identifying and fixing JavaScript issues in the code.
- **vite**: A fast build tool that serves the app with hot-reloading, improving the development experience.
- **autoprefixer**: Automatically adds vendor prefixes to CSS rules for compatibility across different browsers.
- **typescript**: Adds TypeScript support, providing static type checking and improved development experience.



---

