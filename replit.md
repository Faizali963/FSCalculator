# Calculator.net

## Overview

Calculator.net is a comprehensive online calculator platform that provides a wide variety of calculators for different domains including financial, fitness & health, math, and other specialized calculations. The application features a clean, Material Design-inspired interface with both light and dark themes, and includes a prominent scientific calculator as the main feature alongside categorized calculator collections.

The platform is designed as a utility-focused website that prioritizes usability and information density, offering hundreds of different calculator types organized into intuitive categories for easy discovery and access.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript in a Single Page Application (SPA) architecture
- **Routing**: Wouter for lightweight client-side routing with three main routes:
  - Home page (`/`) - features scientific calculator and category overview
  - Category pages (`/category/:id`) - lists calculators within a specific category
  - Individual calculator pages (`/calculator/:category/:id`) - specific calculator implementations
- **UI Framework**: shadcn/ui component library built on Radix UI primitives
- **Styling**: Tailwind CSS with custom design system implementing Material Design principles
- **State Management**: TanStack Query for server state and local React state for component-level state
- **Theme System**: Custom light/dark mode implementation with CSS variables and local storage persistence

### Design System
- **Color Palette**: Sophisticated light/dark mode system with semantic color tokens
- **Typography**: Inter font family with JetBrains Mono for calculator displays
- **Layout**: Consistent spacing system using Tailwind's 4-unit grid (2, 4, 6, 8 units)
- **Components**: Reusable component library with variants for different calculator types and UI elements

### Backend Architecture
- **Runtime**: Node.js with Express.js server
- **Database ORM**: Drizzle ORM configured for PostgreSQL
- **Session Management**: PostgreSQL-backed sessions using connect-pg-simple
- **API Structure**: RESTful API with `/api` prefix for all endpoints
- **Build System**: Vite for frontend bundling with esbuild for server compilation

### Data Layer
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Schema**: User management system with username/password authentication
- **Connection**: Neon Database serverless PostgreSQL for cloud deployment
- **Migrations**: Drizzle Kit for database schema management and migrations

### Calculator Implementation
- **Scientific Calculator**: Full-featured calculator with trigonometric functions, logarithms, and advanced operations
- **Form-based Calculators**: Reusable `CalculatorForm` component for input-driven calculators (financial, health, etc.)
- **Category System**: Organized calculator discovery through categorized browsing
- **Responsive Design**: Mobile-first approach with grid layouts adapting from 2 columns (mobile) to 4 columns (desktop)

### Development Environment
- **Hot Reload**: Vite development server with HMR for rapid development
- **Error Handling**: Runtime error overlay for development debugging
- **TypeScript**: Full type safety across frontend and backend with shared types
- **Path Aliases**: Organized imports using `@/` for client code and `@shared/` for shared utilities

## External Dependencies

### UI and Styling
- **Radix UI**: Comprehensive primitive component library for accessible UI components
- **Tailwind CSS**: Utility-first CSS framework for responsive design
- **Lucide React**: Icon library for consistent iconography
- **class-variance-authority**: Type-safe variant API for component styling

### State Management and Data Fetching
- **TanStack Query**: Server state management, caching, and synchronization
- **React Hook Form**: Form handling with validation support
- **Zod**: Schema validation for form inputs and API responses

### Database and Backend
- **Neon Database**: Serverless PostgreSQL hosting platform
- **Drizzle ORM**: Type-safe SQL query builder and ORM
- **Express.js**: Web application framework for Node.js
- **connect-pg-simple**: PostgreSQL session store for Express sessions

### Development Tools
- **Vite**: Frontend build tool and development server
- **TypeScript**: Static type checking for JavaScript
- **esbuild**: Fast JavaScript bundler for server-side code
- **PostCSS**: CSS processing with Autoprefixer for vendor prefixes

### Utility Libraries
- **date-fns**: Date manipulation and formatting utilities
- **clsx**: Conditional CSS class name utility
- **nanoid**: URL-safe unique ID generator
- **embla-carousel**: Carousel component for image galleries