# QuickDesk - Help Desk Solution

![QuickDesk Logo](https://img.shields.io/badge/QuickDesk-Help%20Desk%20Solution-blue)
![Odoo Hackathon](https://img.shields.io/badge/Odoo%20x%20CGC%20Mohali-Hackathon%202025-orange)

## 🎯 Project Overview

QuickDesk is a simple, efficient help desk solution developed for the Odoo x CGC Mohali Hackathon 2025. The system provides streamlined communication between users and support teams, enabling efficient ticket management and resolution without unnecessary complexity.

## 🚀 Features

### 👥 User Management
- User Registration & Authentication: Secure login/register system
- Role-based Access Control: Three distinct user roles
  - End Users: Create and track tickets
  - Support Agents: Manage and resolve tickets
  - Admins: Full system management

### 🎫 Ticket Management
- Ticket Creation: Users can create tickets with:
  - Subject and detailed description
  - Category selection
  - Optional file attachments
  - Automatic status assignment (Open)

- Ticket Tracking: Real-time status updates
  - Open → In Progress → Resolved → Closed
  - Threaded conversation timeline
  - Comment and update history

### 🔍 Advanced Search & Filtering
- Status-based Filtering: Open/Closed tickets
- Personal Tickets: View only user's own tickets
- Category-based Search: Filter by ticket categories
- Smart Sorting: 
  - Most replied tickets
  - Recently modified
  - Creation date

### 🔔 Notification System
- Email Notifications: Automated alerts for:
  - New ticket creation
  - Status changes
  - Agent responses
  - Ticket resolution

### 📊 Dashboard Features
- User Dashboard: 
  - Personal ticket overview
  - Status summaries
  - Quick actions
- Agent Dashboard:
  - Ticket queues (My Tickets, All Tickets)
  - Assignment management
  - Response actions
- Admin Dashboard:
  - System-wide analytics
  - User management
  - Category management

### 💬 Interactive Features
- Voting System: Upvote/Downvote questions and responses
- Reply System: Threaded conversations on tickets
- Ticket Sharing: Share tickets with team members

## 🛠 Technology Stack

- Frontend: React.js with modern hooks and components
- Backend: Node.js with Express.js framework
- Database: MongoDB with Mongoose ODM
- Authentication: JWT (JSON Web Tokens) with bcrypt for password hashing
- Email Service: Nodemailer for email notifications
- File Storage: Multer for file upload handling
- Styling: CSS3 / Bootstrap / Material-UI (or your preferred styling solution)

## 📋 System Requirements

### User Roles & Permissions

#### End Users (Employees/Customers)
- Create and submit support tickets
- Track ticket status and progress
- Reply to agent responses
- View personal ticket history
- Update profile and notification preferences

#### Support Agents
- View and manage assigned tickets
- Update ticket status and priority
- Add comments and internal notes
- Create tickets on behalf of users
- Access ticket analytics and reports

#### Administrators
- Complete user management (roles, permissions)
- Category and classification management
- System configuration and settings
- Access to all tickets and analytics
- User role assignment and modification

## 🎮 User Flow

1. User Registration/Login: New users register or existing users login
2. Ticket Creation: User creates ticket with required details
3. Automatic Assignment: Ticket enters "Open" status in agent queue
4. Agent Processing: Support agent picks up and processes ticket
5. Status Updates: Ticket progresses through workflow states
6. User Communication: Users receive updates and can reply
7. Resolution: Ticket is resolved and closed with user confirmation

## 🏗 Project Structure

```
QuickDesk/
├── backend/                 # Node.js Express Backend
│   ├── models/             # MongoDB Mongoose models
│   ├── controllers/        # Route controllers and business logic
│   ├── routes/            # Express API routes
│   ├── middleware/        # Authentication, validation middleware
│   ├── config/            # Database and app configuration
│   ├── uploads/           # File upload directory
│   └── server.js          # Express server entry point
├── frontend/              # React.js Frontend
│   ├── src/
│   │   ├── components/    # Reusable React components
│   │   ├── pages/        # React page components
│   │   ├── services/     # API service calls
│   │   ├── context/      # React Context for state management
│   │   ├── utils/        # Helper functions
│   │   └── App.js        # Main React component
│   ├── public/           # Static assets
│   └── package.json      # Frontend dependencies
├── README.md             # Project documentation
└── .gitignore           # Git ignore rules
```

## 🚀 Installation & Setup

### Prerequisites
- Node.js 16+ and npm
- MongoDB (local installation or MongoDB Atlas)
- Git for version control

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/GiriAditya14/QuickDesk_Odoo_Hackathon.git
   cd QuickDesk_Odoo_Hackathon
   ```

2. **Backend Setup**
   ```bash
   # Navigate to backend directory
   cd backend
   
   # Install dependencies
   npm install
   
   # Configure environment variables
   cp .env.example .env
   # Edit .env with your MongoDB URI, JWT secret, email config
   
   # Start backend server
   npm start
   # or for development
   npm run dev
   ```

3. **Frontend Setup**
   ```bash
   # Navigate to frontend directory (open new terminal)
   cd frontend
   
   # Install dependencies
   npm install
   
   # Configure environment variables
   cp .env.example .env
   # Add your backend API URL
   
   # Start React development server
   npm start
   ```

4. **Access the Application**
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000/api`

## 📝 API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Ticket Management
- `GET /api/tickets` - Get all tickets (with filters)
- `POST /api/tickets` - Create new ticket
- `GET /api/tickets/:id` - Get specific ticket
- `PUT /api/tickets/:id` - Update ticket
- `DELETE /api/tickets/:id` - Delete ticket

### User Management (Admin)
- `GET /api/users` - Get all users
- `PUT /api/users/:id/role` - Update user role
- `DELETE /api/users/:id` - Delete user

### Categories
- `GET /api/categories` - Get all categories
- `POST /api/categories` - Create category (Admin)
- `PUT /api/categories/:id` - Update category (Admin)

## 🧪 Testing

```bash
# Run backend tests
cd backend
npm test

# Run frontend tests
cd frontend
npm test

# Run all tests
npm run test:all
```

## 🎯 Key Features Implemented

- ✅ User authentication and authorization
- ✅ Ticket creation with attachments
- ✅ Status workflow management
- ✅ Advanced search and filtering
- ✅ Email notification system
- ✅ Voting system for tickets
- ✅ Responsive dashboard design
- ✅ Role-based access control
- ✅ Category management
- ✅ Threaded conversations

## 🏆 Hackathon Highlights

This project was developed for the Odoo x CGC Mohali Hackathon 2025 and demonstrates:
- Clean Architecture: Well-structured, maintainable codebase
- User Experience: Intuitive interface design
- Scalability: Designed to handle growing user bases
- Performance: Optimized for fast response times
- Security: Implemented proper authentication and authorization

## 👨‍💻 Team

### Development Team - Odoo x CGC Mohali Hackathon 2025

- Aditya Giri   - Backend Developer & Database Design
- Ansh Mishra   - Backend Developer & Database Design
- Kanak Gupta   - Frontend Developer & UI/UX Design
- Khushi Shrivastava - Frontend Developer & Testing

Repository: [QuickDesk_Odoo_Hackathon](https://github.com/GiriAditya14/QuickDesk_Odoo_Hackathon)
## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (git checkout -b feature/amazing-feature)
3. Commit your changes (git commit -m 'Add some amazing feature')
4. Push to the branch (git push origin feature/amazing-feature)
5. Open a Pull Request

## 📞 Support

For any queries or support regarding this project:
- GitHub Issues: [Create an issue](https://github.com/GiriAditya14/QuickDesk_Odoo_Hackathon/issues)

## 🔮 Future Enhancements

- [ ] Real-time chat using Socket.io
- [ ] Mobile-responsive Progressive Web App (PWA)
- [ ] Advanced analytics dashboard with Chart.js
- [ ] Integration with Slack/Discord for notifications
- [ ] Multi-language support with i18next
- [ ] Knowledge base with rich text editor
- [ ] Automated ticket routing based on keywords
- [ ] SLA (Service Level Agreement) tracking
- [ ] Customer satisfaction surveys
- [ ] Advanced reporting and export features

---

Built with ❤️ using MERN Stack for Odoo x CGC Mohali Hackathon 2025


