
---

## **2️⃣ ARCHITECTURE.md** (Brief Architecture/Design Explanation)

Create a file called `ARCHITECTURE.md` in your project folder:

```markdown
# Architecture / Design

## Backend
- **Node.js + Express** handles API routes
- **Endpoints:**
  - `/signup` → register user
  - `/login` → authenticate user, return JWT
  - `/projects` → create and list user projects
  - `/chat` → chat under a project, store messages
- **Authentication:** JWT token in `Authorization` header
- **Storage:** In-memory arrays (users, projects, prompts)
- **Chat:** Mock responses (can be replaced with OpenAI API)

## Frontend
- **HTML + JS** page
- Signup/Login form
- Project creation & listing
- Chat interface with messages
- Sends JWT in headers for protected routes

## Future Enhancements
- Use **OpenAI API** for real responses
- Store data in **AWS DynamoDB**
- Upload files to **AWS S3**
- Deploy backend on **AWS EC2 or Elastic Beanstalk**
