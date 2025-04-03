flask_api_backend/
│── .env
│── .gitignore
│── config.py
│── run.py
│── requirements.txt
│── README.md
│
├── venv/                   # Virtual environment (excluded in .gitignore)
│
├── instance/               # Local instance configuration
│   ├── config.py
│
├── app/
│   ├── __init__.py         # App factory function
│   │
│   ├── api/                # API routes using Blueprints
│   │   ├── __init__.py
│   │   ├── routes.py
│   │   ├── auth_routes.py
│   │   ├── user_routes.py
│   │   ├── ai_routes.py
│   │
│   ├── controllers/        # Business logic layer
│   │   ├── __init__.py
│   │   ├── auth_controller.py
│   │   ├── user_controller.py
│   │   ├── ai_controller.py
│   │
│   ├── models/             # SQLAlchemy Models
│   │   ├── __init__.py
│   │   ├── base_model.py
│   │   ├── user_model.py
│   │   ├── ai_model.py
│   │
│   ├── services/           # Service Layer for AI & Business Logic
│   │   ├── __init__.py
│   │   ├── ai_service.py
│   │   ├── user_service.py
│   │
│   ├── utils/              # Utility functions (Logging, Security)
│   │   ├── __init__.py
│   │   ├── helpers.py
│   │   ├── logger.py
│   │   ├── security.py
│   │
│   ├── extensions.py       # Initialize Flask extensions
│   ├── config.py           # Configuration settings
│
├── migrations/             # Database migrations
│
├── tests/                  # Unit tests
│   ├── __init__.py
│   ├── test_auth.py
│   ├── test_users.py
│   ├── test_ai.py
│
└── docs/                   # Documentation
    ├── api_docs.md
    ├── architecture.md
