# Etworks — Job Portal Frontend

Etworks is the React frontend for a job portal that supports job seekers, employers, and administrators. It provides the user-facing workflows for discovering jobs, managing applications, maintaining profiles, and accessing role-specific dashboards.

## Frontend visual assets

The repository includes these interface-related assets used by the frontend:

| Hero visual | Authentication visual |
|---|---|
| ![Etworks hero background asset](public/herobg_v2.png) | ![Etworks authentication side asset](public/auth_side_image_v2.png) |

These are existing design assets, not captured screenshots of the running application. Add real browser screenshots of the homepage, job listings, and role-specific dashboards when available.

## Main application areas

- Account registration, email OTP verification, login, logout, and password reset
- Google OAuth sign-in flow and role selection
- Role-protected seeker, employer, and administrator areas
- Job browsing, filtering, saving, liking, and posting workflows
- Seeker profile details, skills, projects, and CV information
- CV builder interface with preview and PDF download workflow
- Employer company profile and verification workflow
- Administrator screens for users, CV templates, and company verification
- Job alerts, notifications, and AI assistant interface
- Chapa job-posting payment workflow

## Technology

- React 19
- Vite
- Tailwind CSS
- React Router
- Zustand
- Axios

The frontend works with the companion [EtworksBackend](https://github.com/kura458/EtworksBackend) service.

## Run locally

Make sure the backend is configured and running before testing features that require API access.

```bash
npm install
npm run dev
```

Vite's development server normally starts at:

```text
http://localhost:5173
```

## Environment configuration

Create a local `.env` file in the frontend project root. Configure the API base URL expected by the application:

```env
VITE_API_BASE_URL=http://localhost:8080
VITE_ENV=development
```

Use the actual backend URL for your environment. Never commit private tokens or credentials.

## Related repository

- [EtworksBackend — Spring Boot API](https://github.com/kura458/EtworksBackend)

## Development notes

Some application routes or screens may still be under development. Verify the current implementation before treating a workflow as production-ready.

## Author

Maintained under [kura458](https://github.com/kura458).

---

*Building practical job-search experiences with modern web technologies.*
