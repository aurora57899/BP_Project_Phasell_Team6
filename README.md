# BP_Project_Phase2_Team6
# Scrum:
Scrum is a specific framework within the Agile methodology. It emphasizes short, iterative work cycles called sprints, usually lasting 1-4 weeks. It involves daily stand-up meetings, sprint planning, sprint review, and sprint retrospective.
Scrum is well-suited for projects where there's a need for frequent feedback, collaboration among team members, and the ability to quickly adapt to changes.
For a food diet and weight calculations app, where user needs might evolve, and there could be a requirement for frequent updates and adjustments based on user feedback, Agile or Scrum would likely be more suitable than the Waterfall model. Among Agile methodologies, Scrum is particularly popular for its structure and focus on continuous improvement.


# User Requirements:
# Stakeholders for Budget Planning Software Project:
# End-users: 
These individuals or organizations will directly interact with the budget planning software to manage their finances. They are interested in user-friendly interfaces, accurate calculations, and features that simplify their budgeting process.
# Clients: 
Clients commission the development of the software and provide project requirements. They are interested in meeting specific business objectives, enhancing customer satisfaction, and gaining a competitive edge in the market.
# Developers:
Developers are responsible for designing, coding, and maintaining the software. They aim to build robust, scalable, and secure software that meets the needs of end-users while adhering to project timelines and budget constraints.
# Project Managers:
Project managers oversee the development process, ensuring project goals are met within allocated resources. They coordinate communication between stakeholders, manage risks, and monitor progress to deliver a high-quality product on time and within budget.
# Financial Advisors/Experts: 
These stakeholders provide insights into budgeting best practices. They ensure the software incorporates industry standards and addresses users' specific needs, focusing on features aligned with sound financial principles.


## User Stories:

# User Type: End-user
# Requirement:
As an end-user, I want to be able to import my financial data from various sources (bank accounts, credit cards, etc.) into the software.
# Benefit: 
This feature saves time and effort for users by eliminating the need to manually input financial data, ensuring accuracy and completeness in budget planning.
# User Type: Administrator
# Requirement: 
As an administrator, I need the ability to customize budget categories and set spending limits for different users or departments.
Benefit: This functionality allows administrators to tailor the software to specific organizational needs, ensuring flexibility and control over budgeting processes.
# User Type: End-user
# Requirement: 
As an end-user, I want to receive notifications and alerts when I exceed budget limits or when important financial milestones are reached.
# Benefit: 
Notifications keep users informed about their financial status in real-time, prompting them to make adjustments and avoid overspending, leading to better financial management.
# User Type: Client
# Requirement: 
As a client, I expect the software to have robust data security measures to protect sensitive financial information.
# Benefit:
Implementing strong security measures builds trust with clients, ensuring the confidentiality and integrity of their financial data, and mitigating risks associated with data breaches.
# User Type: Developer
# Requirement:
As a developer, I need comprehensive documentation and support resources to understand the software architecture and integrate new features seamlessly.
# Benefit:
Well-documented software facilitates collaboration among developers, reduces development time, and enhances the overall quality and maintainability of the software.


# Functional Requirements:

# Brief Description:
# Expense Tracking:
The system should allow users to input and track their expenses easily.
# Budget Creation:
Users should be able to create and customize their budgets based on income and expenses.
# Income Management:
Users should be able to input and manage their sources of income.
# Category Management: 
The system should support the creation and customization of spending categories.
# Reporting:
Users should be able to generate reports summarizing their financial activities and performance against budget goals.


