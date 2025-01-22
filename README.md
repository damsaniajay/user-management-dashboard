
# User Management Dashboard

A React-based user management dashboard that allows users to view, add, edit, and delete user details. The application uses JSONPlaceholder API for simulating backend operations and implements local storage for data persistence.

## Features

* View list of users with comprehensive details (ID, First Name, Last Name, Email, Department)
* Add new users through a modal form
* Edit existing user details
* Delete users with confirmation
* Local storage integration for data persistence
* Loading states and error handling
* Responsive design with Tailwind CSS
* Reusable UI components

## Prerequisites

* Node.js (v14.0.0 or higher)
* npm (v6.0.0 or higher)

## Project Setup

1. Clone the repository:
```bash
git clone <your-repository-url>
cd user-management-dashboard
```

2. Initialize the project:
```bash
npm create vite@latest . -- --template react
```
When prompted:
- Select React as the framework
- Select JavaScript as the variant

3. Install dependencies:
```bash
npm install
```

4. Install required packages:
```bash
npm install clsx tailwind-merge lucide-react @radix-ui/react-dialog @radix-ui/react-slot class-variance-authority
```

5. Install Tailwind CSS and its dependencies:
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

6. Start the development server:
```bash
npm run dev
```

7. Open your browser and navigate to the displayed local URL (typically http://localhost:5173) to view the application.

## Project Structure

```
user-management-dashboard/
├── src/
│   ├── App.jsx                    # Main application component
│   ├── main.jsx                   # Entry point
│   ├── index.css                  # Global styles
│   ├── components/
│   │   ├── UserManagementDashboard.jsx
│   │   └── ui/                    # Reusable UI components
│   │       ├── alert.jsx
│   │       ├── card.jsx
│   │       └── dialog.jsx
│   └── lib/
│       └── utils.js               # Utility functions
├── index.html
├── package.json
├── vite.config.js
└── tailwind.config.js
```

## Key Components

### UserManagementDashboard
- Main dashboard component
- Handles CRUD operations
- Implements local storage
- Manages user interface state

### UI Components
- Alert: Displays error and success messages
- Card: Container component for content sections
- Dialog: Modal component for forms

## Dependencies

* React (via Vite)
* Tailwind CSS - Utility-first CSS framework
* class-variance-authority - For managing component variants
* clsx - Utility for constructing className strings
* tailwind-merge - Utility for merging Tailwind classes
* Lucide React - Icon components
* Radix UI primitives - Accessible component primitives

## Features Implementation

### Data Persistence
- Uses localStorage to persist user data between sessions
- Falls back to API data if no local data is available

### User Management
- Create: Add new users with form validation
- Read: Display users in a responsive table
- Update: Edit existing user information
- Delete: Remove users with confirmation

### API Integration
Uses JSONPlaceholder API (https://jsonplaceholder.typicode.com) for simulating backend operations:
* GET /users - Fetch initial users list
* POST /users - Simulate adding new user
* PUT /users/:id - Simulate updating user
* DELETE /users/:id - Simulate deleting user

## Available Scripts

* `npm run dev` - Start development server
* `npm run build` - Build for production
* `npm run preview` - Preview production build

## Development Notes

* The application maintains data in localStorage for persistence
* API calls are simulated using JSONPlaceholder
* Unique IDs are generated using timestamp + index
* Display IDs are maintained sequentially

## Future Improvements

* Add sorting and filtering capabilities
* Implement search functionality
* Add pagination for large datasets
* Implement data caching
* Add more robust form validation
* Add unit tests
* Add batch delete functionality
* Implement user roles and permissions

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
=======
# user-management-dashboard
