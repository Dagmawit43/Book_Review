# Book Review Platform

A modern, full-stack web application for book enthusiasts to discover, review, and track their reading journey. Built with Next.js, React, and Prisma ORM.

## 🌟 Features

- **User Authentication**: Secure signup and login system
- **Book Management**: Add, view, and manage books in your collection
- **Review System**: Rate and review books with text reviews
- **Reading Status**: Track books as 'Want to Read', 'Currently Reading', or 'Read'
- **User Profiles**: Customizable user profiles with reading statistics
- **Genre Filtering**: Browse books by genre
- **Responsive Design**: Works on desktop and mobile devices
- **Admin Dashboard**: Manage users, books, and reviews

## 🛠️ Tech Stack

- **Frontend**: Next.js 13+ (App Router), React 19, Tailwind CSS
- **Backend**: Next.js API Routes
- **Database**: SQLite with Prisma ORM
- **Authentication**: JWT (JSON Web Tokens)
- **Form Handling**: React Hook Form with Zod validation
- **UI Components**: Custom components with Tailwind CSS
- **Image Handling**: Next.js Image Optimization

## 📦 Prerequisites

- Node.js 18.0.0 or later
- npm or yarn
- SQLite (included with Node.js)

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/Dagmawit43/Book_Review.git/
   cd book-review-platform
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory and add the following:
   ```
   DATABASE_URL="file:./dev.db"
   JWT_SECRET="your-secret-key-here"
   ```

4. **Set up the database**
   ```bash
   npx prisma generate
   npx prisma db push
   ```

5. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

6. **Open [http://localhost:3000](http://localhost:3000)** in your browser

## 🗄️ Database Schema

The application uses the following data models:

- **User**: User accounts and profiles
- **Book**: Book information and metadata
- **Review**: User reviews of books
- **Genre**: Book genres and categories
- **UserBookStatus**: Tracks reading status of books for users
- **Contact**: Contact form submissions

## 📂 Project Structure

```
book-review-platform/
├── src/
│   ├── app/                 # Next.js 13+ App Router
│   │   ├── api/             # API routes
│   │   ├── admin/           # Admin dashboard
│   │   ├── book/            # Book-related pages
│   │   └── ...
│   ├── components/          # Reusable UI components
│   ├── context/             # React context providers
│   └── hooks/               # Custom React hooks
├── prisma/
│   ├── migrations/          # Database migrations
│   └── schema.prisma        # Prisma schema
├── public/                  # Static files
├── schemas/                 # Zod validation schemas
└── utils/                   # Utility functions
```

## 🔒 Authentication

The application uses JWT (JSON Web Tokens) for authentication. Protected routes check for a valid JWT in the request headers.

## 📝 API Endpoints

### Auth
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/me` - Get current user profile

### Books
- `GET /api/books` - Get all books
- `GET /api/books/:id` - Get a single book
- `POST /api/books` - Create a new book (admin only)
- `PUT /api/books/:id` - Update a book (admin only)
- `DELETE /api/books/:id` - Delete a book (admin only)

### Reviews
- `GET /api/reviews` - Get all reviews
- `GET /api/reviews/:id` - Get a single review
- `POST /api/reviews` - Create a new review
- `PUT /api/reviews/:id` - Update a review
- `DELETE /api/reviews/:id` - Delete a review

## 🧪 Testing

To run tests:
```bash
npm test
# or
yarn test
```

## 🚀 Deployment

### Vercel
This project is optimized for deployment on Vercel. You can deploy it with a few clicks:

[![Deployed with Vercel](https://vercel.com/button)](https://book-review-3ilh.vercel.app/)

### Live Demo
Check out the deployed project here: [Book Review Platform Live Demo](https://book-review-3ilh.vercel.app/)

## 👥 Contributors

- **Dagmawit Gebreweld** - Frontend Developer  
- **Nathnael Andargachew** - Backend Developer  
- **Tinbite Yonas** - Frontend Developer & Video

## Github Links of contributors ![GitHub](https://img.shields.io/badge/GitHub-000?logo=github&logoColor=white)
- **Dagmawit Gebreweld** - [![GitHub](https://img.shields.io/badge/GitHub-000?logo=github&logoColor=white)](https://github.com/Dagmawit43)
- **Nathnael Andargachew** - [![GitHub](https://img.shields.io/badge/GitHub-000?logo=github&logoColor=white)](https://github.com/malon328)  
- **Tinbite Yonas** - [![GitHub](https://img.shields.io/badge/GitHub-000?logo=github&logoColor=white)](https://github.com/Trilord52)

## 📹 Demo Video
https://drive.google.com/file/d/1LG_hScm-CuRbbeZeWjpTHpHbbTnm9eky/view?usp=sharing
Watch the demo video here: [Google Drive Link](https://drive.google.com/file/d/1LG_hScm-CuRbbeZeWjpTHpHbbTnm9eky/view?usp=sharing)

## 🙏 Acknowledgments

- Built with ❤️ using Next.js and Prisma
- Icons from [Heroicons](https://heroicons.com/)
- UI components built with Tailwind CSS

## 📬 Contact

For any questions, please contact us (contributors) on GitHub.
