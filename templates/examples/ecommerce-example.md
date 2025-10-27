# Contoh Implementasi: E-commerce Platform "ShopEasy"

## 📋 Project Definition

```
PROJECT_NAME = "ShopEasy"
PROJECT_DESCRIPTION = "Platform e-commerce modern dengan fitur lengkap untuk toko online"
TECH_STACK = "Next.js 14 + TypeScript"
DATABASE_TYPE = "Supabase"
MAIN_FEATURES = "Product catalog, Shopping cart, Payment processing, Order management"
USER_TYPES = "Customers, Vendors, Store Admins, Super Admins"
INTEGRATION_SERVICES = "Stripe, SendGrid, WhatsApp, Google Maps, Midtrans"
```

---

## 🚀 Customized Prompt Series untuk ShopEasy

### Prompt 1: Project Setup & Database Configuration

```
Create a Next.js 14 ShopEasy e-commerce platform setup with the following specifications:

1. Initialize Next.js project with TypeScript and App Router
2. Set up Supabase database configuration for e-commerce
3. Create database schema for:
   - Users table (id, name, email, password_hash, phone, role, address, created_at)
   - Products table (id, vendor_id, name, description, price, stock, category_id, images, created_at)
   - Categories table (id, name, slug, description, parent_id)
   - Orders table (id, customer_id, total_amount, status, shipping_address, created_at)
   - Order_items table (id, order_id, product_id, quantity, price)
   - Shopping_carts table (id, user_id, product_id, quantity, created_at)
   - Reviews table (id, product_id, user_id, rating, comment, created_at)

4. Install required dependencies:
   - NextAuth.js for authentication
   - Prisma ORM for database
   - Tailwind CSS + Headless UI
   - Stripe SDK for payments
   - Resend for email service
   - React Hook Form + Zod validation
   - Zustand for state management

5. Create environment variables template
6. Set up e-commerce folder structure with modular architecture

Provide complete setup instructions, package.json, and database schema files.
```

### Prompt 2: Authentication & User Management System

```
Create a comprehensive authentication system for ShopEasy e-commerce with:

1. Multi-Role User Registration:
   - Customer registration form (name, email, password, phone, shipping address)
   - Vendor registration form (business info, tax details, bank account)
   - Email verification system
   - Welcome email with account details

2. Google OAuth 2.0 Integration:
   - Google sign-in for customers
   - Additional profile completion after OAuth
   - Account linking functionality

3. Multi-Level Login System:
   - Customer login portal
   - Vendor dashboard login
   - Admin panel login
   - Role-based redirect after login
   - Password reset functionality

4. Security & Privacy Components:
   - E-commerce privacy policy component
   - GDPR compliance for customer data
   - Cookie consent management

5. Responsive Design:
   - Mobile-first registration/login forms
   - Clean, trustworthy UI design
   - Loading states and error handling
   - Social proof elements

Create all authentication components, API routes, and middleware. Include email templates and e-commerce security best practices.
```

### Prompt 3: Product Management & Catalog System

```
Develop the core product management functionality for ShopEasy:

1. Product Catalog Interface:
   - Grid and list view options
   - Advanced filtering (price, category, rating, brand)
   - Search functionality with autocomplete
   - Product sorting options

2. Product Management Logic:
   - CRUD operations for products
   - Image upload and optimization
   - Inventory tracking system
   - Category management hierarchy
   - Bulk product operations

3. Product Display Experience:
   - Responsive product cards
   - Quick view functionality
   - Product image gallery
   - Related products suggestions
   - Recently viewed products

4. Vendor Product Management:
   - Vendor dashboard for product listing
   - Sales analytics per product
   - Stock management tools
   - Product performance insights

5. SEO and Performance:
   - Product page SEO optimization
   - Image lazy loading
   - Product data caching
   - Search indexing

Provide complete product management system, vendor tools, and customer catalog interface.
```

### Prompt 4: Shopping Cart & Checkout System

```
Create a comprehensive shopping cart and checkout system for ShopEasy:

1. Shopping Cart Features:
   - Add to cart functionality
   - Cart persistence (logged in users)
   - Quantity adjustments
   - Cart summary with calculations
   - Save for later functionality

2. Checkout Process:
   - Guest and registered checkout
   - Multi-step checkout form
   - Shipping address management
   - Shipping options and calculations
   - Tax calculations

3. Payment Integration:
   - Stripe payment processing
   - Midtrans for Indonesian market
   - Multiple payment methods (card, bank transfer, e-wallet)
   - Payment security and validation
   - Payment confirmation emails

4. Order Management:
   - Order confirmation system
   - Order tracking functionality
   - Order history for customers
   - Invoice generation (PDF)

5. Mobile Optimization:
   - Touch-optimized cart interface
   - Mobile payment optimization
   - One-click checkout options

Create cart system, payment processing, order management, and mobile-optimized checkout flow.
```

