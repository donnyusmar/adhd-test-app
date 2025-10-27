# Template Prompt untuk Pengembangan Software Modular dengan GitHub

## 📋 Overview Template

Template ini adalah framework universal untuk mengembangkan aplikasi web modern dengan pendekatan modular yang dapat diterapkan pada berbagai jenis software. Template dirancang untuk memaksimalkan efisiensi Perplexity Labs dan memastikan hasil production-ready.

## 🎯 Cara Menggunakan Template

### Langkah 1: Definisi Project
Ganti placeholders berikut dengan spesifikasi project Anda:

- `[PROJECT_NAME]` = Nama aplikasi Anda
- `[PROJECT_DESCRIPTION]` = Deskripsi singkat aplikasi
- `[TECH_STACK]` = Stack teknologi yang dipilih
- `[DATABASE_TYPE]` = Jenis database (Supabase/Firebase/MongoDB)
- `[MAIN_FEATURES]` = Fitur utama aplikasi
- `[USER_TYPES]` = Jenis pengguna (admin, user biasa, dll)
- `[INTEGRATION_SERVICES]` = Layanan eksternal yang dibutuhkan

### Langkah 2: Sesuaikan Jumlah Prompt
Template default menggunakan 8 prompt modular. Anda dapat:
- Menambah prompt untuk aplikasi kompleks (maksimal 12)
- Mengurangi prompt untuk aplikasi sederhana (minimal 5)
- Menyesuaikan dependencies antar prompt

---

## 🏗️ TEMPLATE PROMPT SERIES

### Prompt 1: Project Setup & Database Configuration

```
Create a [TECH_STACK] [PROJECT_NAME] application setup with the following specifications:

1. Initialize [TECH_STACK] project with TypeScript
2. Set up free online database ([DATABASE_TYPE]) configuration
3. Create database schema for:
   - [Define your main tables here based on project needs]
   - Example: Users table (id, name, email, role, created_at)
   - Example: [Main_Entity] table (id, user_id, data_fields, created_at)
   - Example: [Secondary_Entity] table (id, related_id, metadata, created_at)

4. Install required dependencies:
   - Authentication libraries
   - Database ORM (Prisma or similar)
   - UI components (Tailwind CSS/Material-UI/Chakra UI)
   - [Integration service libraries]
   - [Additional specific libraries for your project]

5. Create environment variables template
6. Set up basic folder structure with modular architecture

Provide complete setup instructions, package.json, and database schema files.
```

### Prompt 2: Authentication & User Management System

```
Create a comprehensive authentication system for the [PROJECT_NAME] app with:

1. User Registration:
   - Form with [specify required fields based on your project]
   - [User verification method - email/phone/etc]
   - [User role assignment logic]
   - [Welcome email/notification system]

2. [OAuth Integration if needed]:
   - [Google/GitHub/Facebook] OAuth 2.0 integration
   - [Additional data collection after OAuth]
   - [Account linking functionality]

3. Login System:
   - [Authentication method - email/username/phone]
   - [Multi-role login if applicable]
   - Session management with JWT
   - Password reset functionality

4. Security & Privacy Components:
   - Privacy policy statement component
   - Data protection compliance notice
   - [GDPR/specific compliance requirements]

5. Responsive Design:
   - Mobile-optimized forms
   - Clean, accessible UI
   - Loading states and error handling

Create all authentication components, API routes, and middleware. Include email templates and security best practices.
```

### Prompt 3: Core Feature Implementation - [MAIN_FEATURE_1]

```
Develop the core [MAIN_FEATURE_1] functionality:

1. [Feature] Interface Design:
   - [Specific UI requirements]
   - [User flow description]
   - [Input validation requirements]
   - [Progress tracking if applicable]

2. [Feature] Logic Implementation:
   - [Core algorithm/business logic]
   - [Data processing requirements]
   - [Validation and error handling]
   - [Performance optimization needs]

3. [Feature] User Experience:
   - Mobile and desktop optimized
   - Clean, intuitive design
   - [Progress indicators if needed]
   - [Save/resume functionality if applicable]

4. [Feature] Data Management:
   - [Data storage strategy]
   - [Data retrieval optimization]
   - [Data export/import if needed]
   - [Backup and recovery considerations]

5. Offline Capability (if applicable):
   - Service worker implementation
   - Local storage for [specific data]
   - Sync when online

Provide complete [feature] component, business logic, and data management functionality.
```

### Prompt 4: User Dashboard & Data Visualization

```
Create a comprehensive user dashboard for [PROJECT_NAME]:

1. Main Dashboard:
   - [Key metrics/data display]
   - [Date/time-based information]
   - Interactive charts and graphs showing:
     * [Specific metric 1]
     * [Specific metric 2] 
     * [Comparison data]
     * [Historical trends]

2. Detailed Data Analysis:
   - [Data interpretation logic]
   - [Insights generation]
   - [Personalized recommendations]
   - Clear, user-friendly explanations

3. Export Features:
   - Download data as [format - PDF/CSV/Excel]
   - [Report generation with specific content]
   - Print-friendly formatting
   - Email sharing option

4. [External Service Integration]:
   - Direct link to [service/platform]
   - [Pre-formatted communication templates]
   - [API integration for data sharing]

5. Responsive Design:
   - Mobile-optimized charts
   - Touch-friendly interactions
   - Fast loading graphics

Create dashboard components, chart generation, export functionality, and external service integration.
```

