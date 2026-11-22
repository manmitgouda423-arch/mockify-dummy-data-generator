# Mockify – Dummy Data Generator

Mockify is a browser-based developer utility for generating realistic, strictly fictional test datasets for frontend development, API mocking, QA workflows, and database seeding.

All records are generated locally in the browser using `@faker-js/faker` and stored only in `localStorage`.

## Features

- **5 Data Categories**:
  - **User Information**: Full name, email (`example.com` / `example.org` / `mockdata.test`), username, fictional `555-01XX` phone number, gender, date of birth, address, city, country.
  - **Product Information**: Product ID, product name, category, price, description, stock quantity, rating.
  - **Company Information**: Company name, industry, synthetic website, email, employee count.
  - **Financial Test Data**: Transaction ID, amount, ISO currency, payment status, transaction date.
  - **Custom Data**: Dynamic schema builder supporting `Text`, `Number`, `Email`, `Boolean`, and `Date` field types.
- **Record Configuration**: Generate between `1` and `1,000` records with live input validation, field toggles, custom SQL table naming, and optional deterministic Faker seeding.
- **Interactive Data Preview**: Search across columns, sort ascending/descending, paginate results (`10`, `25`, `50`, `100` rows per page), and switch between Table, JSON, CSV, and SQL views.
- **Clean Exports**: Download valid `.json`, RFC 4180 escaped `.csv`, and safely escaped `INSERT INTO ...` `.sql` files.
- **Granular Copy Actions**: Copy individual cell values, single JSON records, or the entire dataset with toast confirmation.
- **Local History & Settings**: Automatically save datasets in `localStorage` with quota protection, reopen or export past datasets, and customize JSON indentation, CSV delimiters, and SQL identifier quoting.

## Tech Stack

- **Frontend**: React 19, TypeScript, Vite
- **Styling**: Tailwind CSS v4
- **Data Engine**: `@faker-js/faker`
- **Icons**: `lucide-react`
- **Persistence**: Browser `localStorage`

## Local Setup

```bash
# 1. Install dependencies
npm install

# 2. Start the development server on port 3000
npm run dev

# 3. Build for production
npm run build
```
