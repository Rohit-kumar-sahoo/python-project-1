# python-project-1
Loan Calculator (Python)

A simple yet precise Loan Calculator Application built in Python using the decimal module for accurate financial computations.
This program calculates monthly payments, total interest, and provides an amortization schedule for the first 12 months of a loan.

🚀 Features

💰 Calculate monthly payments based on principal, interest rate, and loan term.

📅 Generate an amortization schedule showing the breakdown of interest and principal.

📊 Display total interest paid and total loan cost over the full term.

✅ Handles both zero-interest and standard interest loans.

🔒 Uses Python’s decimal module for accurate rounding and precision in financial calculations.

🧩 How It Works

The calculator uses the standard amortization formula:

𝑀
=
𝑃
×
𝑟
(
1
+
𝑟
)
𝑛
(
1
+
𝑟
)
𝑛
−
1
M=P×
(1+r)
n
−1
r(1+r)
n
	​


Where:

M = Monthly payment

P = Loan principal

r = Monthly interest rate (annual rate ÷ 12)

n = Total number of payments (years × 12)

If the interest rate is 0, it evenly divides the loan over the term.

⚙️ Requirements

Python 3.7+

No external dependencies (uses only the Python standard library)

🏃‍♂️ Usage

Clone the repository:

git clone https://github.com/your-username/loan-calculator.git
cd loan-calculator


Run the program:

python loan_calculator.py


Follow the prompts:

=== Loan Calculator Application ===

Choose an option:
1. Calculate a new loan
2. Exit

Enter your choice: 1
Enter loan amount: 10000
Enter annual interest rate (e.g., 4.5 for 4.5%): 5
Enter loan term in years: 5
Enter a description for this loan: Car Loan


The app will display:

Monthly payment

Total interest

Total cost

First 12 payments of the amortization schedule

🧾 Example Output
Car Loan
--------------------------------------------------
Loan Amount: $10,000
Monthly Payment: $188.71
Total Interest: $1,322.74
Total Cost: $11,322.74

First 12 Payments:
Pmt   Payment      Interest   Principal  Balance     
--------------------------------------------------
1     $188.71      $41.67     $147.04    $9,852.96  
2     $188.71      $41.05     $147.66    $9,705.30  
...
12    $188.71      $34.38     $154.33    $8,162.54  

📦 File Structure
loan-calculator/
│
├── loan_calculator.py   # Main application file
└── README.md            # Documentation

🧠 Key Classes & Methods
Class / Function	Description
LoanCalculator	Main class handling loan calculations and schedules
calculate_monthly_payment()	Computes fixed monthly payment
generate_amortization_schedule()	Generates a detailed schedule of payments
total_interest_paid()	Returns total interest paid over the life of the loan
get_valid_input()	Handles user input validation
main()	CLI loop for user interaction
🪪 License

This project is licensed under the MIT License — feel free to use, modify, and distribute it.

💡 Future Enhancements (Optional Ideas)

Export amortization schedule to CSV or Excel

Support for bi-weekly or extra payments

Add a GUI using Tkinter or Streamlit

Visualization of interest vs. principal over time