### Prompt 5: Admin Panel & Management System

```
Develop the admin panel for [PROJECT_NAME] management:

1. Admin Authentication:
   - Secure admin login system
   - Role-based access control
   - Admin session management
   - [Multi-level admin roles if needed]

2. [Entity] Management Interface:
   - List all [entities] with [relevant data]
   - Search and pagination functionality
   - [Entity] details view with complete [related data]
   - Bulk operations for [specific actions]

3. Advanced Filtering & Analytics:
   - Filter by [relevant criteria]
   - Filter by [date ranges/categories]
   - Filter by [user demographics/behavior]
   - Custom filter combinations
   - Export filtered results

4. [Entity] Management Operations:
   - Add new [entities]
   - Edit existing [entity data]
   - Delete [entities] (with confirmation)
   - [Specific bulk operations]

5. Analytics Dashboard:
   - [Key business metrics]
   - [Usage statistics charts]
   - [Performance indicators]
   - [Trend analysis graphs]

Create admin components, filtering system, and data management functionality with proper security measures.
```

### Prompt 6: [Advanced Feature] - Automation/AI System

```
Implement an intelligent [automation/AI feature] system:

1. Automated [Process] Generation:
   - [AI/Algorithm] that analyzes [input data]
   - Generate [outputs] based on:
     * [Criteria 1]
     * [Criteria 2]
     * [User preferences/history]
     * [Latest industry standards/research]

2. [Feature] Database:
   - Comprehensive [content] library
   - [Evidence-based/rule-based] [content]
   - Categorized by [relevant categories]
   - Regular updates with [latest information]

3. Admin [Feature] Management:
   - View auto-generated [content]
   - Edit and customize [content]
   - Add manual [content]
   - Delete inappropriate [content]
   - Approve/reject [automated suggestions]

4. [Feature] Integration:
   - Include [content] in user dashboard
   - [Export format] with [content]
   - Email [content] to users
   - Track [effectiveness/usage metrics]

5. [Research/Standards] Integration:
   - Latest [industry] guidelines
   - [Evidence-based] recommendations
   - [Professional standards] compliance
   - [Best practices] implementation

Create the [automation/AI] engine, admin management interface, and integration with existing dashboard.
```

### Prompt 7: UI/UX Enhancement & Performance Optimization

```
Enhance the [PROJECT_NAME] application with advanced UI/UX and performance optimizations:

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

4. Progressive Web App (PWA) Features:
   - Service worker for caching
   - Offline functionality for [specific features]
   - App-like installation capability
   - Push notifications (if applicable)
   - Background sync

5. Error Handling & User Feedback:
   - Comprehensive error boundaries
   - User-friendly error messages
   - Success notifications
   - Loading states
   - Form validation feedback

Create enhanced components, PWA configuration, and performance optimization code.
```

### Prompt 8: Production Deployment & Integration

```
Complete the [PROJECT_NAME] application with final integration and production readiness:

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
   - [Deployment platform] configuration
   - Database hosting setup (production)
   - Environment-specific configurations
   - Monitoring and logging setup

4. Documentation:
   - User manual for [admin/user] features
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
   - [Go-live communication plan]

Provide complete production-ready code, deployment scripts, and comprehensive documentation for launch.
```

---

## 🔄 TEMPLATE DEPENDENCY STRUCTURE

### Layer 1: Foundation (Prompt 1)
- **No Dependencies**
- Sets up: Project structure, database, environment

### Layer 2: Authentication (Prompt 2)  
- **Depends on**: Prompt 1
- Sets up: User management, security, sessions

### Layer 3: Core Features (Prompt 3)
- **Depends on**: Prompt 1, 2
- Sets up: Main application functionality

### Layer 4: User Interface (Prompt 4)
- **Depends on**: Prompt 1, 2, 3
- Sets up: Dashboard, visualization, exports

### Layer 5: Admin Management (Prompt 5)
- **Depends on**: Prompt 1, 2
- Sets up: Admin panel, management tools

### Layer 6: Advanced Features (Prompt 6)
- **Depends on**: Prompt 1-5
- Sets up: AI/automation, advanced functionality

### Layer 7: Optimization (Prompt 7)
- **Depends on**: Prompt 1-6
- Sets up: Performance, UX, PWA features

### Layer 8: Production (Prompt 8)
- **Depends on**: Prompt 1-7
- Sets up: Deployment, testing, documentation

---

## 🛠️ TEMPLATE CUSTOMIZATION GUIDE

