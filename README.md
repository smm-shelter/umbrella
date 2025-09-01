# smm-shelter (v2)

## Overview

The umbrella module is the main orchestration component for the project, serving as a container repository that manages multiple independent sub-repositories. This approach allows each component to be developed, built, and launched independently while providing a unified way to run the complete system.

## Project Structure
```
umbrella
├── backend/            # Subrepository (linked)
├── frontend/           # Subrepository (linked) 
├── other-modules/      # Future subrepositories
├── dumps/              # folder for dumps
└── compose.yaml        # Main orchestration file
```

## Quick Start
1. **Clone the main repository**
```bash
git clone <umbrella-repo-url>
cd umbrella
```
2. **Initialize and update subrepositories**
```bash
git submodule update --init
```
3. **Launch the complete project**
```bash
docker compose up
```

