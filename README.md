# Quiz response scoring

A take-home assessment: a timed quiz. The submitted answers, the evaluator and the score are saved through an API.

## `quiz_app_api`: Django + Django REST Framework

The `quiz` app holds the question and answer models and a submission endpoint that validates the payload and stores the quiz, its question/answer pairs and the score in one transaction, with API tests.

```bash
cd quiz_app_api
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## `quiz-app-web`: React

Quiz rendering with a countdown (`react-countdown`), submission through Axios, and unit tests for the quiz component and API client.

```bash
cd quiz-app-web
npm install
npm start
```
