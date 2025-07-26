# Job Listing App

A modern, full-stack job listing application that connects to a live API to fetch real job opportunities. Built with Next.js, Redux Toolkit Query, TypeScript, and Tailwind CSS, featuring real-time data fetching, state management, and a responsive design.

## 🌟 Features

- **Live Job Data**: Fetches real job listings from external API (`akil-backend.onrender.com`)
- **Advanced State Management**: Redux Toolkit Query for efficient data fetching and caching
- **Smart Loading States**: Loading indicators and error handling for better UX
- **Job Sorting**: Sort opportunities by relevance, name, or date added
- **Detailed Job Pages**: Click on any job to see comprehensive details including:
  - Job description and responsibilities
  - Ideal candidate requirements
  - Location and timing information
  - Required skills and categories
  - Company information and logos
- **Responsive Design**: Optimized for desktop and mobile devices
- **Modern UI**: Clean interface with hover effects and smooth transitions
- **Fallback Handling**: Graceful handling of missing company logos

## 🛠️ Tech Stack

- **Framework**: [Next.js 15](https://nextjs.org) with App Router
- **Language**: TypeScript
- **State Management**: Redux Toolkit Query (RTK Query)
- **Styling**: Tailwind CSS v4 & DaisyUI
- **Icons**: React Icons
- **Runtime**: React 19
- **API**: External REST API integration

## 🚀 Getting Started

### Prerequisites

Make sure you have Node.js installed on your machine (version 18 or higher recommended).

### Installation

1. Clone the repository:

```bash
git clone <your-repo-url>
cd job_listing_app
```

2. Install dependencies:

```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## 📁 Project Structure

```
job_listing_app/
├── app/
│   ├── components/
│   │   ├── JobCard.tsx          # Job card component with Redux integration
│   │   └── ReduxProvider.tsx    # Redux store provider wrapper
│   ├── jobs/
│   │   └── [jobId]/
│   │       └── page.tsx         # Individual job detail page
│   ├── apiSlice.ts             # RTK Query API slice for job data
│   ├── store.ts                # Redux store configuration
│   ├── data.ts                 # TypeScript type definitions
│   ├── layout.tsx              # Root layout with Redux provider
│   └── page.tsx                # Home page
├── eslint.config.mjs          # ESLint configuration
├── next.config.ts             # Next.js configuration
├── tailwind.config.js         # Tailwind CSS configuration
└── tsconfig.json              # TypeScript configuration
```

## � Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## 📊 API & Data Structure

### External API Integration

The application fetches data from: `https://akil-backend.onrender.com/`

**Endpoints:**

- `GET /opportunities/search` - Fetch all job listings
- `GET /opportunities/{id}` - Fetch specific job details

### Redux State Management

- **RTK Query**: Handles API calls with automatic caching and loading states
- **Store Configuration**: Centralized state management with Redux Toolkit
- **Error Handling**: Graceful error states with user-friendly messages

## 🎨 Customization

### Working with the API

The application is designed to work with the live API, but you can:

1. Modify the `baseUrl` in `apiSlice.ts` to point to a different backend
2. Extend the API slice to include additional endpoints
3. Customize the data transformation logic

## 📸 Preview

Simple Loading Page 
![Screen Recording 2025-07-26 at 12 09 37 in the afternoon](https://github.com/user-attachments/assets/44cdc452-17fa-46f8-90a8-a2b70b379b60)

Opportunities Page (Not as slow as shown here)
<img width="1440" height="462" alt="Screenshot 2025-07-26 at 12 14 13 in the afternoon" src="https://github.com/user-attachments/assets/dd6c246b-1a2c-4f04-83c7-06343713794b" />


Applicant Page
<img width="1440" height="774" alt="Screenshot 2025-07-26 at 12 14 28 in the afternoon" src="https://github.com/user-attachments/assets/6c6053bb-f659-4337-8547-66a784a7331c" />


## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Learn More

To learn more about the technologies used in this project:

- [Next.js Documentation](https://nextjs.org/docs) - Learn about Next.js features and API
- [Redux Toolkit Query](https://redux-toolkit.js.org/rtk-query/overview) - Learn about RTK Query for data fetching
- [Redux Toolkit](https://redux-toolkit.js.org/) - Learn modern Redux patterns
- [TypeScript Documentation](https://www.typescriptlang.org/docs/) - Learn TypeScript
- [Tailwind CSS Documentation](https://tailwindcss.com/docs) - Learn Tailwind CSS
- [DaisyUI Documentation](https://daisyui.com/) - Learn DaisyUI components
- [React Documentation](https://react.dev/) - Learn React
