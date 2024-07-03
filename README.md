# ToDo-List

ToDo-List is an application that allows users to maintain a ToDo-List for a day. Users can add new items, edit previous items, or delete items that have been completed. This project is a basic website with a minimal frontend that uses Node.js and Express.js for backend operations and EJS for dynamic rendering. PostgreSQL is used to maintain a database for performing CRUD operations on the items list.

## Table of Contents
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Tech Stack
- **CSS3**: For styling the web page.
- **Node.js**: For setting up the backend server.
- **Express.js**: For managing server-side logic and routing.
- **EJS**: For rendering dynamic content on the web page.
- **PostgreSQL**: For storing and managing the ToDo items.

## Features
- **Add New Items**: Allows users to add new tasks to their ToDo list.
- **Edit Items**: Users can edit the details of existing tasks.
- **Delete Items**: Users can delete tasks that have been completed.
- **CRUD Operations**: The application performs Create, Read, Update, and Delete operations on the database.

## Getting Started
To get a local copy up and running, follow these simple steps:

### Prerequisites
- Node.js installed on your local machine
- PostgreSQL installed and configured
- PG Admin installed for database management
- A code editor (e.g., VSCode)

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/ManavNakai/ToDo-List.git
   ```
2. Navigate to the project directory:
   ```sh
   cd ToDo-List
   ```
3. Install the required dependencies:
   ```sh
   npm install
   ```
   
4. Set up the PostgreSQL database `todo_list` locally using PG Admin and create the `items` table:
   
   4.1. **Open PG Admin and create a new database**:
   
   - Open PG Admin and create a new database named `todo_list`.
   
   4.2. **Create the `items` table**:

   - Create a table named `items` with the following structure:
     
     ```sql
        CREATE TABLE items (
          id SERIAL PRIMARY KEY,
          title VARCHAR(100) NOT NULL
        );
     ```
     
5. Create a `.env` file in the project root and add your PostgreSQL database connection details:
   ```plaintext
   PG_USER=your_db_user
   PG_HOST="localhost"
   PG_DATABASE="todo_list"
   PG_PASSWORD=your_db_password
   PG_PORT="5432"
   ```
6. Start the server:
   ```sh
   node index.js
   ```
7. Open your web browser and go to `http://localhost:3000`.

## Usage
- Open your web browser and navigate to `http://localhost:3000`.
- Use the input field to add new items to your ToDo list.
- Edit or delete items as needed using the provided options.

## Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have suggestions for improving the project, please follow these steps:
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
Distributed under the MIT License. See `LICENSE` for more information.

## Contact
Project Link: [https://github.com/ManavNakai/ToDo-List](https://github.com/ManavNakai/ToDo-List)

---

Thank you for checking out the ToDo-List project! Feel free to reach out if you have any questions or need further assistance.
