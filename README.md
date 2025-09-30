# Cloud_Dashboard
# CNAPP Dashboard

A comprehensive **Cloud Native Application Protection Platform (CNAPP)** dashboard built with React, TypeScript, Redux Toolkit, and Recharts. This project provides dynamic security monitoring with interactive charts for Cloud Security Posture Management (CSPM), Cloud Workload Protection Platform (CWPP), and Registry Scanning.

## 🚀 Features

- **Dynamic Widget System**: Add, remove, and customize widgets across different security categories
- **Interactive Charts**: Real-time data visualization using Recharts (Pie, Bar, Line, Area charts)
- **State Management**: Redux Toolkit for predictable state management
- **Modern UI**: Beautiful, responsive design with Tailwind CSS and shadcn/ui components
- **Local Storage**: Persistent data storage for widget configurations
- **Custom Widgets**: Create your own custom widgets with personalized content
- **Search Functionality**: Quick widget search and filtering
- **Category Management**: Organized security dashboards (CSPM, CWPP, Registry Scan)

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18 or higher) - [Download here](https://nodejs.org/)
- **npm** (comes with Node.js) or **yarn**
- **Git** - [Download here](https://git-scm.com/)

## 🛠️ Local Setup Instructions

### 1. Clone the Repository

```bash
git clone <github.com/abhishekpandey12121>
cd <Cloud_Dashboard>
```

### 2. Install Dependencies

Using npm:
```bash
npm install
```

Or using yarn:
```bash
yarn install
```

### 3. Start the Development Server

Using npm:
```bash
npm run dev
```

Or using yarn:
```bash
yarn dev
```

The application will start on `http://localhost:5173` (or another port if 5173 is busy).

### 4. Build for Production

To create a production build:

```bash
npm run build
```

The build output will be in the `dist` folder.

### 5. Preview Production Build

To preview the production build locally:

```bash
npm run preview
```

## 🏗️ Project Structure

```
src/
├── components/          # React components
│   ├── ui/             # shadcn/ui components
│   ├── AddWidgetDialog.tsx
│   ├── CategorySection.tsx
│   ├── ChartWidget.tsx
│   ├── DashboardHeader.tsx
│   └── WidgetCard.tsx
├── contexts/           # React contexts (deprecated, using Redux now)
├── data/               # JSON data files
│   └── dashboardData.json
├── hooks/              # Custom React hooks
├── pages/              # Page components
│   ├── Home.tsx        # Landing page
│   ├── Index.tsx       # Dashboard page
│   └── NotFound.tsx    # 404 page
├── store/              # Redux store configuration
│   ├── slices/         # Redux slices
│   │   └── dashboardSlice.ts
│   ├── hooks.ts        # Typed Redux hooks
│   └── index.ts        # Store configuration
├── types/              # TypeScript type definitions
│   └── dashboard.ts
├── App.tsx             # Main App component
├── index.css           # Global styles
└── main.tsx           # Application entry point
```

## 🎨 Technology Stack

- **Framework**: React 18
- **Language**: TypeScript
- **Build Tool**: Vite
- **State Management**: Redux Toolkit
- **UI Framework**: Tailwind CSS
- **Component Library**: shadcn/ui
- **Charts**: Recharts
- **Routing**: React Router v6
- **Icons**: Lucide React
- **Notifications**: Sonner

## 🔧 Configuration

### Environment Variables

This project doesn't require environment variables for basic functionality. All configurations are handled through:

- `tailwind.config.ts` - Tailwind CSS configuration
- `vite.config.ts` - Vite build configuration
- `tsconfig.json` - TypeScript configuration

### Customizing Data

To customize the initial dashboard data, edit:

```
src/data/dashboardData.json
```

The JSON structure includes:
- Categories (CSPM, CWPP, Registry Scan)
- Widgets with text, chart type, and chart data
- Available widgets for the add widget dialog

## 📦 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

## 🌐 Deployment

This project can be deployed to various platforms:


### Vercel
```bash
npm install -g vercel
vercel
```

### Netlify
```bash
npm install -g netlify-cli
netlify deploy
```

## 🎯 Usage

### Adding Widgets
1. Click the "+ Add Widget" button in any category
2. Select from available widgets or create a custom one
3. Widget will be added to the selected category

### Removing Widgets
1. Hover over any widget card
2. Click the X button that appears in the top-right corner

### Creating Custom Widgets
1. Click "+ Add Widget"
2. Navigate to the "Custom" tab
3. Enter widget name and content
4. Click "Create Widget"

### Data Persistence
All widget configurations are automatically saved to browser's localStorage and persist across sessions.

## 🔒 Security Features Monitored

- **CSPM**: Cloud accounts status, risk assessments, security scores
- **CWPP**: Namespace alerts, workload protection, compliance status
- **Registry Scan**: Image vulnerabilities, security issues, scan history

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 🆘 Troubleshooting

### Port Already in Use
If port 5173 is busy, Vite will automatically use the next available port.

### Build Errors
```bash
# Clear node_modules and reinstall
rm -rf node_modules package-lock.json
npm install
```

### Type Errors
```bash
# Restart TypeScript server in VS Code
Cmd/Ctrl + Shift + P → TypeScript: Restart TS Server
```


## ✨ Features Showcase

### Interactive Charts
- Pie charts for distribution analysis
- Bar charts for comparative data
- Line charts for trends
- Area charts for cumulative metrics

### Modern UI/UX
- Responsive grid layouts
- Smooth animations and transitions
- Dark/light mode support via Tailwind
- Accessible components from shadcn/ui

### State Management
- Centralized Redux store
- Type-safe actions and reducers
- Middleware support
- DevTools integration

---

