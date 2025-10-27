# ADHD Test Application Development Prompts for Perplexity Labs

## Overview
This document contains a series of modular prompts designed to create a comprehensive ADHD testing web application using Next.js with online database integration. Each prompt is designed to stay within Perplexity Labs' capacity limits.

## Prompt Series Instructions

**Important Notes:**
- Execute prompts in order (1-8)
- Each prompt builds upon the previous one
- Wait for completion before proceeding to next prompt
- Save all generated code before moving to next module

---

## Prompt 1: Project Setup & Database Configuration

```
Create a Next.js ADHD testing application setup with the following specifications:

1. Initialize Next.js project with TypeScript
2. Set up free online database (Supabase or Firebase) configuration
3. Create database schema for:
   - Users table (id, name, age, gender, email, password_hash, phone, unique_code, created_at)
   - Tests table (id, user_id, questions_answers, result_score, severity_level, test_date)
   - Admin_solutions table (id, user_id, solution_text, created_by_admin, created_at)

4. Install required dependencies:
   - Authentication libraries
   - Database ORM (Prisma or similar)
   - UI components (Tailwind CSS)
   - Email service integration
   - PDF generation library

5. Create environment variables template
6. Set up basic folder structure with modular architecture

Provide complete setup instructions, package.json, and database schema files.
```

---

## Prompt 2: Authentication System

```
Create a comprehensive authentication system for the ADHD testing app with:

1. User Registration:
   - Form with name, age, gender, email, password, phone number
   - Generate unique user code
   - Email verification system
   - Send username/password via email

2. Google OAuth 2.0 Integration:
   - Google sign-in with additional phone number collection
   - Merge Google profile with local user data

3. Login System:
   - Email/password authentication
   - Admin login with separate credentials
   - Session management with JWT

4. Privacy & Security Components:
   - Privacy policy statement component
   - Data protection compliance notice
   - GDPR-compliant consent forms

5. Responsive Design:
   - Mobile-optimized forms
   - Clean, accessible UI
   - Loading states and error handling

Create all authentication components, API routes, and middleware. Include email templates and security best practices.
```

---

## Prompt 3: ADHD Test Interface & Logic

```
Develop the core ADHD testing functionality:

1. Pre-test Instructions:
   - Clear guidelines component
   - Emphasis on honest, authentic responses
   - Test duration and question count info

2. ADHD Test Questions:
   - Create comprehensive ADHD assessment questionnaire based on DSM-5 criteria
   - Include both hyperactivity and inattention questions
   - Implement scoring algorithm with severity levels
   - Progressive question flow with validation

3. Test Interface:
   - Mobile and desktop optimized
   - Clean, distraction-free design
   - Progress indicator
   - Save/resume functionality for offline capability

4. Scoring System:
   - Evidence-based scoring methodology
   - Severity level categorization (Normal, Mild, Moderate, Severe)
   - Detailed analysis based on latest ADHD research

5. Offline Capability:
   - Service worker implementation
   - Local storage for test progress
   - Sync when online

Provide complete test component, scoring logic, and offline functionality.
```

---

## Prompt 4: User Dashboard & Results Display

```
Create a comprehensive user dashboard for ADHD test results:

1. Results Dashboard:
   - Clear severity level display
   - Test completion date
   - Interactive graphs and charts showing:
     * Overall ADHD score
     * Hyperactivity vs Inattention breakdown
     * Comparison to normal ranges
     * Historical test results (if multiple tests)

2. Detailed Results Explanation:
   - Evidence-based interpretation of scores
   - Latest ADHD research integration
   - Personalized recommendations
   - Clear, non-medical language explanations

3. Export Features:
   - Download results as high-quality graphics
   - PDF report generation with detailed explanations
   - Print-friendly formatting
   - Email results option

4. WhatsApp Consultation Integration:
   - Direct link to WhatsApp (+6285123523484)
   - Pre-formatted consultation message with user code

5. Responsive Design:
   - Mobile-optimized charts
   - Touch-friendly interactions
   - Fast loading graphics

Create dashboard components, chart generation, PDF export functionality, and WhatsApp integration.
```

---

## Prompt 5: Admin Dashboard - User Management

