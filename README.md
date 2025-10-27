# ADHD Test Application - Next.js Modular Development

## 📋 Project Overview

Komprehensif aplikasi test ADHD yang dibangun dengan Next.js, menampilkan:
- ✅ Sistem registrasi dan login dengan Google OAuth 2.0
- ✅ Test ADHD berdasarkan standar DSM-5
- ✅ Dashboard hasil dengan visualisasi grafik
- ✅ Panel admin dengan manajemen pengguna
- ✅ Sistem rekomendasi AI berbasis hasil test
- ✅ Export PDF dan integrasi WhatsApp
- ✅ Mobile & desktop responsive
- ✅ Offline capability (PWA)

## 🏗️ Architecture Overview

### Tech Stack
- **Frontend**: Next.js 14+ with TypeScript
- **Database**: Supabase (Free tier)
- **Authentication**: NextAuth.js + Google OAuth
- **UI/UX**: Tailwind CSS + Headless UI
- **Charts**: Recharts/Chart.js
- **PDF Generation**: jsPDF/Puppeteer
- **Email**: Resend/SendGrid
- **Deployment**: Vercel

### Database Schema
```sql
-- Users table
CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  name VARCHAR NOT NULL,
  age INTEGER NOT NULL,
  gender VARCHAR NOT NULL,
  email VARCHAR UNIQUE NOT NULL,
  password_hash VARCHAR,
  phone VARCHAR NOT NULL,
  unique_code VARCHAR UNIQUE NOT NULL,
  google_id VARCHAR,
  created_at TIMESTAMP DEFAULT NOW()
);

-- Tests table
CREATE TABLE tests (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  user_id UUID REFERENCES users(id),
  questions_answers JSONB NOT NULL,
  result_score INTEGER NOT NULL,
  severity_level VARCHAR NOT NULL,
  test_date TIMESTAMP DEFAULT NOW()
);

-- Admin solutions table
CREATE TABLE admin_solutions (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  user_id UUID REFERENCES users(id),
  solution_text TEXT NOT NULL,
  created_by_admin UUID REFERENCES users(id),
  created_at TIMESTAMP DEFAULT NOW()
);
```

## 🚀 Development Phases

Project ini dikembangkan dalam 8 fase modular yang saling tergantung:

### Phase 1: Project Setup & Database
- Next.js project initialization
- Supabase database configuration
- Dependencies installation
- Environment setup

### Phase 2: Authentication System
- User registration & login forms
- Google OAuth 2.0 integration
- Email verification system
- Privacy & security components

### Phase 3: ADHD Test Interface
- DSM-5 based questionnaire
- Progressive test flow
- Scoring algorithm implementation
- Offline capability

### Phase 4: User Dashboard
- Results visualization with charts
- PDF export functionality
- WhatsApp consultation integration
- Historical test data

### Phase 5: Admin Dashboard
- User management interface
- Advanced filtering system
- Test CRUD operations
- Analytics dashboard

### Phase 6: AI Solution System
- Automated solution generation
- Evidence-based recommendations
- Admin solution management
- Research integration

### Phase 7: UI/UX Enhancement
- Performance optimization
- Mobile responsiveness
- PWA implementation
- Accessibility compliance

### Phase 8: Production Deployment
- Final integration testing
- Production configuration
- Documentation completion
- Launch preparation

## 📁 Project Structure

```
adhd-test-app/
├── docs/                     # Documentation files
│   ├── prompts/              # Development prompts
│   ├── dependencies/         # Dependency diagrams
│   └── guides/               # Implementation guides
├── src/
│   ├── app/                  # Next.js App Router
│   ├── components/           # Reusable components
│   ├── lib/                  # Utilities and configurations
│   ├── hooks/                # Custom React hooks
│   └── types/                # TypeScript definitions
├── public/                   # Static assets
├── database/                 # Database migrations & seeds
└── deployment/               # Deployment configurations
```

## 🔧 Getting Started

### Prerequisites
- Node.js 18+
- npm or yarn
- Supabase account
- Google OAuth credentials

### Installation
1. Clone repository
2. Install dependencies
3. Configure environment variables
4. Set up database
5. Run development server

Detailed setup instructions akan tersedia setelah Phase 1 completion.

## 📚 Documentation

- [Development Prompts](./docs/prompts/adhd-app-prompts.md)
- [Dependency Diagram](./docs/dependencies/dependency-diagram.md)
- [API Documentation](./docs/api/) (Coming soon)
- [Deployment Guide](./docs/deployment/) (Coming soon)

## 🤝 Contributing

Project ini menggunakan pendekatan modular development:
1. Ikuti urutan development phases
2. Test setiap module sebelum lanjut
3. Dokumentasi setiap perubahan
4. Follow coding standards

## 📞 Contact & Support

- WhatsApp Consultation: +6285123523484
- Developer: [donnyusmar](https://github.com/donnyusmar)
- Issues: [GitHub Issues](https://github.com/donnyusmar/adhd-test-app/issues)

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

---

**Status**: 🚧 In Development
**Current Phase**: Ready for Phase 1 implementation
**Last Updated**: October 27, 2025