# WhizQuiz

This is an online quiz organizing website project, developed using Python's web framework Django.<br>

## Current Features

### Site access features:

* User must be logged in to access the Quiz.
* For signup user is required to give *username*, *first name*, *last name*, *e-mail address* and *password*.
* For login the user will be required to enter *username* and *password* only.

### Features of the quiz:

* All questions are multiple choice question.
* Each question is displayed only once per user.
* Questions are displayed randomly for every user.
* If the user by-mistake presses refresh or go back to the previous page, there will be a new question for the user and the 
  question he/she was on will be marked as attempted.
* A message will be  displayed after every attempted question whether the answer was correct or incorrect.


### Leaderboard features:

* Leaderboard is a shorted list according to the score obtained by the users.
* If two users are having same score, the user who has signed up earlier will have good ranking than the one who joined late.
* Leaderboard is open to all. No login required.

### Administrative features:

* Only admin can add questions.
* Admin can add questions and modify them until they are not marked as *Has been published?*
* Once a question has been published, it can neither be modified nor can be accessed. Admin can only see a list of questions.
* Admin can search questions by question text or choice text.
* Admin can filter questions based on whether the questions have been published or not.


### 1. Clone this repository
```bash
git clone https://github.com/superkd37/WhizQuiz.git
```

### 2. Install the virtual environment pipenv
```bash
pip install pipenv
```

### 3. Create the virtualenv
```bash
## run following command from `WhizQuiz` directory
pipenv shell
```

### 4. Install python packages
```bash
cd WhizQuiz
pip install -r requirements.txt
```

### 5. Setup the database
*TODO - Add instructions for this when I start using MySQL database.*

### 6. Run database migrations
```bash
python manage.py migrate
```

### 7. Create superuser
```bash
python manage.py createsuperuser
```

### 8. Run development server
```bash
python manage.py runserver
```
