# UGSFootGun
An open source backend for Unity Gaming Service to store player data and to set up your economy service

## project directory
The project directory may change later.


project-root/
├── cmd/                  # Entry points for the application
│   └── server/
│       └── main.go       # Main application entry
├── config/               # Configuration files and utilities
│   └── config.go
├── internal/             # Core application logic
│   ├── api/              # API layer
│   │   ├── handlers/     # HTTP handlers
│   │   │   ├── player.go # Player-related handlers
│   │   │   └── economy.go # Economy-related handlers
│   │   └── router.go     # Routes setup
│   ├── database/         # Database layer
│   │   ├── postgres.go   # PostgreSQL connection and queries
│   │   └── migrations/   # SQL migration files
│   ├── models/           # Data models
│   │   ├── player.go     # Player model
│   │   └── economy.go    # Economy model
│   ├── services/         # Business logic
│   │   ├── player.go     # Player service
│   │   └── economy.go    # Economy service
│   └── utils/            # Utility functions
│       └── helpers.go
├── pkg/                  # Optional: Shared packages for reuse
├── scripts/              # Scripts for deployment or management
│   └── setup_db.sh
└── go.mod                # Go module file


## to run the project
```cmd
go run cmd/server/main.go
```