### Prompt 5: Admin & Vendor Management Panel

```
Develop comprehensive admin and vendor management panels for ShopEasy:

1. Multi-Level Admin Authentication:
   - Super admin access control
   - Store admin permissions
   - Vendor panel access
   - Role-based feature restrictions

2. Product & Inventory Management:
   - All products overview with filters
   - Bulk product operations
   - Inventory alerts and reports
   - Category management system
   - Product approval workflow for vendors

3. Order & Customer Management:
   - Order processing workflow
   - Customer support tools
   - Refund and return management
   - Customer analytics and segmentation
   - Bulk order operations

4. Vendor Management:
   - Vendor onboarding approval
   - Commission and payout management
   - Vendor performance analytics
   - Vendor communication tools

5. Sales Analytics Dashboard:
   - Revenue and sales metrics
   - Product performance analytics
   - Customer behavior insights
   - Vendor performance comparison
   - Financial reporting tools

Create admin interfaces, vendor management system, and comprehensive analytics dashboard with proper security measures.
```

### Prompt 6: AI-Powered Recommendation & Marketing System

```
Implement intelligent recommendation and marketing automation for ShopEasy:

1. AI Product Recommendation Engine:
   - Collaborative filtering for "customers also bought"
   - Content-based recommendations
   - Personalized product suggestions based on:
     * Purchase history
     * Browsing behavior
     * Similar customer profiles
     * Seasonal trends

2. Marketing Automation Database:
   - Customer segmentation rules
   - Email marketing campaigns
   - Abandoned cart recovery
   - Personalized discount offers
   - Cross-selling and upselling suggestions

3. Admin Marketing Management:
   - Campaign creation and management
   - A/B testing for recommendations
   - Performance tracking and analytics
   - Customer journey mapping
   - ROI analysis for marketing activities

4. Customer Experience Integration:
   - Personalized homepage
   - Smart search with suggestions
   - Dynamic pricing strategies
   - Loyalty program integration

5. Analytics & Insights:
   - Recommendation effectiveness tracking
   - Customer lifetime value calculation
   - Marketing attribution analysis
   - Conversion funnel optimization

Create AI recommendation engine, marketing automation system, and comprehensive analytics integration.
```

### Prompt 7: UI/UX Enhancement & Performance Optimization

```
Enhance ShopEasy e-commerce platform with advanced UI/UX and performance optimizations:

1. E-commerce Design System:
   - Modern, trustworthy e-commerce design
   - Consistent product card layouts
   - Professional checkout design
   - Trust badges and security indicators
   - Accessibility compliance for shopping

2. Mobile-First E-commerce:
   - Touch-optimized product browsing
   - Mobile-friendly cart and checkout
   - Swipe gestures for product images
   - Mobile payment optimization
   - App-like shopping experience

3. Performance Optimization:
   - Product image optimization and CDN
   - Lazy loading for product catalogs
   - Shopping cart state optimization
   - Database query optimization for products
   - Caching strategies for product data

4. PWA E-commerce Features:
   - Offline product browsing
   - Add to cart offline functionality
   - Push notifications for orders
   - App installation prompts
   - Background sync for cart data

5. Conversion Optimization:
   - Loading state optimizations
   - Error handling for payments
   - Success feedback for purchases
   - Cart abandonment prevention
   - Social proof integration

Create enhanced e-commerce components, PWA configuration, and conversion-focused optimizations.
```

### Prompt 8: Production Deployment & E-commerce Integration

```
Complete ShopEasy e-commerce platform with final integration and production readiness:

1. E-commerce Integration Testing:
   - End-to-end purchase flow testing
   - Payment gateway testing
   - Order fulfillment workflow testing
   - Multi-vendor functionality testing

2. Production E-commerce Configuration:
   - Payment gateway production keys
   - Email service production setup
   - SSL certificate for secure transactions
   - CDN configuration for product images

3. E-commerce Deployment:
   - Vercel deployment with e-commerce optimization
   - Supabase production database
   - Domain setup with SSL
   - Performance monitoring for e-commerce metrics

4. E-commerce Documentation:
   - Vendor onboarding guide
   - Customer user manual
   - Admin panel documentation
   - API documentation for integrations

5. Launch Preparation:
   - Payment processing testing
   - Security audit for transactions
   - GDPR compliance verification
   - Performance testing under load
   - Customer support system setup

6. E-commerce Launch Checklist:
   - Product catalog verification
   - Payment gateway testing
   - Order fulfillment workflow
   - Customer communication templates
   - Legal compliance verification

Provide complete production-ready e-commerce platform, deployment scripts, and comprehensive launch documentation.
```

