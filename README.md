<!DOCTYPE html>
<html>

<head>
    <title>Expense Tracker</title>
    <link rel="stylesheet" type="text/css" href="style.css" />
</head>

<body>
    <div class="container">
        <h1>Expense Tracker</h1>
        <form id="expense-form">
            <input type="text" id="expense-name" placeholder="Expense Name" required />
            <input type="number" id="expense-amount" placeholder="Amount" required />
            <select id="expense-category" required>
                <option value="" disabled selected>SELECT CATEGORY</option>
                <option value="Food">Food</option>
                <option value="Transport">Transport</option>
                <option value="Entertainment">Entertainment</option>
                <option value="Other">Other</option>
            </select>
            <input type="date" id="expense-date" required />
            <button type="submit">Add Expense</button>
        </form>
        <div class="expense-table">
            <table>
                <thead>
                    <tr>
                        <th>EXPENSE NAME</th>
                        <th>AMOUNT</th>
                        <th>CATEGORY</th>
                        <th>DATE</th>
                        <th>CALCULATE</th>
                    </tr>
                </thead>
                <tbody id="expense-list"></tbody>
            </table>
            <div class="total-amount">
                <strong>Total:</strong> $<span id="total-amount">0</span>
            </div>
        </div>
        <div class="filter">
            <label for="filter-category">Filter by Category:</label>
            <select id="filter-category">
                <option value="All">All</option>
                <option value="Food">Food</option>
                <option value="Transport">Transport</option>
                <option value="Entertainment">Entertainment</option>
                <option value="Other">Other</option>
            </select>
        </div>
    </div>
    <script src="script.js"></script>
</body>

</html>
