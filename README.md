# Symphony Limited MVC - .NET 10.0

## Quick Setup (Visual Studio)

### Step 1: Database Setup
1. SQL Server mein yeh database already exist karna chahiye: `SymphonyLtd1DB`
2. Ya khud banayein: `CREATE DATABASE SymphonyLtd1DB;`

### Step 2: Connection String
`appsettings.json` mein apna SQL Server name check karein:
```json
"Server=.;Database=SymphonyLtd1DB;Trusted_Connection=True;TrustServerCertificate=True;"
```
Agar SQL Server ka naam alag hai to change karein (e.g. `Server=YOURPC\SQLEXPRESS`)

### Step 3: Migrations Run Karein
Visual Studio mein **Package Manager Console** kholein:
```
Add-Migration InitialCreate
Update-Database
```

### Step 4: Run!
Press `F5` ya `Ctrl+F5`

---

## Admin Login
- **Username:** admin
- **Password:** admin123

---

## Project Structure
- **Public Site:** `/` - Home, Courses, Exam Results, FAQs, Contact
- **Admin Panel:** `/Admins/Login` - Full CRUD for all 18 tables

## Features
- Public homepage with GSAP animations
- Roll number based result lookup
- Contact form with DB storage
- Admin dashboard with stats
- Complete CRUD for all 18 database tables
- Session-based admin authentication
- Auto-seeded FAQs and default content

## Tech Stack
- .NET 10.0 MVC
- Entity Framework Core 9
- SQL Server
- Bootstrap 5.3
- GSAP Animations
