**Seeker's Centre**

**Seeker's Centre** is a job listing platform designed to help job seekers find jobs and internships  and allow administrators  to upload and manage job postings efficiently. ![](Aspose.Words.812fdfd3-b226-4110-aa37-1bdfe058b03e.001.png)

**Features**

**User Features**

- **Registration & Login**: Users can create an account and log in securely.
- **Job Listings**: Browse available jobs and internships.
- **Job Application Links**: Navigate directly to the application  page for each job.

**Admin Features**

- **Job Upload**: Admins can upload job details, which are dynamically displayed  on the platform.
- **Delete Jobs**: Admins can remove jobs directly from the admin panel. ![](Aspose.Words.812fdfd3-b226-4110-aa37-1bdfe058b03e.002.png)

**Tech Stack**

**Backend**

- **Node.js**: Handles server-side logic.
- **Express**: Manages server requests and routing.
- **MongoDB**: Database to store user information.

**Frontend**

- **HTML/CSS/JavaScript**: Build the user interface.
- **Static Pages**: Jobs and internships  are served dynamically.

**Additional Libraries/Tools**

- **Mongoose**: MongoDB object modeling  for Node.js.
- **Bcrypt**: Secure password hashing.
- **Multer**: Handle file uploads.
- **Cors**: Enable cross-origin requests. ![](Aspose.Words.812fdfd3-b226-4110-aa37-1bdfe058b03e.003.png)

**Prerequisites**

- **Node.js**: Ensure Node.js is installed (v14+ recommended).
- **MongoDB**: Install MongoDB  and ensure it is running  on localhost:27017. ![ref1]

**Setup Instructions**

1. **Download zip file**

cd seekers-centre

2. **Install Dependencies** npm install
2. **Configure MongoDB**

   Ensure MongoDB is running  locally. Modify the MongoDB connection  string in server.js if necessary: mongoose.connect('mongodb://127.0.0.1:27017/seekers-centre',  { useNewUrlParser: true, useUnifiedTopology:  true });

4. **Start the Server**

node server.js

The server will start on http://localhost:5000. ![](Aspose.Words.812fdfd3-b226-4110-aa37-1bdfe058b03e.005.png)

**Project Structure**

Seeker's Centre/

├── models/

│   └── user.js                     # User schema and methods ├── public/

│   ├── jobs/                       # Contains individual job description HTML files │   │   ├── job1.html               # Example job HTML

│   │   ├── job2.html               # Example job HTML

│   │   └── ...                     # Other job description  files

│   ├── bg1.webp                    # Background  images

│   ├── logo.png                    # Platform logo

│   ├── profile-icon.png            # Profile icon image

│   ├── styles.css                  # Global styling file

│   ├── index.html                  # Landing page for users

│   ├── jobs.html                   # Jobs listing page

│   ├── internships.html            # Internships listing page

│   └── logged\_in/                  # Separate logged-in user folder

│       ├── admin.html              # Admin panel page

│       ├── jobs.html               # Jobs listing for logged-in users

│       ├── internships.html        # Internships listing for logged-in users

│       ├── styles.css              # Styling for logged-in users

│       └── ...                     # Supporting  images/scripts

├── server/

│   └── server.js                   # Main server code

├── package.json                    # Dependencies and scripts ├── package-lock.json               # Dependency tree lockfile ![ref1]

**API Endpoints**

**User Endpoints**

**Endpoint  Method Description ![](Aspose.Words.812fdfd3-b226-4110-aa37-1bdfe058b03e.006.png)**/api/register  POST  Register a new user. /api/login

|POST |
| - |
|POST |

/api/logout

**Admin Endpoints**



|Upload a new job or internship. |
| - |

**Endpoint  Method ![](Aspose.Words.812fdfd3-b226-4110-aa37-1bdfe058b03e.007.png)**/upload-job  POST /admin  GET ![](Aspose.Words.812fdfd3-b226-4110-aa37-1bdfe058b03e.008.png)

Access admin panel.

**Usage**

1. **Run the Platform**
- Access the app at http://localhost:5000.
2. **Admin Job Upload**
- Navigate to the admin panel at /admin.
- Fill in the job details form to upload a job.
3. **Job Browsing**
- Visit the jobs or internships  pages to view listings.

**Common Issues & Solutions**

**MongoDB Connection Error**

- Ensure MongoDB is running: mongod
- Verify the database connection  string in server.js.

**Static Files Not Found**

- Confirm static files are placed in the public/ directory.

**License :** This project is licensed under the MIT License.**

