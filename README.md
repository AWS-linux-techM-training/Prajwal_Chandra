# Simple Library Management System

## Overview
The Simple Library Management System is designed to manage the various aspects of a library, including book management, patron management, circulation, acquisitions, and reporting. This system helps streamline library operations and improve efficiency.

## Database Structure

### Database 1: Book Management
- **Books**: `id`, `title`, `author`, `publication_date`, `ISBN`
- **Authors**: `id`, `name`, `biography`
- **Publishers**: `id`, `name`, `address`
- **Genres**: `id`, `name`, `description`
- **Book Genres**: `id`, `book_id`, `genre_id`

### Database 2: Patron Management
- **Patrons**: `id`, `name`, `email`, `phone_number`, `address`
- **Membership Types**: `id`, `name`, `description`, `duration`
- **Patron Membership**: `id`, `patron_id`, `membership_type_id`, `start_date`, `end_date`
- **Patron Fines**: `id`, `patron_id`, `fine_amount`, `fine_date`
- **Patron Payments**: `id`, `patron_id`, `payment_amount`, `payment_date`

### Database 3: Circulation Management
- **Checkouts**: `id`, `book_id`, `patron_id`, `checkout_date`, `due_date`
- **Returns**: `id`, `checkout_id`, `return_date`
- **Holds**: `id`, `book_id`, `patron_id`, `hold_date`, `expiration_date`
- **Waitlists**: `id`, `book_id`, `patron_id`, `waitlist_date`
- **Checkout History**: `id`, `book_id`, `patron_id`, `checkout_date`, `return_date`

### Database 4: Acquisitions Management
- **Orders**: `id`, `book_id`, `quantity`, `order_date`, `total_cost`
- **Vendors**: `id`, `name`, `address`, `contact_info`
- **Order Items**: `id`, `order_id`, `book_id`, `quantity`, `cost`
- **Receipts**: `id`, `order_id`, `receipt_date`, `total_cost`
- **Invoices**: `id`, `order_id`, `invoice_date`, `total_cost`

### Database 5: Reporting and Analytics
- **Circulation Stats**: `id`, `date`, `total_checkouts`, `total_returns`
- **Collection Stats**: `id`, `date`, `total_books`, `total_authors`
- **Patron Stats**: `id`, `date`, `total_patrons`, `total_membership`
- **Fine Stats**: `id`, `date`, `total_fines`, `total_payments`
- **Survey Responses**: `id`, `date`, `question_id`, `response_text`

## Clone the repository:
   ```bash
   git clone https://github.com/Prajwal122003/library_management_system
```

## Presentation 
  ```bash
  https://www.canva.com/design/DAF2TIcBFP4/2vnS82ERYwQV_oaNUP8RPw/view?utm_content=DAF2TIcBFP4&utm_campaign=designshare&utm_medium=link&utm_source=editor
```
