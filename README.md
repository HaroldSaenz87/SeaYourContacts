# SeaYourContacts

A full-stack contact management web application built with HTML, CSS, JavaScript, and PHP (LAMP stack). Users can create accounts, log in securely, and manage a personal contact list with full CRUD functionality.

---

## ✨ Features

- **User Authentication** — Sign up and sign in with MD5-hashed passwords
- **Add Contacts** — Save contacts with first name, last name, email, and phone number
- **Search Contacts** — Live search as you type, with optional filters for first name, last name, email, or phone
- **Edit Contacts** — Update contact details via an animated modal
- **Delete Contacts** — Confirm and delete contacts via a delete confirmation modal
- **Session Management** — User sessions persist via `sessionStorage`; unauthenticated users are redirected to the login page
- **Phone Formatting** — Phone numbers are automatically formatted as `555-555-5555`

---

## 🛠️ Tech Stack

| Layer     | Technology                     |
|-----------|-------------------------------|
| Frontend  | HTML5, CSS3, Vanilla JavaScript |
| Backend   | PHP                            |
| Database  | MySQL (via `mysqli`)           |
| Server    | Apache (LAMP stack)            |
| Fonts     | Google Fonts — Quicksand       |

---

## 🔒 Security Notes

- Passwords are hashed on the client side using MD5 before being sent to the server. For production use, it is strongly recommended to switch to a server-side hashing algorithm such as `bcrypt` via PHP's `password_hash()`.
- All database queries use **prepared statements** with bound parameters to prevent SQL injection.
- Contact deletion verifies both the contact `ID` and the `userID` to prevent unauthorized deletions.

---

## 📸 Pages

### Login / Sign-up (`index.html`)
A sliding panel UI where users can toggle between signing in and creating a new account.

### My Contacts (`account.html`)
The main dashboard where users can add, search, filter, edit, and delete their contacts. Includes animated modals for editing and deleting contacts.

---

## 👥 Contributors

| Name             | Role                                        |
|------------------|---------------------------------------------|
| Harold           | Frontend Development                        |
| Rae              | API Development                             |
| Nicholas         | API Development                             |
| Nia              | Database                                    |
| Sreeja           | Project Manager / Frontend Development      |

### Frontend Contributions
- Designed and built the login/sign-up sliding panel UI (`index.html`, `login.css`)
- Built the contacts dashboard layout and styling (`account.html`, `account.css`)
- Implemented animated edit and delete modals
- Added live search with filter dropdown
- Created contact cards with hover effects and fade-in animations
- Added underwater/ocean theme with animated shark and diver decorations
- Integrated Google Fonts (Quicksand) and responsive layout

---

## DEMO
[▶ Watch Demo](https://drive.google.com/file/d/1SkjKbnJ2VyLiusSuEOW6Da2L1gU7hWGE/view?usp=sharing)

## 📄 License

This project was built for educational purposes
