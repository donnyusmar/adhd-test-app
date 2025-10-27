# Development Guide - ADHD Test Application

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ dan npm/yarn
- Git untuk version control
- Supabase account (free tier)
- Google Cloud Console account untuk OAuth
- Code editor (VS Code recommended)

### Installation Steps
1. Clone repository dari GitHub
2. Install dependencies dengan npm/yarn
3. Setup environment variables
4. Configure database connection
5. Run development server

## 📁 Project Structure

```
adhd-test-app/
├── docs/                     # Documentation
│   ├── prompts/              # Development prompts
│   ├── dependencies/         # Dependency diagrams
│   └── guides/               # Development guides
├── src/
│   ├── app/                  # Next.js 14 App Router
│   │   ├── (auth)/           # Authentication routes
│   │   ├── (dashboard)/      # User dashboard
│   │   ├── (admin)/          # Admin panel
│   │   ├── api/              # API routes
│   │   └── globals.css       # Global styles
│   ├── components/           # Reusable components
│   │   ├── auth/             # Auth components
│   │   ├── test/             # Test components
│   │   ├── dashboard/        # Dashboard components
│   │   ├── admin/            # Admin components
│   │   └── ui/               # UI components
│   ├── lib/                  # Utilities
│   │   ├── auth.ts           # Auth configuration
│   │   ├── database.ts       # Database client
│   │   ├── validations.ts    # Form validations
│   │   └── utils.ts          # Helper functions
│   ├── hooks/                # Custom React hooks
│   │   ├── useAuth.ts        # Authentication hook
│   │   ├── useTest.ts        # Test management hook
│   │   └── useAdmin.ts       # Admin functionality hook
│   └── types/                # TypeScript definitions
│       ├── auth.ts           # Auth types
│       ├── test.ts           # Test types
│       └── database.ts       # Database types
├── public/                   # Static assets
│   ├── icons/                # App icons
│   └── images/               # Images
├── database/                 # Database related
│   ├── migrations/           # DB migrations
│   └── seeds/                # Sample data
└── deployment/               # Deployment configs
    ├── vercel.json           # Vercel configuration
    └── docker/               # Docker files (optional)
```

## 🚀 Development Phases

### Phase 1: Foundation Setup
**Objective**: Establish project foundation
**Duration**: 2-3 days

**Tasks**:
- [x] Next.js project initialization
- [ ] Supabase database setup
- [ ] Environment variables configuration
- [ ] Basic folder structure
- [ ] Dependencies installation

**Key Files to Create**:
- `package.json` with all required dependencies
- `next.config.js` with optimizations
- `.env.example` template
- `lib/database.ts` for Supabase client
- Database schema SQL files

### Phase 2: Authentication System
**Objective**: Complete user authentication
**Duration**: 2-3 days

**Tasks**:
- [ ] User registration form
- [ ] Google OAuth 2.0 integration
- [ ] Email verification system
- [ ] Session management
- [ ] Privacy policy components

**Key Files to Create**:
- `lib/auth.ts` - Authentication logic
- `components/auth/` - Auth UI components
- `app/api/auth/` - Auth API routes
- `middleware.ts` - Route protection

### Phase 3: ADHD Test Implementation
**Objective**: Core testing functionality
**Duration**: 3-4 days

**Tasks**:
- [ ] DSM-5 based questionnaire
- [ ] Test flow and validation
- [ ] Scoring algorithm
- [ ] Offline capability
- [ ] Progress tracking

**Key Files to Create**:
- `components/test/` - Test UI components
- `lib/scoring.ts` - Scoring algorithms
- `types/test.ts` - Test type definitions
- `hooks/useTest.ts` - Test state management

### Phase 4: User Dashboard
**Objective**: Results visualization and exports
**Duration**: 3-4 days

**Tasks**:
- [ ] Results display with charts
- [ ] PDF export functionality
- [ ] WhatsApp integration
- [ ] Historical data view
- [ ] Mobile optimization

**Key Files to Create**:
- `components/dashboard/` - Dashboard components
- `lib/charts.ts` - Chart configurations
- `lib/pdf-export.ts` - PDF generation
- `lib/whatsapp.ts` - WhatsApp integration

### Phase 5: Admin Panel
**Objective**: Administrative functionality
**Duration**: 2 days

**Tasks**:
- [ ] User management interface
- [ ] Advanced filtering
- [ ] Test CRUD operations
- [ ] Analytics dashboard
- [ ] Data visualization

**Key Files to Create**:
- `components/admin/` - Admin UI components
- `app/(admin)/` - Admin route group
- `hooks/useAdmin.ts` - Admin functionality
- `lib/analytics.ts` - Analytics logic

### Phase 6: AI Solution System
**Objective**: Intelligent recommendations
**Duration**: 2-3 days

**Tasks**:
- [ ] Solution generation algorithm
- [ ] Evidence-based recommendations
- [ ] Admin solution management
- [ ] Research integration
- [ ] Solution tracking

