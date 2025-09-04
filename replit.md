# Overview

This is a full-stack inventory management application built with Express.js backend and React frontend. The application allows users to manage products with features including adding, editing, deleting, and searching products. It uses a PostgreSQL database with Drizzle ORM for data persistence and provides a modern, responsive UI built with shadcn/ui components.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **UI Library**: shadcn/ui components built on top of Radix UI primitives
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack React Query for server state management
- **Forms**: React Hook Form with Zod validation
- **Routing**: Wouter for client-side routing
- **Component Structure**: Modular components with separation of concerns (forms, tables, modals)

## Backend Architecture
- **Framework**: Express.js with TypeScript
- **API Design**: RESTful API with CRUD operations for products
- **Validation**: Zod schemas for request validation
- **Error Handling**: Centralized error handling middleware
- **Development**: Hot reload with Vite middleware integration
- **Storage**: Abstracted storage interface with in-memory implementation for development

## Data Layer
- **Database**: PostgreSQL configured for production
- **ORM**: Drizzle ORM with type-safe queries
- **Schema**: Products table with fields for name, category, price, quantity, and SKU
- **Migrations**: Drizzle migrations system for schema management
- **Validation**: Shared Zod schemas between frontend and backend

## Project Structure
- **Monorepo Setup**: Single repository with client, server, and shared code
- **Shared Types**: Common schemas and types in `/shared` directory
- **Path Aliases**: Configured TypeScript path mapping for clean imports
- **Build System**: Separate build processes for client (Vite) and server (esbuild)

## Development Experience
- **Hot Reload**: Vite dev server with Express middleware integration
- **Type Safety**: End-to-end TypeScript with shared schemas
- **Code Quality**: ESLint and TypeScript strict mode
- **Development Tools**: Replit-specific plugins for enhanced development experience

# External Dependencies

## Core Framework Dependencies
- **@neondatabase/serverless**: PostgreSQL database client optimized for serverless environments
- **drizzle-orm**: Type-safe ORM for database operations
- **express**: Web application framework for the backend API
- **react**: Frontend library for building user interfaces
- **@tanstack/react-query**: Server state management and caching

## UI and Styling
- **@radix-ui/***: Comprehensive collection of accessible UI primitives
- **tailwindcss**: Utility-first CSS framework
- **class-variance-authority**: Utility for creating variant-based component styles
- **clsx**: Utility for constructing className strings

## Form Handling and Validation
- **react-hook-form**: Performant forms with easy validation
- **@hookform/resolvers**: Resolvers for various validation schemas
- **zod**: TypeScript-first schema validation
- **drizzle-zod**: Integration between Drizzle ORM and Zod validation

## Development and Build Tools
- **vite**: Fast build tool and development server
- **typescript**: Static type checking
- **esbuild**: Fast JavaScript bundler for production builds
- **tsx**: TypeScript execution environment for development

## Additional Utilities
- **date-fns**: Modern JavaScript date utility library
- **wouter**: Minimalist routing for React applications
- **cmdk**: Command palette interface component
- **embla-carousel-react**: Carousel component for React