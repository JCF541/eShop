# E-Commerce Microservices Platform

## Project Vision
This project demonstrates an e-commerce platform built with a microservices architecture using Python (Flask), MySQL, and a JavaScript (React) front end. Each core functionality—user management, product catalog, and order processing—is developed as an independent microservice, enabling modularity, scalability, and maintainability.

## Architecture Overview
- **User Service:** Handles user registration, authentication (via JWT), and profile management.
- **Product Service:** Manages product data, including creation, updates, and inventory control.
- **Order Service:** Processes orders and tracks order statuses.
- **Frontend:** A responsive React application that interacts with the backend services.
- **Common:** Shared utilities, documentation, and API contracts.

## Initial Milestones
1. **Project Setup:** Establish directory structure, virtual environments, and containerization.
2. **User Service Implementation:** Develop and test user registration, login, and profile APIs.
3. **Product Service Implementation:** Develop and test CRUD operations for products.
4. **Order Service Implementation:** Develop and test order placement and management.
5. **Front-End Integration:** Build a React app to interface with all microservices.
6. **Deployment:** Containerize services with Docker and set up CI/CD pipelines.

## Getting Started

### Prerequisites
- Python 3.9+
- Node.js (for the React frontend)
- MySQL Server
- Docker & Docker Compose

### Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/ecommerce-microservices.git
   cd ecommerce-microservices

### VSCode Project Setup

## **Step-by-Step Guide: Downloading, Installing, and Setting Up Packages via VSCode Terminal**

1. **Open VSCode and Load Your Project:**
   - Launch Visual Studio Code.
   - Open your project folder by selecting **File > Open Folder...** and choosing your `ecommerce-microservices` directory.

2. **Open the Integrated Terminal:**
   - Open the terminal in VSCode by pressing `Ctrl + ` (backtick) or via **View > Terminal**.

3. **Navigate to a Microservice Folder (e.g., User Service):**
   - In the terminal, type:
     ```bash
     cd user-service
     ```

4. **Create a Virtual Environment:**
   - Run the following command to create a virtual environment named `venv`:
     ```bash
     python3 -m venv venv
     ```
   - *Note:* If you’re on Windows, use:
     ```bash
     python -m venv venv
     ```

5. **Activate the Virtual Environment:**
   - **On macOS/Linux:**
     ```bash
     source venv/bin/activate
     ```
   - **On Windows:**
     ```bash
     .\venv\Scripts\activate
     ```

6. **Confirm the Virtual Environment Activation:**
   - Your terminal prompt should now show the virtual environment name (e.g., `(venv)`).

7. **Download & Install the Required Packages:**
   - Ensure that your `requirements.txt` file is present in the `user-service` directory.
   - Run the following command to install all dependencies:
     ```bash
     pip install -r requirements.txt
     ```
   - This command reads the `requirements.txt` file and downloads the listed packages (e.g., Flask, SQLAlchemy, etc.) along with their specified versions.

8. **Verify the Installation:**
   - You can check the installed packages by running:
     ```bash
     pip freeze
     ```
   - This command should list all installed packages matching those in your `requirements.txt`.

9. **Repeat for Other Services:**
   - For each microservice (e.g., `product-service` and `order-service`), navigate into the folder, create and activate a virtual environment, and install the dependencies using their respective `requirements.txt` files.

10. **Optional: Create a VSCode Task for Repeated Setup (Advanced):**
    - You can create a `tasks.json` file in the `.vscode` directory to automate these commands. For example:
      ```json
      {
          "version": "2.0.0",
          "tasks": [
              {
                  "label": "Setup User Service",
                  "type": "shell",
                  "command": "python3 -m venv venv && source venv/bin/activate && pip install -r requirements.txt",
                  "group": "build",
                  "problemMatcher": []
              }
          ]
      }
      ```
    - Run this task via **Terminal > Run Task...** in VSCode.

Following these instructions will ensure that you have a consistent development environment across all your microservices, making it easier to start coding and testing your application.

---

These corrections and the detailed setup guide should provide you with a clear and actionable plan for both organizing your project’s directory structure and configuring your development environment in VSCode.
