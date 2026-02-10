# 🤖 Smart-Budget-Ollama

<div align="center">

![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Ollama](https://img.shields.io/badge/Ollama-qwen2.5:14b-orange.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

**An AI-powered personal finance manager that understands natural language**

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Examples](#-examples) • [Contributing](#-contributing)

</div>

---

## 📖 About

**Smart-Budget-Ollama** is an intelligent command-line financial management system that leverages **Ollama** and **Qwen 2.5 (14B)** to process natural language inputs and convert them into structured financial data. No more manual categorization or complex interfaces—just type what you spent or earned, and let AI do the rest!

This project demonstrates:
- 🧠 **LLM Integration** for natural language understanding
- 💰 **Personal Finance Management** with automatic categorization
- 📊 **Data Analytics** with visual reports and insights
- 🎯 **Goal Tracking** to help you achieve financial objectives
- 🔒 **Privacy-First** approach (all data stored locally)

> **Note:** This project is open for collaboration! I'm looking for like-minded developers who want to build and learn together, not for employment.

---

## ✨ Features

### 🎙️ Natural Language Processing
- Type expenses and income in plain English
- AI automatically categorizes transactions
- Supports multiple transaction formats
- Handles currency conversions

### 📊 15 Expense Categories
```
Restaurant Food • Cafe & Beverages • Groceries • Public Transport
Taxi & Ride-share • Gas & Parking • Clothing • Cosmetics
Medicine • Utility Bills • Internet & Mobile • Entertainment
Books & Education • Gifts • Other
```

### 💵 9 Income Categories
```
Salary & Wages • Bonus & Tips • Sale of Goods • Investment Income
Gift Received • Loan & Borrowing • Refund • Part-time Work • Other
```

### 📈 Analytical Queries
- **Budget Status**: View your current financial state
- **Expense by Category**: Detailed breakdown with visual bars
- **Income Summary**: Track all your income sources
- **Recent Transactions**: Quick overview of latest activities
- **Target Distance**: See how far you are from your savings goals
- **Smart Reports**: AI-powered financial insights

### 🎯 Goal Tracking
- Set multiple financial goals (car, house, vacation, etc.)
- Track progress automatically
- Get notified when goals are achieved

---

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- [Ollama](https://ollama.ai/) installed and running
- Qwen 2.5 (14B) model pulled

### Step 1: Clone the Repository
```bash
git clone https://github.com/SAEED.S.M/Smart-Budget-Ollama.git
cd Smart-Budget-Ollama
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Install Ollama and Pull Model
```bash
# Install Ollama (if not already installed)
# Visit: https://ollama.ai/

# Pull the Qwen 2.5 14B model
ollama pull qwen2.5:14b
```

### Step 4: Run the Application
```bash
python financial_manager_usd.py
```

---

## 💡 Usage

### Setting Your Budget
```
💬 I have $5000 in my account
✅ Current budget updated: $5,000.00
```

### Recording Expenses
```
💬 Spent 45 dollars at Starbucks
✅ Expense recorded: Cafe & Beverages - $45.00
💰 Current Balance: $4,955.00
```

### Recording Income
```
💬 Received my salary today, 6000 dollars
✅ Income recorded: Salary & Wages - $6,000.00
💰 Current Balance: $10,955.00
```

### Setting Financial Goals
```
💬 I want to buy a MacBook Pro for 2500 dollars
✅ New goal added: macbook with price $2,500.00
📌 Current number of goals: 1
```

### Analytical Queries
```
💬 Show me my expenses by category
💬 How far am I from my goals?
💬 What's my budget status?
💬 Show recent transactions
💬 Summarize my income
```

---

## 📸 Examples

### Expense Breakdown
```
======================================================================
💸 Total Expenses: $3,456.78
======================================================================
💰 Current Balance: $7,498.22
======================================================================

📊 Expenses by Category:

 0. Restaurant Food           │████████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░│  24.5% │     $847.12
 1. Cafe & Beverages          │████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│  16.2% │     $560.00
 2. Supermarket & Groceries   │██████████████░░░░░░░░░░░░░░░░░░░░░░░░░░│  28.3% │     $978.45
 3. Public Transportation     │███░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│   5.8% │     $200.50
...
```

### Goal Progress
```
📊 Distance to Goals:
💰 Current Budget: $7,498.22

1. macbook:
   🎯 Target Price: $2,500.00
   ✅ Goal achieved! ($4,998.22 extra)

2. car:
   🎯 Target Price: $15,000.00
   📉 Remaining: $7,501.78 (50.0% remaining)
```

---

## 🛠️ Tech Stack

- **Python 3.8+** - Core programming language
- **Ollama** - Local LLM inference engine
- **Qwen 2.5 (14B)** - Large language model for NLU
- **CSV** - Transaction storage
- **JSON** - State management

---

## 📁 Project Structure

```
Smart-Budget-Ollama/
│
├── financial_manager_usd.py    # Main application
├── transactions.csv            # Transaction history (auto-generated)
├── financial_state.json        # Budget & goals state (auto-generated)
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
└── LICENSE                     # MIT License
```

---

## 🎯 Roadmap

- [ ] Multi-currency support with real-time exchange rates
- [ ] Export reports to PDF/Excel
- [ ] Recurring transactions (subscriptions, bills)
- [ ] Data visualization with charts and graphs
- [ ] Budget limits and alerts
- [ ] Mobile app integration
- [ ] Cloud sync (optional, privacy-focused)
- [ ] Custom AI model fine-tuning
- [ ] Multi-user support for families
- [ ] Integration with bank APIs (read-only)

---

## 🤝 Contributing

I'm looking for **collaborators** who want to learn and build together! This is not a job posting—I'm seeking partners who are passionate about:
- AI/LLM applications
- Personal finance technology
- Open-source development
- Learning by doing

### How to Contribute

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Contribution Ideas
- Add new analytical queries
- Improve the AI prompt engineering
- Create data visualizations
- Add export features
- Write tests
- Improve documentation
- Build a web interface
- Create mobile app

---

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Saeed Samad Motlagh**

- GitHub: [@SAEED.S.M](https://github.com/SAEED.S.M)
- GitHub ID: `saee87d`
- Email: saeed.samad.motlagh@gmail.com

---

## 🌟 Support

If you find this project helpful, please consider:
- ⭐ Starring the repository
- 🐛 Reporting bugs
- 💡 Suggesting new features
- 🤝 Contributing code
- 📢 Sharing with others

---

## 🙏 Acknowledgments

- [Ollama](https://ollama.ai/) - For making local LLM inference accessible
- [Alibaba Cloud](https://qwenlm.github.io/) - For the amazing Qwen models
- The open-source community - For inspiration and tools

---

## ⚠️ Disclaimer

This is a personal finance tool for educational and personal use. Always consult with financial professionals for serious financial decisions. Your data is stored locally and never transmitted to external servers (except for LLM inference through Ollama).

---

<div align="center">

**Built with ❤️ by developers, for developers**

If you're interested in collaborating on this or future projects, reach out!

[⬆ Back to Top](#-smart-budget-ollama)

</div>
