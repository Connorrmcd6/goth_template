# Golang Templ HTMX (GoTH) Template

This repository serves as a template for building server-side web applications using Golang, Templ, and HTMX. It provides a solid foundation to get started quickly with these technologies.

## Overview

- **Golang**: A statically typed, compiled programming language designed for simplicity and efficiency.
- **Templ**: A templating engine for Go, enabling easy and efficient HTML generation.
- **HTMX**: A library that allows you to access modern browser features directly from HTML, making it easier to build interactive web applications.

## Getting Started

### Prerequisites

- [Golang](https://golang.org/doc/install) (version 1.16 or higher)
- [Node.js](https://nodejs.org/) (for managing frontend dependencies)
- [Tailwind CSS](https://tailwindcss.com/) (for styling)

### Installation

1. **Clone the repository**:

   ```sh
   git clone https://github.com/yourusername/goth-template.git
   cd goth-template
   ```

2. **Install dependencies**:

   ```sh
   go mod tidy
   go install github.com/air-verse/air@latest
   go install github.com/a-h/templ/cmd/templ@latest
   npm install
   ```

3. **Build the project**:

   ```sh
   make build
   ```

4. **Run the application in development mode with hot reloading**:
   ```sh
   terminal 1: air
   terminal 2: templ generate --watch --proxy=http://localhost:3000
   terminal 3: make css
   ```

### Usage

- Access the application at `http://localhost:3000`.
- Modify the templates in the `views` directory to customize the HTML.
  - The template is configured to use the [pines.js](https://devdojo.com/pines) UI library to speed up development.
- Use HTMX attributes in your HTML to add interactivity without writing JavaScript.

## Resources

- **Original Idea**: [Watch the video](https://www.youtube.com/live/1dqp1s72Z8E?si=BQKgbhSajzaQWnlP) that inspired this template.
- **Golang Documentation**: [golang.org/doc](https://golang.org/doc/)
- **Templ Documentation**: [templ.dev](https://templ.guide/)
- **HTMX Documentation**: [htmx.org](https://htmx.org/)

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with your improvements.
