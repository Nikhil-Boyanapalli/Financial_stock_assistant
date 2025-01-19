# Financial Stock Assistant 📈

The **Financial Stock Assistant** is a Streamlit-based chatbot application designed to provide users with real-time stock analysis, including stock prices, technical indicators (e.g., SMA, EMA, RSI, MACD), and visualizations. It leverages OpenAI's GPT-3.5-turbo for intelligent conversational interactions and Yahoo Finance for stock market data.

---

## Features

- **Real-Time Stock Price**: Fetch the latest closing price of a stock.
- **Simple Moving Average (SMA)**: Calculate the SMA for a specified time window.
- **Exponential Moving Average (EMA)**: Compute the EMA for a given timeframe.
- **Relative Strength Index (RSI)**: Measure the momentum of stock price changes.
- **MACD Analysis**: Generate MACD, signal, and histogram values for technical analysis.
- **Stock Price Visualization**: Plot the stock's closing price over the past year.

---

## Requirements

Ensure you have the following installed on your system:

- Python 3.7 or higher
- The following Python libraries:
  - `openai`
  - `streamlit`
  - `pandas`
  - `matplotlib`
  - `yfinance`

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Nikhil-Boyanapalli/Financial_stock_assistant.git
   cd Financial_stock_assistant
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add your OpenAI API Key:
   - Save your API key in a file named `API_KEY` in the project directory.

---

## Usage

1. Run the Streamlit application:
   ```bash
   streamlit run main.py
   ```

2. Open the application in your web browser using the URL provided in the terminal (e.g., `http://localhost:8501`).

3. Enter your queries in natural language, such as:
   - "What is the current price of AAPL?"
   - "Calculate the SMA for TSLA over a 20-day window."
   - "Plot the stock price of MSFT."

---

## Functions Overview

| **Function**       | **Description**                                                                                  | **Parameters**                   |
|---------------------|--------------------------------------------------------------------------------------------------|----------------------------------|
| `get_stock_price`   | Retrieves the latest stock price for a given ticker symbol.                                      | `ticker` (string)               |
| `calculate_SMA`     | Calculates the Simple Moving Average (SMA) over a given window.                                 | `ticker` (string), `window` (int)|
| `calculate_EMA`     | Calculates the Exponential Moving Average (EMA) for a specified time window.                    | `ticker` (string), `window` (int)|
| `calculate_RSI`     | Computes the Relative Strength Index (RSI) for a given stock.                                   | `ticker` (string)               |
| `calculate_MACD`    | Calculates the MACD, signal, and histogram values.                                              | `ticker` (string)               |
| `plot_stock_price`  | Plots the closing stock price over the last year.                                               | `ticker` (string)               |

---

## Example Query Flow

1. **User Input**: "Show me the MACD for AAPL."
2. **Function Execution**: The application computes MACD values and displays them.
3. **Assistant Output**: The assistant provides a response based on the computed values.

---

## File Structure

```
Financial_stock_assistant/
├── main.py           # Main application code
├── requirements.txt  # List of dependencies
├── API_KEY           # File containing the OpenAI API key
└── README.md         # Project documentation
```

---

## Future Enhancements

- Support for additional technical indicators.
- Integration with more stock data providers.
- Advanced visualization features like candlestick charts.
- Improved natural language understanding for diverse queries.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests for bug fixes, improvements, or feature requests.

---

## Acknowledgments

- [Streamlit](https://streamlit.io/)
- [OpenAI API](https://platform.openai.com/)
- [Yahoo Finance API](https://pypi.org/project/yfinance/)

