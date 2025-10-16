# duedatedash.github.io
from flask import Flask, render_template_string

app = Flask(__name__)

@app.route('/')
def home():
    return render_template_string("""
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>9A DueDateDash</title>
        <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&display=swap" rel="stylesheet">
        <style>
            body {
                background-color: #f3e5ab;
                display: flex;
                justify-content: center;
                align-items: center;
                height: 100vh;
                margin: 0;
                font-family: 'Playfair Display', serif;
            }
            h1 {
                color: #5a3e2b;
                font-size: 4rem;
                text-shadow: 3px 3px 10px rgba(90, 62, 43, 0.3);
                background: linear-gradient(90deg, #a47c48, #8b5e34, #5a3e2b);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
                animation: glow 3s ease-in-out infinite alternate;
            }
            @keyframes glow {
                from { text-shadow: 0 0 5px #a47c48, 0 0 10px #8b5e34; }
                to { text-shadow: 0 0 15px #a47c48, 0 0 30px #8b5e34; }
            }
        </style>
    </head>
    <body>
        <h1>9A DueDateDash</h1>
    </body>
    </html>
    """)

if __name__ == '__main__':
    app.run(debug=True)
