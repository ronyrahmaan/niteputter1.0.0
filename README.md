# NitePutter Mobile Application

A premium React Native application for controlling LED golf cups and managing night golf experiences.

## Overview

NitePutter is an enterprise-grade mobile application built with React Native and Expo, designed to provide seamless control over LED golf equipment through Bluetooth connectivity. The application features a sophisticated user interface, real-time device management, e-commerce integration, and comprehensive user account functionality.

## Key Features

### Device Control
- **Bluetooth Low Energy (BLE) connectivity** for cup management
- **Real-time color customization** with advanced color picker
- **Multi-cup synchronization** and group control
- **Custom lighting modes** (static, pulse, strobe, rainbow)
- **Brightness and temperature controls**

### E-Commerce Platform
- **Integrated Stripe payment processing**
- **Product catalog** with detailed specifications
- **Shopping cart** with persistent storage
- **Order management** and tracking
- **Promotional code** system

### User Experience
- **Secure authentication** with persistent sessions
- **Comprehensive user profiles** with referral system
- **Real-time notifications** and announcements
- **Instructional video library**
- **Professional support system**

### Technical Excellence
- **TypeScript** for type safety
- **Zustand** for state management
- **Supabase** for backend services
- **Professional UI/UX** with themed components
- **Offline-first architecture** with data persistence

## Quick Start

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Expo CLI
- iOS Simulator or Android Emulator

### Installation

```bash
# Clone the repository
git clone https://github.com/your-org/niteputterappv6.git
cd niteputterappv6

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Start development server
npm start
```

### Development Commands

```bash
# Start Expo development server
npm start

# Run on iOS simulator
npm run ios

# Run on Android emulator
npm run android

# Run on web
npm run web

# Lint code
npm run lint

# Run tests
npm test

# TypeScript check
npm run typecheck
```

## Architecture

### Core Technologies
- **React Native** + **Expo** - Cross-platform mobile framework
- **TypeScript** - Type-safe JavaScript
- **Zustand** - Lightweight state management
- **React Navigation** - Navigation framework
- **Expo Router** - File-based routing

### Backend Integration
- **Supabase** - Database and authentication
- **Stripe** - Payment processing
- **SendGrid** - Email services
- **Expo Updates** - Over-the-air updates

### State Management
- Centralized stores for different domains (auth, shop, devices, etc.)
- Persistent storage using AsyncStorage
- Optimistic updates for better UX

## Environment Setup

Copy the environment template and configure:

```bash
cp .env.example .env
```

Required environment variables:
- `EXPO_PUBLIC_SUPABASE_URL` - Supabase project URL
- `EXPO_PUBLIC_SUPABASE_ANON_KEY` - Supabase anonymous key
- `STRIPE_PUBLISHABLE_KEY` - Stripe public key
- `SENDGRID_API_KEY` - SendGrid API key

## Project Structure

```
src/
├── components/         # Reusable UI components
│   ├── ui/            # Base UI components
│   └── forms/         # Form components
├── features/          # Feature-based modules
│   ├── auth/          # Authentication screens
│   ├── shop/          # E-commerce functionality
│   ├── niteControl/   # Device control features
│   └── profile/       # User profile management
├── store/             # Zustand state stores
├── lib/               # Utilities and services
│   ├── api/           # API integrations
│   ├── stripe/        # Payment processing
│   ├── supabase/      # Backend services
│   └── theme/         # Design system
├── hooks/             # Custom React hooks
└── types/             # TypeScript type definitions
```

## Contributing

This document provides guidelines and instructions for the project.

### Development Workflow

#### Branch Strategy
- `main` - Production-ready code
- `develop` - Integration branch for features
- `feature/*` - Individual feature development
- `hotfix/*` - Emergency fixes for production

#### Commit Convention
Follow conventional commit format:
```
type(scope): description

Examples:
feat(auth): add biometric authentication
fix(payment): resolve Stripe integration issue
docs(readme): update installation instructions
```

### Code Quality Standards

#### TypeScript
- Use strict TypeScript configuration
- Define proper types for all props and state
- Avoid `any` type usage
- Use meaningful interface and type names

#### React Native Best Practices
- Use functional components with hooks
- Implement proper error boundaries
- Follow React Native performance guidelines
- Use platform-specific code when necessary

#### State Management
- Use Zustand stores for global state
- Keep stores focused and modular
- Implement proper error handling
- Use optimistic updates where appropriate

### Testing Requirements

#### Unit Tests
- Write tests for all utility functions
- Test component logic and state changes
- Mock external dependencies
- Maintain minimum 70% code coverage

#### Integration Tests
- Test critical user flows
- Verify API integrations
- Test offline functionality
- Validate payment processing

#### E2E Tests
- Test complete user journeys
- Validate on real devices
- Test edge cases and error scenarios

### Pull Request Process

1. **Create Feature Branch**
```bash
git checkout develop
git pull origin develop
git checkout -b feature/your-feature-name
```

2. **Develop and Test**
- Write code following established patterns
- Add comprehensive tests
- Update documentation as needed
- Ensure all checks pass locally

3. **Pre-commit Checks**
```bash
npm run lint
npm run typecheck
npm test
```

4. **Submit Pull Request**
- Fill out PR template completely
- Link related issues
- Request appropriate reviewers
- Ensure CI checks pass

### Review Criteria

#### Code Review Checklist
- [ ] Code follows established patterns
- [ ] TypeScript types are properly defined
- [ ] Tests cover new functionality
- [ ] Documentation is updated
- [ ] No security vulnerabilities
- [ ] Performance considerations addressed
- [ ] Accessibility requirements met

#### Design Review
- [ ] UI matches design specifications
- [ ] Responsive design works on all devices
- [ ] Animations are smooth and purposeful
- [ ] Loading states are handled gracefully
- [ ] Error states provide clear feedback

## Performance Guidelines

### React Native Performance
- Use FlatList for large lists
- Implement proper image optimization
- Avoid inline styles and functions
- Use React.memo for expensive components

### Bundle Size Management
- Import only needed modules
- Use tree shaking for large libraries
- Optimize images and assets
- Monitor bundle size in CI

### Memory Management
- Clean up subscriptions in useEffect
- Avoid memory leaks in async operations
- Optimize image loading and caching
- Profile app performance regularly

## Security Considerations

### Data Protection
- Never commit sensitive credentials
- Use environment variables for secrets
- Implement proper input validation
- Follow OWASP mobile security guidelines

### API Security
- Use HTTPS for all communications
- Implement proper authentication
- Validate all API responses
- Handle errors securely

## Deployment

### Development Previews
```bash
# Create preview build
expo build:preview

# Publish to Expo
expo publish
```

### Production Builds
```bash
# iOS production build
expo build:ios --release-channel production

# Android production build
expo build:android --release-channel production
```

### Release Process
1. Create release branch from develop
2. Update version numbers and changelog
3. Run full test suite
4. Deploy to staging for verification
5. Create release tag
6. Deploy to production
7. Monitor for issues

## Getting Help

### Resources
- [React Native Documentation](https://reactnative.dev/)
- [Expo Documentation](https://docs.expo.dev/)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [Zustand Documentation](https://github.com/pmndrs/zustand)

## License

Proprietary software. All rights reserved.