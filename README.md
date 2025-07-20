
# 💱 Currency Converter (Streamlit App)

A simple, real-time currency converter built with [Streamlit](https://streamlit.io/) that allows users to convert amounts between different currencies using live exchange rates.

---

## 🚀 Features

- Convert between any two currencies instantly.
- Real-time exchange rates from [ExchangeRate-API](https://www.exchangerate-api.com/).
- Clean, interactive UI using Streamlit.
- No button press needed — auto-updates on input change!

---

## 📁 Project Structure

```
currency-converter/
├── constants.py         # List of available currencies
├── main.py              # Core logic: fetching rates & converting
├── app.py               # Streamlit UI logic
├── requirements.txt     # List of Python dependencies
└── README.md            # Project documentation (this file)
```

---

## 🧩 Example UI

<p align="center">
  <img src="https://streamlit.io/images/brand/streamlit-logo-secondary-colormark-darktext.png" alt="streamlit" width="300"/>
</p>

> Convert amounts like `100 USD → EUR` in seconds!

---

## ⚙️ Installation & Setup

1. **Clone the repository**:

```bash
git clone https://github.com/your-username/currency-converter.git
cd currency-converter
```

2. **(Optional) Create a virtual environment**:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**:

```bash
pip install -r requirements.txt
```

4. **Run the app**:

```bash
streamlit run app.py
```

> The app will open in your default browser at: `http://localhost:8501`

---

## 🧾 Requirements

The required libraries are listed in `requirements.txt`. Example:

```txt
streamlit
requests
```

You can install them via:

```bash
pip install -r requirements.txt
```

---

## 🧠 How It Works

- `constants.py`: Contains a list of supported currencies (`CURRENCIES`).
- `main.py`: Contains:
  - `get_exchange_rate(base, target)` – Fetches exchange rate from API.
  - `convert_currency(amount, rate)` – Simple multiplication.
- `app.py`: The Streamlit frontend UI, calls functions and renders output.

---

## 💡 Example constants.py

```python
CURRENCIES = [
    "USD", "EUR", "GBP", "JPY", "CAD", "AUD", "INR", "CNY", "BRL", "ZAR"
]
```

---

## 📌 Notes

- You may need an API key if you're using a paid or limited-tier API provider. In such a case, add your key to `main.py`.
- Make sure to avoid naming conflicts (e.g., don’t name your file `constants.py` if a package with that name is installed globally).

---

## 🛡️ License

MIT License ©️ 2025 Your Name

---

## 🙌 Contributions

Pull requests and suggestions are welcome! Feel free to open an issue to discuss.
