- 👋 Hi, I’m @NAWABNOMAN786
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
NAWABNOMAN786/NAWABNOMAN786 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
pip install Flask

from flask import Flask, render_template

app = Flask(__name__)

# Sample products data
products = [
    {"id": 1, "name": "Product 1", "price": 100},
    {"id": 2, "name": "Product 2", "price": 150},
]

@app.route('/')
def index():
    return render_template('index.html', products=products)

if __name__ == '__main__':
    app.run(debug=True)
