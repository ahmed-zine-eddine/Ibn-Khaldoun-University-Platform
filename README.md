# PFE – Ibn Khaldoun University Platform

Full-stack university management platform built With modern ChatBot & Multilingual Toxic Content Detection System 

## Structure

```
PFE/
├── frontend/   → React 19 + Tailwind CSS frontend
├── backend/    → Node.js + Express API server
├── ai-service/ → Python + FastAPI + uvicorn    
└── .github/    → CI / collaboration config
```

## Getting Started

### Frontend
```bash
cd frontend
npm install
npm start        # → http://localhost:3000
```

### Backend
```bash
cd backend
npm install
npm run dev      # → http://localhost:5000
```

## Collaboration

- **Never** commit `node_modules/` or `.env` files.
- Run `npm install` inside both `frontend/` and `backend/` after cloning.
- Create a `.env` file in `backend/` with `PORT=5000` (see `backend/README.md`).

See each folder's `README.md` for more details.

```
p_F_EF-univ-main
├─ Attached files will be deleted
│  └─ PFE-Consiel-Dicipline-main
│     └─ Discipline
│        ├─ discipline_ts
│        │  ├─ ADD_TO_app.ts.txt
│        │  └─ src
│        │     └─ modules
│        │        └─ discipline
│        │           ├─ controllers
│        │           │  ├─ conseil.controller.ts
│        │           │  ├─ decision.controller.ts
│        │           │  ├─ dossier.controller.ts
│        │           │  └─ infraction.controller.ts
│        │           ├─ index.ts
│        │           └─ routes
│        │              └─ discipline.routes.ts
│        └─ frontend_only
│           ├─ index.html
│           ├─ package-lock.json
│           ├─ package.json
│           ├─ src
│           │  ├─ App.jsx
│           │  ├─ main.jsx
│           │  └─ services
│           │     └─ api.js
│           └─ vite.config.js
├─ backend
│  ├─ package-lock.json
│  ├─ package.json
│  ├─ prisma
│  │  ├─ migrations
│  │  │  ├─ 20260309140906_init_41_tables
│  │  │  │  └─ migration.sql
│  │  │  ├─ 20260418000000_collapse_to_three_roles
│  │  │  │  └─ migration.sql
│  │  │  ├─ 20260418010000_add_alerts
│  │  │  │  └─ migration.sql
│  │  │  └─ migration_lock.toml
│  │  ├─ schema.prisma
│  │  ├─ schema.prisma.bak
│  │  ├─ schema.prisma.pre-refactor.bak
│  │  └─ seed.ts
│  ├─ prisma.config.ts
│  ├─ README.md
│  ├─ scripts
│  │  └─ apply-schema-compat.js
│  ├─ src
│  │  ├─ app.ts
│  │  ├─ config
│  │  │  ├─ auth.ts
│  │  │  ├─ database.ts
│  │  │  └─ env.ts
│  │  ├─ controllers
│  │  │  ├─ actualites
│  │  │  │  └─ actualites.controller.ts
│  │  │  ├─ admin
│  │  │  │  ├─ admin.controller.ts
│  │  │  │  └─ audit.controller.ts
│  │  │  ├─ affectation
│  │  │  │  └─ affectation.controller.ts
│  │  │  ├─ ai
│  │  │  │  └─ ai.controller.ts
│  │  │  ├─ alerts
│  │  │  │  └─ alerts.controller.ts
│  │  │  ├─ annonces
│  │  │  │  └─ annonce.controller.ts
│  │  │  ├─ auth
│  │  │  │  └─ auth.controller.ts
│  │  │  ├─ copieRemise
│  │  │  │  └─ copiesRemise.controller.ts
│  │  │  ├─ dashboard
│  │  │  │  └─ teacher-dashboard.controller.ts
│  │  │  ├─ discipline
│  │  │  │  └─ discipline.controller.ts
│  │  │  ├─ documents
│  │  │  │  └─ documents.controller.ts
│  │  │  ├─ enseignants
│  │  │  │  └─ enseignants.controller.ts
│  │  │  ├─ pfe
│  │  │  │  ├─ pfe-group.controller.ts
│  │  │  │  └─ pfe.controller.ts
│  │  │  ├─ requests
│  │  │  │  └─ request.controller.ts
│  │  │  ├─ settings
│  │  │  │  └─ site-settings.controller.ts
│  │  │  ├─ student
│  │  │  │  └─ student.controller.ts
│  │  │  └─ teacher
│  │  │     └─ teacher.controller.ts
│  │  ├─ middlewares
│  │  │  ├─ annonces-upload.middleware.ts
│  │  │  ├─ auth.middleware.ts
│  │  │  ├─ documents-upload.middleware.ts
│  │  │  ├─ error.middleware.ts
│  │  │  ├─ permission.middleware.ts
│  │  │  ├─ rate-limit.middleware.ts
│  │  │  ├─ role.middleware.ts
│  │  │  ├─ site-settings-upload.middleware.ts
│  │  │  └─ upload.middleware.ts
│  │  ├─ modules
│  │  │  ├─ actualites
│  │  │  │  └─ routes
│  │  │  │     └─ actualites.routes.ts
│  │  │  ├─ admin
│  │  │  │  ├─ routes
│  │  │  │  │  └─ admin.routes.ts
│  │  │  │  └─ services
│  │  │  │     └─ admin.service.ts
│  │  │  ├─ affectation
│  │  │  │  └─ routes
│  │  │  │     └─ affectation.routes.ts
│  │  │  ├─ ai
│  │  │  │  └─ routes
│  │  │  │     └─ ai.routes.ts
│  │  │  ├─ alerts
│  │  │  │  └─ routes
│  │  │  │     └─ alerts.routes.ts
│  │  │  ├─ annonces
│  │  │  │  └─ routes
│  │  │  │     └─ annonces.routes.ts
│  │  │  ├─ auth
│  │  │  │  ├─ auth.service.ts
│  │  │  │  ├─ email.service.ts
│  │  │  │  └─ routes
│  │  │  │     └─ auth.routes.ts
│  │  │  ├─ copieRemise
│  │  │  │  └─ routes
│  │  │  │     └─ copiesRemise.routes.ts
│  │  │  ├─ dashboard
│  │  │  │  ├─ routes
│  │  │  │  │  ├─ teacher-dashboard.routes.ts
│  │  │  │  │  └─ teacherDashboard.routes.js
│  │  │  │  └─ services
│  │  │  │     ├─ teacher-dashboard.service.ts
│  │  │  │     └─ teacherDashboard.service.js
│  │  │  ├─ discipline
│  │  │  │  └─ routes
│  │  │  │     └─ discipline.routes.ts
│  │  │  ├─ documents
│  │  │  │  └─ routes
│  │  │  │     └─ documents.routes.ts
│  │  │  ├─ enseignants
│  │  │  │  └─ routes
│  │  │  │     └─ enseignants.routes.ts
│  │  │  ├─ pfe
│  │  │  │  └─ routes
│  │  │  │     ├─ group-management.routes.ts
│  │  │  │     └─ pfe.routes.ts
│  │  │  ├─ requests
│  │  │  │  ├─ routes
│  │  │  │  │  └─ request.routes.ts
│  │  │  │  └─ validators
│  │  │  │     └─ request.validator.ts
│  │  │  ├─ settings
│  │  │  │  └─ routes
│  │  │  │     └─ site-settings.routes.ts
│  │  │  ├─ student
│  │  │  │  ├─ routes
│  │  │  │  │  └─ student.routes.ts
│  │  │  │  └─ services
│  │  │  │     ├─ student-panel.service.ts
│  │  │  │     └─ student.service.ts
│  │  │  └─ teacher
│  │  │     ├─ routes
│  │  │     │  └─ teacher.routes.ts
│  │  │     └─ services
│  │  │        └─ teacher.service.ts
│  │  ├─ server.ts
│  │  ├─ services
│  │  │  ├─ actualites
│  │  │  │  └─ actualites.service.ts
│  │  │  ├─ affectation
│  │  │  │  └─ affectation.service.ts
│  │  │  ├─ ai
│  │  │  │  └─ ai.service.ts
│  │  │  ├─ alerts
│  │  │  │  └─ alerts.service.ts
│  │  │  ├─ annonces
│  │  │  │  └─ announcements.service.ts
│  │  │  ├─ auth
│  │  │  │  └─ auth.service.ts
│  │  │  ├─ common
│  │  │  │  ├─ audit-log.service.ts
│  │  │  │  ├─ rbac.service.ts
│  │  │  │  └─ search.service.ts
│  │  │  ├─ dashboard
│  │  │  │  ├─ admin-dashboard.service.ts
│  │  │  │  └─ teacher-dashboard.service.ts
│  │  │  ├─ discipline
│  │  │  │  └─ discipline.service.ts
│  │  │  ├─ documents
│  │  │  │  └─ documents.service.ts
│  │  │  ├─ email
│  │  │  │  └─ email.service.ts
│  │  │  ├─ index.ts
│  │  │  ├─ pfe
│  │  │  │  ├─ pfe-assignment.service.ts
│  │  │  │  ├─ pfe-group.service.ts
│  │  │  │  └─ pfe.service.ts
│  │  │  ├─ requests
│  │  │  │  ├─ requests.service.ts
│  │  │  │  └─ workflow.service.ts
│  │  │  └─ student
│  │  │     └─ student.service.ts
│  │  └─ utils
│  │     ├─ logger.ts
│  │     ├─ password.ts
│  │     └─ tokens.ts
│  ├─ test-env.ts
│  ├─ tsconfig.json
│  ├─ tsconfig.tsbuildinfo
│  └─ uploads
│     ├─ 1775491605105.jpg
│     ├─ 1776522212586.jpg
│     ├─ 1776536781275-auto-send-test.pdf
│     ├─ annonces
│     │  ├─ 1776287765987-712318874.pdf
│     │  ├─ 1776289937264-669409353.pdf
│     │  ├─ 1776366997477-568830915.pdf
│     │  └─ 1776510332656-907308340.jpg
│     ├─ announcements
│     ├─ site-settings
│     │  └─ 1776506764300-Logo.png
│     ├─ student-reclamations
│     ├─ student-requests
│     ├─ teacher-announcements
│     └─ teacher-documents
├─ CLEANUP_RECOMMENDATIONS.md
├─ CONTRIBUTING.md
├─ docs
│  ├─ API_CONTRACT.md
│  ├─ database_schema.sql
│  ├─ project architecture.txt
│  └─ templates
│     ├─ users-import-test-valid-only.xlsx
│     └─ users-import-test.xlsx
├─ frontend
│  ├─ package-lock.json
│  ├─ package.json
│  ├─ postcss.config.js
│  ├─ public
│  │  ├─ apple-touch-icon.png
│  │  ├─ favicon-96x96.png
│  │  ├─ favicon.ico
│  │  ├─ favicon.svg
│  │  ├─ index.html
│  │  ├─ Logo.png
│  │  ├─ logo192.png
│  │  ├─ logo512.png
│  │  ├─ manifest.json
│  │  ├─ robots.txt
│  │  ├─ site.webmanifest
│  │  ├─ web-app-manifest-192x192.png
│  │  └─ web-app-manifest-512x512.png
│  ├─ README.md
│  ├─ src
│  │  ├─ App.jsx
│  │  ├─ assets
│  │  │  └─ images
│  │  │     ├─ Banner.jpg
│  │  │     ├─ computer.jpg
│  │  │     ├─ hero-bg.jpg
│  │  │     ├─ ibnKhaldoun.jpg
│  │  │     ├─ prof.jpg
│  │  │     ├─ student1.jpg
│  │  │     ├─ student2.jpg
│  │  │     └─ Students.jpg
│  │  ├─ components
│  │  │  ├─ admin
│  │  │  │  ├─ AdminSectionCard.jsx
│  │  │  │  ├─ shared
│  │  │  │  │  ├─ DataTable.jsx
│  │  │  │  │  ├─ Modal.jsx
│  │  │  │  │  └─ Pagination.jsx
│  │  │  │  ├─ StaffManagementTable.jsx
│  │  │  │  ├─ StudentAssignmentManager.jsx
│  │  │  │  ├─ TeacherAssignmentWorkflow.jsx
│  │  │  │  └─ UserRegistrationForm.jsx
│  │  │  ├─ ai
│  │  │  │  └─ AIChatbot.jsx
│  │  │  ├─ auth
│  │  │  │  └─ ProtectedRoute.jsx
│  │  │  ├─ common
│  │  │  │  ├─ AlertBanner.jsx
│  │  │  │  ├─ Button
│  │  │  │  │  ├─ Button.jsx
│  │  │  │  │  └─ index.js
│  │  │  │  ├─ Card
│  │  │  │  │  ├─ Card.jsx
│  │  │  │  │  └─ index.js
│  │  │  │  ├─ DashboardCard.jsx
│  │  │  │  ├─ Footer
│  │  │  │  │  ├─ Footer.jsx
│  │  │  │  │  └─ index.js
│  │  │  │  ├─ Input
│  │  │  │  │  ├─ index.js
│  │  │  │  │  └─ Input.jsx
│  │  │  │  ├─ ModulePlaceholderPage.jsx
│  │  │  │  ├─ Navbar
│  │  │  │  │  ├─ index.js
│  │  │  │  │  └─ Navbar.jsx
│  │  │  │  └─ Skeleton.jsx
│  │  │  ├─ dashboard
│  │  │  │  ├─ DashboardSection.jsx
│  │  │  │  ├─ EmptyState.jsx
│  │  │  │  ├─ KPITile.jsx
│  │  │  │  ├─ ProgressBar.jsx
│  │  │  │  ├─ StatusIndicator.jsx
│  │  │  │  └─ teacher
│  │  │  │     ├─ AttendanceBoard.jsx
│  │  │  │     ├─ AttendanceButtons.jsx
│  │  │  │     ├─ DashboardCharts.jsx
│  │  │  │     ├─ DataTables.jsx
│  │  │  │     ├─ NoteForm.jsx
│  │  │  │     ├─ NotesBoard.jsx
│  │  │  │     ├─ ProfileHeader.jsx
│  │  │  │     ├─ StatCards.jsx
│  │  │  │     ├─ StudentManagement.jsx
│  │  │  │     ├─ StudentsBoard.jsx
│  │  │  │     └─ StudentTable.jsx
│  │  │  ├─ features
│  │  │  │  ├─ about
│  │  │  │  │  ├─ AboutHero.jsx
│  │  │  │  │  ├─ HistorySection.jsx
│  │  │  │  │  ├─ MissionSection.jsx
│  │  │  │  │  └─ TeamSection.jsx
│  │  │  │  ├─ auth
│  │  │  │  │  ├─ LoginForm.jsx
│  │  │  │  │  └─ RegisterForm.jsx
│  │  │  │  ├─ contact
│  │  │  │  │  ├─ ContactForm.jsx
│  │  │  │  │  ├─ ContactHero.jsx
│  │  │  │  │  ├─ ContactInfo.jsx
│  │  │  │  │  └─ MapSection.jsx
│  │  │  │  ├─ home
│  │  │  │  │  ├─ BannerSection.jsx
│  │  │  │  │  ├─ FeaturesSection.jsx
│  │  │  │  │  ├─ GallerySection.jsx
│  │  │  │  │  ├─ HeroSection.jsx
│  │  │  │  │  └─ StatisticsSection.jsx
│  │  │  │  ├─ news
│  │  │  │  │  └─ news.jsx
│  │  │  │  └─ teacher
│  │  │  │     ├─ OverviewStats.jsx
│  │  │  │     ├─ PendingTasks.jsx
│  │  │  │     ├─ RecentCourses.jsx
│  │  │  │     ├─ TeacherHeader.jsx
│  │  │  │     ├─ TeacherSidebar.jsx
│  │  │  │     └─ UpcomingClasses.jsx
│  │  │  ├─ home
│  │  │  │  ├─ AnnouncementsSection.jsx
│  │  │  │  ├─ BannerSection.jsx
│  │  │  │  ├─ FeaturesSection.jsx
│  │  │  │  ├─ GallerySection.jsx
│  │  │  │  ├─ HeroSection.jsx
│  │  │  │  ├─ NewsIntegrationSection.jsx
│  │  │  │  └─ StatisticsSection.jsx
│  │  │  ├─ layout
│  │  │  │  ├─ AuthLayout
│  │  │  │  │  ├─ AuthLayout.jsx
│  │  │  │  │  └─ index.js
│  │  │  │  └─ MainLayout
│  │  │  │     ├─ index.js
│  │  │  │     └─ MainLayout.jsx
│  │  │  └─ public
│  │  │     ├─ PublicFooter.jsx
│  │  │     ├─ PublicLayout.jsx
│  │  │     └─ PublicNavbar.jsx
│  │  ├─ contexts
│  │  │  ├─ AuthContext.jsx
│  │  │  └─ SiteSettingsContext.jsx
│  │  ├─ design-system
│  │  │  ├─ components
│  │  │  │  ├─ Alert.jsx
│  │  │  │  ├─ Button.jsx
│  │  │  │  ├─ Card.jsx
│  │  │  │  ├─ form
│  │  │  │  │  ├─ Checkbox.jsx
│  │  │  │  │  ├─ index.js
│  │  │  │  │  ├─ Input.jsx
│  │  │  │  │  └─ PasswordInput.jsx
│  │  │  │  ├─ index.js
│  │  │  │  ├─ Modal.jsx
│  │  │  │  └─ navigation
│  │  │  │     ├─ index.js
│  │  │  │     ├─ Sidebar.jsx
│  │  │  │     └─ Topbar.jsx
│  │  │  ├─ docs
│  │  │  │  └─ README.md
│  │  │  ├─ themes
│  │  │  │  └─ ThemeProvider.jsx
│  │  │  └─ tokens
│  │  │     ├─ colors.js
│  │  │     ├─ spacing.js
│  │  │     └─ typography.js
│  │  ├─ hooks
│  │  │  ├─ useAuth.js
│  │  │  ├─ useLocalStorage.js
│  │  │  └─ useNotification.js
│  │  ├─ i18n
│  │  │  ├─ index.js
│  │  │  └─ locales
│  │  │     ├─ ar.json
│  │  │     ├─ en.json
│  │  │     └─ fr.json
│  │  ├─ index.css
│  │  ├─ index.jsx
│  │  ├─ layouts
│  │  │  ├─ AdminLayout.jsx
│  │  │  ├─ DashboardLayout.jsx
│  │  │  ├─ StudentLayout.jsx
│  │  │  └─ TeacherLayout.jsx
│  │  ├─ pages
│  │  │  ├─ AboutPage.jsx
│  │  │  ├─ ActualitesPage.jsx
│  │  │  ├─ admin
│  │  │  │  └─ Groups.jsx
│  │  │  ├─ AdminAcademicAssignmentsPage.jsx
│  │  │  ├─ AdminAcademicManagementPage.jsx
│  │  │  ├─ AdminAlertsPage.jsx
│  │  │  ├─ AdminPanelPage.jsx
│  │  │  ├─ AdminRequestsPage.jsx
│  │  │  ├─ AdminSiteSettingsPage.jsx
│  │  │  ├─ AdminUsersListPage.jsx
│  │  │  ├─ AdminUsersPage.jsx
│  │  │  ├─ AIAssistantPage.jsx
│  │  │  ├─ CaseDetailPage.jsx
│  │  │  ├─ ChangePasswordPage.jsx
│  │  │  ├─ ComponentShowcase.jsx
│  │  │  ├─ ContactPage.jsx
│  │  │  ├─ dashboard
│  │  │  │  ├─ student
│  │  │  │  │  └─ StudentDashboard.jsx
│  │  │  │  └─ teacher
│  │  │  │     └─ TeacherDashboard.jsx
│  │  │  ├─ DisciplinaryCasesPage.jsx
│  │  │  ├─ DocumentsPage.jsx
│  │  │  ├─ ForgotPasswordPage.jsx
│  │  │  ├─ HomePage.jsx
│  │  │  ├─ LoginPage.jsx
│  │  │  ├─ NotFoundPage.jsx
│  │  │  ├─ PFE
│  │  │  │  ├─ DefensePage.jsx
│  │  │  │  ├─ GroupsPage.jsx
│  │  │  │  ├─ ProjectsPage.jsx
│  │  │  │  └─ SubjectsPage.jsx
│  │  │  ├─ ProfilePage.jsx
│  │  │  ├─ RegisterPage.jsx
│  │  │  ├─ RequestDetailPage.jsx
│  │  │  ├─ RequestsPage.jsx
│  │  │  ├─ ResetPasswordPage.jsx
│  │  │  ├─ SettingsPage.jsx
│  │  │  ├─ Student
│  │  │  │  ├─ Dashboard.jsx
│  │  │  │  ├─ index.js
│  │  │  │  ├─ MyComplaints.jsx
│  │  │  │  ├─ MyCourses.jsx
│  │  │  │  ├─ MyGrades.jsx
│  │  │  │  ├─ MyProjects.jsx
│  │  │  │  ├─ Profile.jsx
│  │  │  │  └─ Schedule.jsx
│  │  │  ├─ StudentDashboard.jsx
│  │  │  ├─ StudentDisciplinaryView.jsx
│  │  │  ├─ StudentNotesPage.jsx
│  │  │  ├─ StudentSpecialiteChoicePage.jsx
│  │  │  ├─ SupportPage.jsx
│  │  │  ├─ Teacher
│  │  │  │  ├─ Dashboard.jsx
│  │  │  │  ├─ GradeManagement.jsx
│  │  │  │  ├─ index.js
│  │  │  │  ├─ MyCourses.jsx
│  │  │  │  ├─ MyStudents.jsx
│  │  │  │  ├─ Profile.jsx
│  │  │  │  ├─ Projects.jsx
│  │  │  │  └─ Schedule.jsx
│  │  │  ├─ TeacherDashboard.jsx
│  │  │  └─ UnauthorizedPage.jsx
│  │  ├─ routes
│  │  │  ├─ PrivateRoute.jsx
│  │  │  ├─ StudentRoutes.jsx
│  │  │  └─ TeacherRoutes.jsx
│  │  ├─ services
│  │  │  ├─ ai.js
│  │  │  ├─ api.js
│  │  │  └─ pfe.js
│  │  ├─ theme
│  │  │  ├─ ThemeProvider.jsx
│  │  │  └─ ThemeSwitcher.jsx
│  │  └─ utils
│  │     ├─ constants.js
│  │     ├─ formatters.js
│  │     ├─ rbac.js
│  │     └─ validators.js
│  └─ tailwind.config.js
├─ GROUP_8_PFE_CONTRIBUTIONS.md
├─ README.md
├─ REFACTOR_LOG.md
├─ rules.md
├─ skill.md
├─ tmp_admin_cookies.txt
├─ tmp_source_compare_report.txt
└─ tmp_source_list.txt

```
