# Magic Link
This is the second edition of #umaStackQueNaoDomino. Python Edition.
The project offer API to generate, send and validate a magic link.

# What's a Magic Link
Magic Link is kind of an authenticated URL, which you send to the consumer in form of SMS/email that helps them to log in to the system with just one click of the link without any human interaction (no need for the user to enter username+password).
[Description Source](https://hackernoon.com/magic-links-d680d410f8f7)

# First things first 
You need to have pip (of course).
 
- `python3 -m venv env`
- `source env/bin/activate`
- `which python`
- `pip install -r requirements.txt`

## How to Run
### Running FastAPI
- `uvicorn main:app --reload`

### Running Redis Server
- `redis-server`

### Consume Queue
- `rq worker send_magic_links`

## Firestore
On this project we store validated magic links into Firebase Firestore, please check the oficial [quick start documentation](https://firebase.google.com/docs/firestore/quickstart) in order to setup your project and export the `serviceAccountKey.json`

