# PropertyConnect
### Find. Match. Connect. Home.
**Property Listing, Matching and Management System**

Live Demo: `https://karabopriskykalunga-beep.github.io/propertyconnect-final/`
> Change this link to your new repo name after you create it.

---

## 👥 Team
- **Karabo Elias Kalunga** - Lead Dev, QA (Main Admin)
- **Malesa Letsobana** - UI/UX
- **Gavaza Mashaba** - Backend
- **Thapelo Swana** - DBA
- **Tlhotlhonya Maponya** - JS Dev
- **Nkokae Maponya** - QA / Docs

## 🎯 What It Does
PropertyConnect helps NSFAS students and luxury buyers find houses in all 9 provinces of South Africa.

- **NSFAS Students:** Rooms R1 800 - R4 500 (Pretoria, Johannesburg, Durban, Polokwane, Cape Town)
- **Luxury Buyers:** Villas R3.5M - R10.5M (Limpopo, Pretoria, Johannesburg, Durban, Cape Town)

## ✨ Features in this Final Version
- **Signup (2 Steps):** Personal + Address & Banking, Role: Client / Owner
- **Login + Forgot Password:** Verified with Email + Bank Account
- **Profile:** Click top-right tag to edit name, phone, bank, password
- **Dashboard:** Search by location, Province tabs (9 Provinces), City + House Type filter
- **Preference:** Save province / type / max budget, auto-filters on next login
- **Filter + Filter Records:** Every filter/search is saved in `filter_history`
- **Favourites:** ❤️ Save / Remove
- **Buy / Rent:** Generates reference `PC-XXXXXX`, pays to owner bank, listing removed
- **Viewing Requests - 2 WAY:** Client sends → Owner / Admin **Approve / Decline / Reply** → Client sees green reply box
- **Enquiries - 2 WAY:** Client sends → Owner replies
- **Reports - 2 WAY:** Client reports scam → Admin **Reply / Resolve / Delete** → Client sees admin reply
- **My History:** Viewings + Purchases + Enquiries + Favourites
- **System Log:** Every action logged (LOGIN, SEARCH, BUY, REPORT, etc.)
- **Security:** Change password, Change bank, Delete account
- **Admin Management:** Main Admin `karabopriskykalunga@gmail.com` can Make / Remove Admin, Delete User, Delete Listing, View All Reports + Viewings

## 🛠️ Languages Used (4)
| Language | Used For |
| --- | --- |
| HTML | Structure, Pages, Modals |
| CSS | Styling, Yellow / Dark Theme, Mobile Layout |
| JavaScript | Logic, Supabase Connection, All Features |
| SQL (PostgreSQL) | Database Tables in Supabase |

## 🗄️ Database (Supabase)
Tables: `users`, `listings`, `transactions`, `visits`, `favorites`, `viewing_requests`, `enquiries`, `reports`, `logs`, `filter_history`

## 🚀 How To Run
### Option 1 - GitHub Pages (Live)
1. Open live link above
2. Create Account → Login
3. Browse, Search, Favourite, View, Enquire, Report

### Option 2 - Local
1. Download `index.html`
2. Double-click to open in browser
3. Internet needed for Supabase connection

## 🔑 Test Accounts
- **Admin:** `karabopriskykalunga@gmail.com` / password you set in Supabase `users` table
- **Client:** Sign Up as a new user, Role = Client
- **Owner:** Sign Up as a new user, Role = Owner

## ⚙️ Setup - New Supabase (If you clone this)
1. Create new project in Supabase
2. SQL Editor → Run the SQL in `SUPABASE_SETUP.sql` (or create the 10 tables above)
3. Copy Project URL + Publishable Key
4. In `index.html`, replace:
```js
const SUPABASE_URL = "YOUR_NEW_URL";
const SUPABASE_KEY = "YOUR_NEW_KEY";