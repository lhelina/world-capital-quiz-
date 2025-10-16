Capital City Quiz 


A web-based quiz that tests users on country capitals. Users enter the capital of a randomly selected country, and the app keeps track of their total correct answers. The quiz data is stored in a PostgreSQL database.
Technologies used: Node.js, Express, PostgreSQL, EJS, HTML/CSS, dotenv

-Features
Randomly selects a country from the database.
Users submit their answers and get instant feedback.
Keeps track of total correct answers.
Alerts the user when a wrong answer is submitted.

Setup / How to Run
1.Clone the repository
```
git clone https://github.com/yourusername/capital-city-quiz.git
cd capital-city-quiz
```
2.Install dependencies
```
npm install
```
3.Setup PostgreSQL database
Create a database (e.g., world)
Create the capitals table:
```
CREATE TABLE capitals (
  country VARCHAR(100) PRIMARY KEY,
  capital VARCHAR(100) NOT NULL
);

-- Example insert
INSERT INTO capitals (country, capital) VALUES
('France', 'Paris'),
('United Kingdom', 'London'),
('United States of America', 'Washington');
```

4.Create a .env file in the project root:
```
DB_USER=your_postgres_user
DB_PASSWORD=your_password
DB_HOST=localhost
DB_PORT=5432
DB_NAME=world
PORT=3000
```
5.Run the server
```
npm start
```
6.Open in browser
Visit http://localhost:3000 to play the quiz.