### For Simple Applications (5 Prompts):
1. Foundation & Auth (merge Prompt 1+2)
2. Core Features (Prompt 3)
3. User Interface (Prompt 4)
4. Admin Panel (Prompt 5)
5. Production (merge Prompt 7+8)

### For Complex Applications (12 Prompts):
1. Project Setup
2. Database & Models
3. Authentication
4. Core Feature 1
5. Core Feature 2
6. User Dashboard
7. Admin Panel
8. Advanced Feature 1
9. Advanced Feature 2
10. API & Integrations
11. UI/UX & Performance
12. Testing & Deployment

### Customization Parameters:

**Technology Stack Options:**
- Frontend: Next.js, React, Vue.js, Angular, Svelte
- Backend: Node.js, Python/Django, Ruby/Rails, PHP/Laravel
- Database: Supabase, Firebase, MongoDB, PostgreSQL, MySQL
- Styling: Tailwind CSS, Material-UI, Chakra UI, Styled Components

**Feature Categories:**
- E-commerce: Products, Cart, Payment, Inventory
- SaaS: Subscriptions, Billing, Usage Analytics, API Management
- Social: Posts, Comments, Messaging, Notifications
- Analytics: Data Collection, Processing, Visualization, Reporting
- Educational: Courses, Assessments, Progress Tracking, Certificates

---

## 📁 GITHUB INTEGRATION TEMPLATE

### Repository Structure Template:
```
[project-name]/
├── docs/
│   ├── prompts/
│   │   └── development-prompts.md
│   ├── dependencies/
│   │   └── dependency-diagram.md
│   └── guides/
│       └── development-guide.md
├── src/
│   ├── [framework-structure]/
│   ├── components/
│   ├── lib/
│   ├── hooks/
│   └── types/
├── public/
├── [database-folder]/
├── deployment/
├── README.md
├── .gitignore
└── [config-files]
```

### GitHub Setup Commands:
```bash
# 1. Create repository on GitHub
# 2. Clone locally
git clone https://github.com/[username]/[project-name].git
cd [project-name]

# 3. Add documentation files
# 4. Commit initial structure
git add .
git commit -m "feat: initial project structure and documentation"
git push origin main

# 5. Development workflow
# After each prompt completion:
git add .
git commit -m "feat: complete prompt X - [feature description]"
git push origin main
```

---

## 🎯 USAGE EXAMPLES

### Example 1: E-commerce Platform
```
PROJECT_NAME = "ShopEasy"
TECH_STACK = "Next.js"
DATABASE_TYPE = "Supabase"
MAIN_FEATURES = "Product catalog, Shopping cart, Payment processing"
USER_TYPES = "Customers, Vendors, Admins"
INTEGRATION_SERVICES = "Stripe, SendGrid, WhatsApp"
```

### Example 2: Learning Management System
```
PROJECT_NAME = "EduPlatform"
TECH_STACK = "React + Express"
DATABASE_TYPE = "MongoDB"
MAIN_FEATURES = "Course creation, Video lessons, Quiz system"
USER_TYPES = "Students, Instructors, Admins"
INTEGRATION_SERVICES = "Zoom, PayPal, YouTube API"
```

### Example 3: Project Management Tool
```
PROJECT_NAME = "TaskMaster"
TECH_STACK = "Vue.js + Laravel"
DATABASE_TYPE = "PostgreSQL"
MAIN_FEATURES = "Task tracking, Team collaboration, Time tracking"
USER_TYPES = "Team members, Project managers, Admins"
INTEGRATION_SERVICES = "Slack, Google Calendar, Jira"
```

---

## ✅ IMPLEMENTATION CHECKLIST

### Pre-Development:
- [ ] Define project requirements clearly
- [ ] Choose appropriate technology stack
- [ ] Customize prompts with project-specific details
- [ ] Set up GitHub repository
- [ ] Create project documentation structure

### Development Phase:
- [ ] Execute prompts sequentially (1-8)
- [ ] Test each module thoroughly
- [ ] Commit progress after each prompt
- [ ] Document any modifications or issues
- [ ] Maintain dependency tracking

### Post-Development:
- [ ] Complete integration testing
- [ ] Performance optimization
- [ ] Security audit
- [ ] Production deployment
- [ ] User acceptance testing
- [ ] Documentation finalization

---

## 🚀 SUCCESS METRICS

### Code Quality:
- TypeScript strict mode compliance
- Test coverage > 80%
- No critical security vulnerabilities
- Performance scores > 90

### Development Efficiency:
- Each prompt completed within estimated time
- Minimal rework between phases
- Clear dependency management
- Smooth integration between modules

### Production Readiness:
- All features functional
- Responsive design across devices
- Error handling comprehensive
- Documentation complete
- Deployment successful

---

**Template ini dapat diadaptasi untuk berbagai jenis aplikasi web modern. Sesuaikan placeholders dengan kebutuhan spesifik project Anda dan ikuti sequential development process untuk hasil optimal!**