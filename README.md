Temporary Firebase account	


stefan@mindliteracy.com
dodecaedru172812


rm database.db
uvicorn main:app --host 0.0.0.0 --port 8089 --reload

export GOOGLE_APPLICATION_CREDENTIALS="9af211329b2fc82e5efe906062c730082819b23fe8394bc435e0b1bf0458eb54"
export FIREBASE_CONFIG="b79606fb3afea5bd1609ed40b622142f1c98125abcfe89a76a661b0e8e343910"



export GOOGLE_APPLICATION_CREDENTIALS="/Users/stefandeaconu/PycharmProjects/Personal/9af211329b2fc82e5efe906062c730082819b23fe8394bc435e0b1bf0458eb54"
export FIREBASE_CONFIG="/Users/stefandeaconu/PycharmProjects/Personal/b79606fb3afea5bd1609ed40b622142f1c98125abcfe89a76a661b0e8e343910"

PYTHONPATH="/Users/stefandeaconu/PycharmProjects/Personal/empowerpeople-api/" fastapi dev main.py --port 8089 --reload%
