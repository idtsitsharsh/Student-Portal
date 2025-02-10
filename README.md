Student Portal Dashboard
This is a student portal dashboard built using Next.js and Tailwind CSS. The dashboard displays various sections such as a welcome banner, upcoming tests, attempted tests, and a left sidebar navigation menu.

Features
Left Sidebar Navigation: Contains links for Tests, Announcements, Profile, and Schedule.
Welcome Banner: Displays a personalized welcome message and a 3D avatar.
Upcoming Tests: A section that shows the list of upcoming tests with subject names and dates.
Attempted Tests: Displays previously attempted tests with scores and time taken.
Tech Stack
Next.js: React framework for building the application.
Tailwind CSS: Utility-first CSS framework for styling.
Lucide Icons: Provides modern, open-source icons used in the sidebar.
Project Structure
bash
Copy
Edit
/src
├── app
│   ├── layout.js
│   └── page.js
├── components
│   ├── LeftSidebar.js
│   ├── UpcomingTestCards.js
│   ├── AttemptedTestSection.js
│   └── WelcomeBanner.js
└── styles
    └── globals.css
src/app/
layout.js: Main layout of the application.
page.js: Main page that renders the dashboard.
src/components/
LeftSidebar.js: Sidebar with navigation links.
UpcomingTestCards.js: Displays upcoming tests.
AttemptedTestSection.js: Displays attempted tests.
WelcomeBanner.js: Displays a welcome message and avatar.
src/styles/
globals.css: Global styles used across the app.
Installation
Clone the repository to your local machine:

bash
Copy
Edit
git clone <repository_url>
Navigate into the project directory:

bash
Copy
Edit
cd <project_directory>
Install the necessary dependencies:

bash
Copy
Edit
npm install
Configure Tailwind CSS: Ensure that the tailwind.config.js file is set up correctly to point to your src directory for CSS purging. Example:

js
Copy
Edit
module.exports = {
  content: [
    './src/**/*.{js,ts,jsx,tsx}', // Make sure to include the src folder
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
Create a .env.local file to store any local environment variables (if needed).

Running the Project
Run the development server:

bash
Copy
Edit
npm run dev
Open your browser and go to:

arduino
Copy
Edit
http://localhost:3000
Folder Structure
src/: Contains all the source code for the application.
components/: Reusable components for the dashboard.
styles/: Tailwind CSS configuration and global styles.
app/: The core of the application, including the main page and layout.
Customizing the Dashboard
You can modify the following sections to suit your needs:

LeftSidebar.js: Update the navigation items and icons.
UpcomingTestCards.js: Modify the test details such as name, date, and subject.
AttemptedTestSection.js: Add or remove attempted tests and their scores.
WelcomeBanner.js: Update the avatar and the welcome message.
Contribution
Feel free to fork this repository and contribute to improving the dashboard. If you have any suggestions or improvements, open an issue or submit a pull request.
