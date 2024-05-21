# FLASK

### Flask installation
```
pip install flask
```

### Minimal application
```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"
```

### Run the app.py to initialize it on the Flask server 
