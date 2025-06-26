# Wayfare Deli & Coffee - Full-Stack Web Application

## Overview

This is a modern React-based restaurant website for Wayfare Deli & Coffee, a plant-forward coffee shop and deli in Claremont, Cape Town. The application features a complete restaurant website with performance optimizations, SEO features, and a modern design system built with React, TypeScript, and Tailwind CSS.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS with shadcn/ui component library
- **State Management**: TanStack Query (React Query) for server state
- **Routing**: Wouter for client-side routing
- **Build Tool**: Vite for fast development and optimized builds
- **UI Components**: Radix UI primitives with custom theming

### Backend Architecture
- **Runtime**: Node.js with Express.js
- **Language**: TypeScript with ES modules
- **Database**: PostgreSQL with Drizzle ORM
- **Session Management**: Express sessions with PostgreSQL storage
- **Development**: Hot reload with Vite integration

### Database Layer
- **ORM**: Drizzle ORM for type-safe database operations
- **Database**: PostgreSQL (configured for Neon serverless)
- **Schema**: Centralized schema definitions in `/shared/schema.ts`
- **Migrations**: Drizzle Kit for database migrations

## Key Components

### Performance Optimizations
- **Image Optimization**: Custom lazy loading with intersection observer
- **Caching**: Browser caching with proper cache headers
- **Code Splitting**: Vite-based code splitting and minification
- **Core Web Vitals**: Performance monitoring and optimization
- **Service Worker**: Client-side caching for offline support

### SEO Features
- **Meta Tags**: Comprehensive Open Graph and Twitter Card support
- **Sitemap**: XML sitemap generation
- **Structured Data**: Proper HTML semantics
- **Google Site Verification**: Integrated verification

### UI/UX Features
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Accessibility**: WCAG compliant with reduced motion support
- **Animation**: Smooth scroll animations with intersection observer
- **Component Library**: Comprehensive shadcn/ui components

## Data Flow

### Frontend Data Flow
1. React components use TanStack Query for server state management
2. Custom hooks handle scroll animations and performance optimizations
3. Wouter handles client-side routing
4. Tailwind CSS provides consistent styling

### Backend Data Flow
1. Express.js handles HTTP requests and routing
2. Drizzle ORM provides type-safe database operations
3. PostgreSQL stores user data and sessions
4. Vite middleware serves the frontend in development

### Database Schema
- **Users Table**: Basic user authentication schema
- **Schema Validation**: Zod integration for runtime validation
- **Type Safety**: Full TypeScript integration with Drizzle

## External Dependencies

### Core Dependencies
- **@tanstack/react-query**: Server state management
- **drizzle-orm**: Type-safe database operations
- **@neondatabase/serverless**: PostgreSQL serverless connection
- **wouter**: Lightweight routing
- **@radix-ui**: Accessible UI primitives

### Development Tools
- **Vite**: Build tool and development server
- **TypeScript**: Type safety and better development experience
- **Tailwind CSS**: Utility-first CSS framework
- **PostCSS**: CSS processing and optimization

### Third-Party Services
- **Google Fonts**: Web font loading
- **Font Awesome**: Icon library
- **Google Maps**: Location embedding
- **WhatsApp API**: Direct messaging integration

## Deployment Strategy

### Build Process
- **Development**: `npm run dev` - Vite dev server with HMR
- **Production Build**: `npm run build` - Creates optimized production bundle
- **Database**: `npm run db:push` - Pushes schema changes to database

### Deployment Configuration
- **Platform**: Replit with autoscale deployment
- **Build Command**: `npm run build`
- **Start Command**: `npm run start`
- **Port**: 5000 (mapped to 80 externally)

### Environment Variables
- `DATABASE_URL`: PostgreSQL connection string (required)
- `NODE_ENV`: Environment setting (development/production)

### Performance Considerations
- Static asset caching (1 year for assets, 1 hour for HTML)
- Gzip compression for text assets
- Lazy loading for images and components
- Service worker for offline caching

## Changelog
- June 26, 2025. Added PostgreSQL database integration with Drizzle ORM - replaced in-memory storage with persistent database storage
- June 23, 2025. Initial setup

## User Preferences

Preferred communication style: Simple, everyday language.