---

## 📁 Struktur Database E-commerce

```sql
-- Users (Multi-role: customer, vendor, admin)
CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  name VARCHAR NOT NULL,
  email VARCHAR UNIQUE NOT NULL,
  password_hash VARCHAR,
  phone VARCHAR,
  role VARCHAR DEFAULT 'customer',
  is_verified BOOLEAN DEFAULT false,
  created_at TIMESTAMP DEFAULT NOW()
);

-- Customer profiles
CREATE TABLE customer_profiles (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  user_id UUID REFERENCES users(id),
  shipping_address JSONB,
  billing_address JSONB,
  preferences JSONB
);

-- Vendor profiles
CREATE TABLE vendor_profiles (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  user_id UUID REFERENCES users(id),
  business_name VARCHAR NOT NULL,
  business_address JSONB,
  tax_id VARCHAR,
  bank_details JSONB,
  commission_rate DECIMAL DEFAULT 0.1,
  is_approved BOOLEAN DEFAULT false
);

-- Categories
CREATE TABLE categories (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  name VARCHAR NOT NULL,
  slug VARCHAR UNIQUE NOT NULL,
  description TEXT,
  parent_id UUID REFERENCES categories(id),
  image_url VARCHAR
);

-- Products
CREATE TABLE products (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  vendor_id UUID REFERENCES users(id),
  name VARCHAR NOT NULL,
  description TEXT,
  price DECIMAL NOT NULL,
  stock INTEGER DEFAULT 0,
  category_id UUID REFERENCES categories(id),
  images JSONB,
  specifications JSONB,
  is_active BOOLEAN DEFAULT true,
  created_at TIMESTAMP DEFAULT NOW()
);

-- Shopping carts
CREATE TABLE shopping_carts (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  user_id UUID REFERENCES users(id),
  product_id UUID REFERENCES products(id),
  quantity INTEGER NOT NULL,
  created_at TIMESTAMP DEFAULT NOW()
);

-- Orders
CREATE TABLE orders (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  customer_id UUID REFERENCES users(id),
  total_amount DECIMAL NOT NULL,
  status VARCHAR DEFAULT 'pending',
  shipping_address JSONB,
  payment_method VARCHAR,
  payment_status VARCHAR DEFAULT 'pending',
  created_at TIMESTAMP DEFAULT NOW()
);

-- Order items
CREATE TABLE order_items (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  order_id UUID REFERENCES orders(id),
  product_id UUID REFERENCES products(id),
  vendor_id UUID REFERENCES users(id),
  quantity INTEGER NOT NULL,
  price DECIMAL NOT NULL
);

-- Reviews
CREATE TABLE reviews (
  id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
  product_id UUID REFERENCES products(id),
  customer_id UUID REFERENCES users(id),
  rating INTEGER CHECK (rating >= 1 AND rating <= 5),
  comment TEXT,
  created_at TIMESTAMP DEFAULT NOW()
);
```

## 🛠️ Tech Stack Detail

### Frontend:
- **Next.js 14**: App Router, Server Components
- **TypeScript**: Strict typing
- **Tailwind CSS**: Styling dengan Headless UI
- **Zustand**: Global state management
- **React Hook Form**: Form handling
- **Zod**: Schema validation

### Backend & Database:
- **Supabase**: Database, Auth, Storage
- **Prisma**: ORM dan migrations
- **NextAuth.js**: Authentication
- **Stripe**: Payment processing
- **Resend**: Email service

### Deployment & DevOps:
- **Vercel**: Hosting dan deployment
- **GitHub**: Version control
- **Supabase**: Database hosting
- **Cloudinary**: Image storage dan optimization

## 🚀 Development Timeline

- **Week 1**: Setup + Auth (Prompt 1-2)
- **Week 2**: Product Management (Prompt 3)
- **Week 3**: Cart + Checkout (Prompt 4)
- **Week 4**: Admin Panel (Prompt 5)
- **Week 5**: AI Features (Prompt 6)
- **Week 6**: Optimization (Prompt 7)
- **Week 7**: Deployment (Prompt 8)

**Total**: 7 minggu untuk MVP e-commerce platform

---

**Template e-commerce ini memberikan foundation lengkap untuk membangun platform jual-beli modern dengan fitur multi-vendor, payment gateway, dan sistem manajemen yang comprehensive!**