**Key Files to Create**:
- `lib/ai-solutions.ts` - AI recommendation engine
- `components/solutions/` - Solution UI components
- `database/solutions-data.ts` - Solution database

### Phase 7: UI/UX Enhancement
**Objective**: Performance and user experience
**Duration**: 2 days

**Tasks**:
- [ ] Design system implementation
- [ ] Mobile optimization
- [ ] Performance tuning
- [ ] PWA setup
- [ ] Accessibility compliance

**Key Files to Create**:
- `components/ui/` - Design system components
- `public/sw.js` - Service worker
- `styles/` - Enhanced styling
- `lib/pwa.ts` - PWA configuration

### Phase 8: Production Deployment
**Objective**: Production readiness
**Duration**: 1-2 days

**Tasks**:
- [ ] Final integration testing
- [ ] Production configuration
- [ ] Deployment setup
- [ ] Documentation completion
- [ ] Performance monitoring

**Key Files to Create**:
- `deployment/` - Deployment configurations
- `docs/api/` - API documentation
- Production environment files

## 🛠️ Development Guidelines

### Code Standards
- **TypeScript**: Strict typing untuk semua components
- **ESLint + Prettier**: Consistent code formatting
- **Conventional Commits**: Semantic commit messages
- **Component Structure**: Functional components dengan hooks

### Testing Strategy
- **Unit Tests**: Jest untuk utility functions
- **Component Tests**: React Testing Library
- **E2E Tests**: Playwright untuk critical user flows
- **Manual Testing**: Cross-browser dan mobile testing

### Performance Guidelines
- **Code Splitting**: Lazy loading untuk large components
- **Image Optimization**: Next.js Image component
- **Bundle Analysis**: Regular bundle size monitoring
- **Caching Strategy**: Proper cache headers dan service worker

### Security Considerations
- **Input Validation**: Client dan server-side validation
- **SQL Injection**: Parameterized queries via ORM
- **XSS Protection**: Sanitization untuk user inputs
- **Authentication**: Secure session management

## 🔧 Development Tools

### Recommended VS Code Extensions
```json
{
  "recommendations": [
    "bradlc.vscode-tailwindcss",
    "ms-vscode.vscode-typescript-next",
    "esbenp.prettier-vscode",
    "dbaeumer.vscode-eslint",
    "ms-playwright.playwright",
    "bradlc.vscode-tailwindcss"
  ]
}
```

### Package.json Scripts
```json
{
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint",
    "test": "jest",
    "test:watch": "jest --watch",
    "test:e2e": "playwright test",
    "type-check": "tsc --noEmit",
    "db:migrate": "supabase db push",
    "db:seed": "tsx database/seed.ts"
  }
}
```

## 🐛 Troubleshooting

### Common Issues

**1. Environment Variables Not Loading**
```bash
# Check .env.local file exists and has correct format
# Restart development server after env changes
npm run dev
```

**2. Database Connection Issues**
```bash
# Verify Supabase URL and anon key
# Check database migrations are applied
npm run db:migrate
```

**3. Build Failures**
```bash
# Clear Next.js cache
rm -rf .next
npm run build
```

**4. TypeScript Errors**
```bash
# Run type checking
npm run type-check
```

### Debug Configuration
```json
// .vscode/launch.json
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Next.js: debug server-side",
      "type": "node-terminal",
      "request": "launch",
      "command": "npm run dev"
    }
  ]
}
```

## 📈 Monitoring & Analytics

### Performance Monitoring
- **Vercel Analytics**: Built-in performance metrics
- **Core Web Vitals**: LCP, FID, CLS monitoring
- **Bundle Analyzer**: Regular size analysis

### Error Tracking
- **Sentry**: Production error monitoring
- **Console Logging**: Development debugging
- **User Feedback**: In-app feedback system

## 🚀 Deployment Checklist

### Pre-deployment
- [ ] All tests passing
- [ ] TypeScript compilation successful
- [ ] Environment variables configured
- [ ] Database migrations applied
- [ ] Performance optimization completed

### Production Environment
- [ ] Vercel deployment configured
- [ ] Custom domain setup
- [ ] SSL certificate active
- [ ] Error monitoring enabled
- [ ] Analytics tracking configured

### Post-deployment
- [ ] Smoke testing in production
- [ ] Performance metrics baseline
- [ ] Monitoring alerts configured
- [ ] Backup strategy implemented
- [ ] Documentation updated

---

## 🔗 Quick Links

- [Development Prompts](../prompts/adhd-app-prompts.md)
- [Dependency Diagram](../dependencies/dependency-diagram.md)
- [GitHub Repository](https://github.com/donnyusmar/adhd-test-app)
- [Supabase Dashboard](https://supabase.com/dashboard)
- [Vercel Dashboard](https://vercel.com/dashboard)

## 🤝 Contributing

1. Fork repository
2. Create feature branch
3. Follow development phases
4. Test thoroughly
5. Submit pull request
6. Code review process
7. Merge ke main branch

**Happy Coding! 🚀**