# AI Workshop - OpenEdge ABL Project

This project demonstrates the Business Entity pattern for OpenEdge ABL applications, providing a standardized approach to data access with separation of UI and business logic layers.

## Project Structure

- `src/business/` - Business entity classes and dataset definitions
- `src/` - UI window files (.w)
- `dump/` - Database schema definitions
- `doc/` - Architecture documentation
- `.windsurf/` - Windsurf IDE rules and workflows
- `.github/` - GitHub issue templates

## Key Components

- **CustomerEntity** - Business entity for Customer data access (CRUD + validation)
- **EntityFactory** - Singleton factory for managing business entity instances
- **CustomerDataset.i** - Dataset/temp-table definition for Customer data transfer
- **CustomerWin.w** - Customer management UI window
- **ItemWin.w** - Item management UI window

## Architecture

Uses the Business Entity pattern with:
- UI Layer (Windows) → Business Entity Layer → Database Layer
- EntityFactory singleton for entity lifecycle management
- Dataset-based data transfer between layers

## Requirements

- OpenEdge 12.8+
- Sports2000 sample database