# b. Acceptance Criteria:
# Expense Tracking:
Users can add new expenses with details such as amount, date, and category.
Users can view a list of all recorded expenses.
Expenses are displayed in a clear and organized manner.
# Budget Creation:
Users can create a new budget by specifying income sources and allocating funds to different expense categories.
Budgets can be edited or deleted as needed.
Budgets reflect accurate calculations based on user inputs.
# Income Management:
Users can add new sources of income with details such as amount and frequency.
Income sources are displayed along with expenses for a comprehensive financial overview.
Users can edit or delete income sources as necessary.
# Category Management:
Users can create custom spending categories.
Users can assign expenses to specific categories.
Categories can be edited, deleted, or reorganized by the user.
# Reporting:
Users can generate reports for a specified time period, displaying total income, total expenses, and budget variances.
Reports are presented in a visually appealing and easy-to-understand format.
Users can export reports in various formats (e.g., PDF, CSV) for further analysis or sharing.

# Non-Functional Requirements:
# Brief Description:

# Performance:
The system should respond quickly to user actions and provide a seamless experience.
# Usability:
The system should be intuitive and easy to navigate, requiring minimal training for users to understand and utilize its features.
# Reliability:
The system should be dependable, with minimal downtime or errors, ensuring users can rely on it for accurate budget planning.
# Security: 
The system should protect user data and privacy through robust security measures, such as encryption and secure authentication.

# b. Acceptance Criteria:
# Performance:
The system should load within 3 seconds of user initiation.
Response times for actions like adding expenses or generating reports should be under 1 second.
The system should handle concurrent user interactions without noticeable lag or delays.
# Usability:
Users should be able to perform common tasks (e.g., adding expenses, creating budgets) without referring to documentation.
Navigation menus and buttons should be logically organized and labeled clearly.
Help documentation should be easily accessible within the application.
# Reliability:
The system should have a uptime of at least 99.9%.
Backup and recovery procedures should be in place to ensure data integrity in case of system failures.
Error messages should be informative and guide users on how to resolve issues.
# Security:
User passwords should be securely hashed and stored.
The system should utilize HTTPS for secure communication over the internet.
Access controls should be implemented to restrict unauthorized access to sensitive user 

# a. Architecture:
The chosen architecture for the food diet and weight calculations app is a client-server architecture with a three-tier structure: presentation layer, application layer, and data layer.
Presentation Layer: This layer handles the user interface components, including screens for inputting food intake, tracking weight, and viewing diet plans.
Application Layer: This layer contains the business logic and processes user requests. It interacts with the presentation layer for user input and with the data layer for retrieving and storing data.
Data Layer: This layer includes the database where user information, food data, diet plans, and weight tracking data are stored. It interacts with the application layer for data retrieval and storage.

# b. Database Model:
The database model includes tables for users, food items, diet plans, and weight tracking.
Tables: Users (user_id, username, password, email, etc.), FoodItems (food_id, name, calories, nutrients, etc.), DietPlans (plan_id, user_id, start_date, end_date, plan_details, etc.), WeightTracking (tracking_id, user_id, date, weight).
Relationships: Users have a one-to-many relationship with DietPlans and WeightTracking. FoodItems are referenced in DietPlans.
Constraints: Unique constraints on usernames and email addresses to ensure data integrity.

# c. Technologies Used:
Frontend: HTML5, CSS3, JavaScript, React.js for dynamic UI elements and user interaction.
Backend: Node.js for server-side logic, Express.js for RESTful API development, and authentication.
Database: MongoDB for its flexibility and scalability in handling unstructured data.
Additional Technologies: JSON Web Tokens (JWT) for authentication and authorization, bcrypt for password hashing, Axios for HTTP requests.

# d. User Interface Design:
(Provide wireframes/mockups or describe the UI)
Wireframes include screens for user registration/login, inputting food intake, tracking weight, viewing diet plans, and accessing user settings.
The UI design focuses on simplicity, intuitive navigation, and clear presentation of data.

# e. Security Measures:
Encryption: User passwords are hashed using bcrypt before storing in the database to protect against unauthorized access.
Authentication: JWT tokens are generated upon successful login and passed with each request for user authentication.
Authorization: Restricted access to certain endpoints based on user roles and permissions.
Data Validation: Input data is validated on both the client and server sides to prevent injection attacks and ensure data integrity.
Secure Communication: HTTPS protocol is used to encrypt data transmission between the client and server, providing an additional layer of security.
