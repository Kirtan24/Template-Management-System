# 🧾 Template Management System

It is a centralized Template Management System that streamlines the creation, management, and distribution of email and document templates with support for e-signatures, scheduling, and dynamic content.

## ⚙️ Features

- Role-based access: System Admin, Company Admin, Employee, Signer
- Document & Email template management
- Dynamic fields with docx templates
- Bulk document generation via Excel/CSV
- E-signature workflows
- Email scheduling and inbox tracking

## 👤 User Roles

| Role          | Permissions Summary                                       |
| ------------- | --------------------------------------------------------- |
| System Admin  | Full system control (companies, permissions, users, etc.) |
| Company Admin | Manages company templates, users, permissions             |
| Employee      | Uses features based on permissions                        |
| Signer        | Signs documents via secure email link                     |
| Site Visitor  | Registers company request via homepage                    |

## 🚀 Getting Started

### Prerequisites

- Node.js ≥ 18.x
- npm / yarn
- MongoDB / PostgreSQL
- Git
- Docker & Docker Compose (optional, for containerized setup)

### Installation (Without Docker)

```bash
# Clone repo
git clone https://github.com/your-org/template-io.git
cd template-io

# Install backend dependencies
cd template-back
npm install

# Install frontend dependencies
cd ../template-front
npm install
````

### Running with Docker

```bash
# Build and start containers
docker-compose up --build

# To run in detached mode (background)
docker-compose up -d

# Stop containers
docker-compose down
```

> This will automatically build your backend and frontend images and run the application along with any required services defined in `docker-compose.yml`.

### Notes

* Make sure to configure environment variables in `.env` files for both frontend and backend.