```
Develop the admin dashboard for user and test management:

1. Admin Authentication:
   - Secure admin login system
   - Role-based access control
   - Admin session management

2. User Management Interface:
   - List all users with test results
   - Search and pagination functionality
   - User details view with complete test history

3. Advanced Filtering System:
   - Filter by severity levels
   - Filter by test date ranges
   - Filter by demographics (age, gender)
   - Custom filter combinations
   - Export filtered results

4. Test Management:
   - Add new tests for users
   - Edit existing test results
   - Delete test records (with confirmation)
   - Bulk operations

5. Data Visualization:
   - Admin analytics dashboard
   - User statistics charts
   - Test completion rates
   - Severity distribution graphs

Create admin components, filtering system, and data management functionality with proper security measures.
```

---

## Prompt 6: AI-Powered Solution System

```
Implement an intelligent solution recommendation system:

1. Automated Solution Generation:
   - AI algorithm that analyzes user test results
   - Generate personalized recommendations based on:
     * ADHD severity level
     * Specific symptom patterns
     * User demographics
     * Latest evidence-based treatments

2. Solution Database:
   - Comprehensive solution library
   - Evidence-based interventions
   - Categorized by severity and symptom type
   - Regular updates with latest research

3. Admin Solution Management:
   - View auto-generated solutions for each user
   - Edit and customize solutions
   - Add manual solutions
   - Delete inappropriate solutions
   - Approve/reject AI suggestions

4. Solution Integration:
   - Include solutions in user dashboard
   - PDF export with solutions
   - Email solutions to users
   - Track solution effectiveness

5. Research Integration:
   - Latest ADHD treatment guidelines
   - Evidence-based recommendations
   - Professional therapy suggestions
   - Lifestyle modification advice

Create the AI solution engine, admin management interface, and integration with existing dashboard.
```

---

## Prompt 7: UI/UX Enhancement & Performance Optimization

```
Enhance the application with advanced UI/UX and performance optimizations:

1. Advanced UI Components:
   - Clean, modern design system
   - Accessibility compliance (WCAG 2.1)
   - Consistent color scheme and typography
   - Smooth animations and transitions
   - Loading skeletons and states

2. Mobile Optimization:
   - Touch-optimized interactions
   - Responsive breakpoints
   - Mobile-first design approach
   - Gesture support for navigation
   - Optimized for various screen sizes

3. Performance Optimization:
   - Code splitting and lazy loading
   - Image optimization
   - Database query optimization
   - Caching strategies
   - Minification and compression

4. Offline Functionality Enhancement:
   - Progressive Web App (PWA) setup
   - Service worker for caching
   - Offline test completion
   - Data synchronization when online
   - Offline indicator

5. Error Handling & User Feedback:
   - Comprehensive error boundaries
   - User-friendly error messages
   - Success notifications
   - Loading states
   - Validation feedback

Create enhanced components, PWA configuration, and performance optimization code.
```

---

## Prompt 8: Final Integration & Production Deployment

```
Complete the application with final integration and production readiness:

1. Final Integration:
   - Connect all modules seamlessly
   - End-to-end testing scenarios
   - Data flow validation
   - Security audit and fixes

2. Production Configuration:
   - Environment variables for production
   - Database migration scripts
   - SSL certificate setup
   - CDN configuration for assets

3. Deployment Setup:
   - Vercel deployment configuration
   - Database hosting setup (production)
   - Environment-specific configurations
   - Monitoring and logging setup

4. Documentation:
   - User manual for admin features
   - API documentation
   - Deployment guide
   - Maintenance procedures

5. Final Testing & Quality Assurance:
   - Cross-browser compatibility
   - Mobile device testing
   - Load testing scenarios
   - Security penetration testing
   - User acceptance testing checklist

6. Launch Checklist:
   - Pre-launch verification steps
   - Backup procedures
   - Rollback plans
   - Performance monitoring setup

Provide complete production-ready code, deployment scripts, and comprehensive documentation for launch.
```

---

## Implementation Guidelines

### Order of Execution:
1. Execute prompts sequentially (1-8)
2. Test each module before proceeding
3. Save all generated code and documentation
4. Verify integrations at each step

### Best Practices:
- Always backup generated code
- Test functionality after each prompt
- Review security implementations carefully
- Validate database connections and queries
- Ensure responsive design on multiple devices

### Notes for Perplexity Labs:
- Each prompt is designed to stay within token limits
- Modular approach prevents system overload
- Sequential execution ensures proper dependencies
- Complete application will be production-ready

---

**Total Estimated Development Time:** 8 prompt sessions
**Expected Output:** Full-featured, production-ready ADHD testing web application