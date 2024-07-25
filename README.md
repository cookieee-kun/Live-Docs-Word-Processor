## <a name="introduction"> Introduction</a>

LiveDocs is a Next.js web application designed to emulate Google Docs, featuring real-time multi-user collaboration and comprehensive document management. The application is built using Next.js for the user interface, Liveblocks for real-time functionalities, and styled with TailwindCSS.

## <a name="tech-stack"> Tech Stack</a>

- Next.js
- TypeScript
- Liveblocks
- Lexical Editor
- ShadCN
- Tailwind CSS

## <a name="features"> Features</a>

 **1. Authentication**: User authentication using GitHub through NextAuth, ensuring secure sign-in/out and session management.

**2. Collaborative Text Editor**: Multiple users can edit the same document simultaneously with real-time updates.

**3. Documents Management**
   - **Create Documents**: Users can create new documents, which are automatically saved and listed.
   - **Delete Documents**: Users can delete documents they own.
   - **Share Documents**: Users can share documents via email or link with view/edit permissions.
   - **List Documents**: Display all documents owned or shared with the user, with search and sorting functionalities.

 **4. Comments**: Users can add inline and general comments, with threading for discussions.

**5. Active Collaborators on Text Editor**: Show active collaborators with real-time presence indicators.

**6. Notifications**: Notify users of document shares, new comments, and collaborator activities.

**7. Responsive**: The application is responsive across all devices.

and many more, including code architecture and reusability 

## <a name="quick-start"> Quick Start</a>

Follow these steps to set up the project locally on your machine.

**Prerequisites**

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

**Cloning the Repository**

```bash
git clone https://github.com/cookieee-kun/Live-Docs-Word-Processor.git
cd collaborative-editor
```

**Installation**

Install the project dependencies using npm:

```bash
npm install
```

**Set Up Environment Variables**

Create a new file named `.env` in the root of your project and add the following content:

```env
#Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

#Liveblocks
NEXT_PUBLIC_LIVEBLOCKS_PUBLIC_KEY=
LIVEBLOCKS_SECRET_KEY=
```

Replace the placeholder values with your actual Clerk & LiveBlocks credentials. You can obtain these credentials by signing up on the [Clerk](https://clerk.com/) and [Liveblocks](liveblocks.io/) website.

**Running the Project**

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to view the project.
