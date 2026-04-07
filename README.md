# Home Rental System

A full-stack web application for listing, browsing, and managing home rentals. Built with Node.js, Express, MongoDB, and EJS templating.

## Features

- **User Authentication**: Sign up and login functionality for users
- **Create Listings**: Users can create and edit property listings
- **Reviews & Ratings**: Add reviews and ratings to listings
- **Responsive Design**: Clean and intuitive user interface
- **Image Support**: Upload and display property images
- **Search & Filter**: Find listings based on requirements
- **Admin Dashboard**: Manage users and listings

## Project Structure

```
├── app.js                 # Main application file
├── middleware.js          # Custom middleware functions
├── schema.js              # Database schema validations
├── package.json           # Project dependencies
│
├── models/                # MongoDB models
│   ├── listing.js         # Listing model
│   ├── review.js          # Review model
│   └── user.js            # User model
│
├── routes/                # Express routes
│   ├── listing.js         # Listing routes
│   ├── review.js          # Review routes
│   └── user.js            # User routes
│
├── classroom/             # Additional classroom features
│   ├── server.js          # Classroom server
│   └── routes/            # Classroom routes
│
├── views/                 # EJS templates
│   ├── layouts/           # Layout templates
│   ├── includes/          # Reusable components
│   ├── listings/          # Listing views
│   └── users/             # User views
│
├── public/                # Static files
│   ├── css/               # Stylesheets
│   └── js/                # Client-side scripts
│
├── utils/                 # Utility functions
│   ├── ExpressError.js    # Custom error class
│   └── wrapAsync.js       # Async error wrapper
│
└── init/                  # Database initialization
    ├── index.js
    └── data.js
```

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/snehalsable10/Home-Rental-System.git
   cd Home-Rental-System
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory:
   ```
   MONGODB_URI=your_mongodb_connection_string
   SESSION_SECRET=your_session_secret
   PORT=3000
   ```

4. **Initialize the database**
   ```bash
   node init/index.js
   ```

5. **Start the application**
   ```bash
   npm start
   ```

   The app will be available at `http://localhost:3000`

## Usage

### User Registration & Login
- Navigate to the signup page to create a new account
- Login with your credentials
- Access your profile and manage listings

### Creating a Listing
1. Click "Add New Listing"
2. Fill in property details (title, description, location, price, etc.)
3. Upload property images
4. Submit the listing

### Viewing & Reviewing
- Browse all available listings
- Click on a listing to view details
- Add reviews and ratings to properties you've visited

## Technologies Used

- **Backend**: Node.js, Express.js
- **Database**: MongoDB, Mongoose ODM
- **Frontend**: EJS, HTML, CSS, JavaScript
- **Authentication**: Express Session, Passport.js
- **Other**: Multer (file uploads), Joi (validation)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

---

**Author**: Sneha  
**Repository**: [Home-Rental-System](https://github.com/snehalsable10/Home-Rental-System)
