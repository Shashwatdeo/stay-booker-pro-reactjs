# Stay Booker Pro

**Stay Booker Pro** is a production-ready hotel booking website built with modern web technologies. It is designed to be a fully functional and responsive web application for hotel booking services.

> 🔧 For the backend API, check out: [`staybooker-express-api`](https://github.com/Shashwatdeo/staty-booker-pro-express-api.git)

---

## 🚀 Key Features

- **Production-Ready**: Crafted with real-world deployment and usability in mind.  
- **Modern Tech Stack**: Built using React.js, Tailwind CSS, MirageJS for mocking APIs, and Cypress for end-to-end testing.  
- **Containerization with Docker**: The application is containerized using Docker for consistent environment setup and smooth deployments.  
- **CI/CD with Jenkins**: Integrated Jenkins pipeline to automate testing and deployment processes for efficient DevOps workflows.  
- **Skeleton Loading**: Enhances user experience with skeleton screens during data loading.  
- **Responsive Design**: Tailwind CSS ensures the UI is fully responsive across all devices.  
- **Comprehensive Test Coverage**: Cypress test suites validate core functionalities and ensure reliability.  
- **Future Backend Integration**: Planned integration with Express.js for a complete full-stack experience.  

---

## 🧑‍💻 Getting Started

Follow these instructions to set up the project locally for development and testing.

### Prerequisites

- Node.js  
- npm or yarn  
- Docker (optional, for containerized setup)  

### Installation

1. **Clone the repository**  
   `git clone https://github.com/Shashwatdeo/stay-booker-pro-reactjs.git`

2. **Navigate to the project directory**  
   `cd stay-booker-pro`

3. **Install dependencies**  
   `npm install`  
   _or_  
   `yarn install`

4. **Start the development server**  
   `npm start`  
   _or_  
   `yarn start`  
   The application will be running at [http://localhost:3000](http://localhost:3000)

---

## 🐳 Docker Setup (Optional)

To run the application inside a Docker container:

1. **Build the Docker image**  
   `docker build -t stay-booker-pro .`

2. **Run the container**  
   `docker run -p 3000:3000 stay-booker-pro`  
   Access the app at [http://localhost:3000](http://localhost:3000)

---

## 🔁 Jenkins CI/CD Pipeline

The project includes a Jenkins pipeline for automated CI/CD processes:

- **Triggers on push to main branch**
- **Steps included**:
  - Install dependencies  
  - Run lint checks and tests  
  - Build the project  
  - Deploy the container (optional)  

This helps streamline the development process and ensures consistent delivery of quality software.

---

## ✅ Running the Tests

Cypress is used for end-to-end testing. To run tests:

`npm test`  
_or_  
`npx cypress open`  

This will open the Cypress test runner where you can execute specific or all test cases.

---

## 🔍 Code Quality and Workflow

### Husky Pre-Commit Hooks  
Husky is configured to run pre-commit hooks that ensure formatting and linting are followed automatically.

### GitHub Actions Workflow  
GitHub Actions automate:  
- Build validation  
- Prettier formatting checks  
- Test execution  

This ensures each pull request or code push maintains the integrity and quality of the codebase.

---

## 🤝 Contributing

We welcome contributions!

If you have ideas, bug fixes, or new features to suggest, feel free to open an issue or a pull request.

### Code Quality & Linting

Please run linting before committing changes:  
`npm run lint-fix`

To skip checks (only if necessary):  
`git commit -m "Your message" -n`

---

## 🌱 Future Scope

- Backend integration with **Express.js**  
- Authentication & user roles (Admin/Guest)  
- Booking confirmation emails  
- Admin dashboard for hotel management  
- Payment gateway integration  
