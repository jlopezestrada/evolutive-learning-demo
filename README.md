# Evolutive Learning Demo
Examples and visualizations of how evolutive programming works.

## Project Structure (WIP, may change)
```markdown
├── cmd/                    # Main application entry points
│   └── evolutive/          # Console mode main package
│       └── main.go         # Starts the evolutive learning simulation
├── internal/               # Core application logic (private to the module)
│   ├── evolutive/          # Evolutive algorithm implementation
│   │   ├── population.go   # Population initialization & management
│   │   ├── genome.go       # Genome representation & mutation logic
│   │   ├── fitness.go      # Fitness evaluation functions
│   │   └── selection.go    # Selection and crossover logic
│   └── utils/              # Helper functions
│       └── logger.go       # Logging utilities
├── pkg/                    # Public reusable packages
│   └── mathutils/          # Math helpers for mutation rates, randomization
│       └── random.go
├── Dockerfile              # Container definition for the project
├── go.mod                  # Go module definition
├── go.sum                  # Go dependencies checksum
└── README.md               # Project documentation
```

## Quickstart
### Go Installation
---
The project uses Go `1.24.6` as the main programming language. 
Follow these steps to install the latest version of Go.

```bash
# Remove old Go installation if necessary
sudo rm -rf /usr/local/go

# 1. Set the version and architecture
VER="go1.24.6" # latest version when the project was developed
OS_ARCHITECTURE="linux-amd64" # architecture of the system, use arm if needed

# 2. Download and extract
wget "https://go.dev/dl/${VER}.${OS_ARCHITECTURE}.tar.gz"
sudo tar -C /usr/local -xzf "${VER}.${OS_ARCHITECTURE}.tar.gz"

# 3. Add Go to PATH
echo 'export PATH="/usr/local/go/bin:$PATH"' >> ~/.profile

# 4. Apply changes
source ~/.profile

# 5. Verify installation
go version
```

### Run the program
---
TODO

## License
`MIT`
