# 🍽️ Eat-N-Split (React)

A simple and interactive **bill-splitting application** built using React.
This app allows users to split expenses with friends and keep track of balances in a clean and intuitive way.

---

## 📌 Overview

Eat-N-Split helps users manage shared expenses by:

- Adding friends
- Selecting a friend to split a bill
- Calculating who owes whom
- Updating balances dynamically

This project focuses on **core React concepts like lifting state up, props-based communication, and controlled components**.

---

## ✨ Features

- 👥 Add new friends
- 💸 Split bills with selected friend
- 🔄 Automatically calculate balances
- 📊 Track who owes money
- ⚡ Instant UI updates
- 🎯 Simple and user-friendly interface

---

## 🧠 Key Concepts Implemented

### 🔹 Lifting State Up

- Centralized state in the parent component
- Shared data across multiple child components
- Controlled which friend is selected and updated balances globally

---

### 🔹 Props & Data Flow

- Passed **data (friend list, balances)** from parent → child
- Passed **functions (handlers)** to allow child → parent updates
- Maintained unidirectional data flow

---

### 🔹 Controlled Components

- Managed form inputs (bill value, user expense) via state
- Ensured UI stays in sync with data

---

## 🔄 Data Flow (How It Works)

```id="flow-eat"
User Action (Child Component)
        ↓
Calls Handler Function (via props)
        ↓
Parent State Updates
        ↓
Updated Data Passed Back as Props
        ↓
UI Re-renders Automatically
```

---

## 🧩 Component Structure

```id="structure-eat"
App (State Owner)
│
├── FriendList
│   └── Friend
│
├── FormAddFriend
│
└── FormSplitBill
```

👉 The **App component acts as the single source of truth**, managing:

- Friends list
- Selected friend
- Balances

---

## ⚙️ How It Works (Logic)

- User selects a friend
- Enters bill amount and expenses
- App calculates:
  - Who paid more
  - Who owes money

- Updates the balance accordingly

---

## 🛠️ Tech Stack

- **React** (Functional Components + Hooks)
- **JavaScript (ES6+)**
- **CSS**

---

## ⚙️ Installation & Setup

1. Clone the repository:

```bash id="clone-eat"
git clone https://github.com/SuryaTejaTangella/Eat-N-Split.git
```

2. Navigate to the project:

```bash id="cd-eat"
cd Eat-N-Split
```

3. Install dependencies:

```bash id="install-eat"
npm install
```

4. Run the app:

```bash id="run-eat"
npm start
```

---

## 🚀 Future Enhancements

- 💾 Persist data using local storage
- 📱 Improve mobile responsiveness
- 🔍 Add search/filter for friends
- 📊 Expense history tracking

---

## 👨‍💻 Author

**Surya Teja Tangella**
Aspiring Software Developer | Java Backend + React
Transitioning from Banking → IT / FinTech

---

## ⭐ Show Your Support

If you like this project, consider giving it a ⭐ on GitHub!
