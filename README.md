# Grocery Store Application (Backend)

**Author:** Gaurav Ginodia  
**Email:** [gauravginodia02@gmail.com](mailto:gauravginodia02@gmail.com)

## Project Description
This project is a backend implementation of a grocery store application, similar to platforms like BigBasket and Grofers. The application manages user authentication, product management, and cart functionality, with admin controls to oversee and manage the store’s products and categories.

## Demo Video

[![Demo Video](https://img.youtube.com/vi/qdm0NxUCoUg/0.jpg)](https://youtu.be/qdm0NxUCoUg?feature=shared)

## Technologies and Frameworks Used
- **Flask**
  - `flask_login` for user authentication.
  - `flask_bcrypt` for password hashing.
  - `flask_wtf` for form handling and validation.
  - `flask_sqlalchemy` for database integration.
- **Jinja2** for templating.
- **SQLite** for database storage.
- **HTML & CSS** for frontend styling.
- **VSCode** as the development platform.

## Project Architecture
- **Main page**: `run.py`
- **Inside `app_grocery` folder**:
  - `database.py`: Manages database operations.
  - `form.py`: Manages form structure and validation.
  - `links.py`: Handles connections between forms and templates.
  - Templates (HTML) and static assets (CSS, images) are stored in the respective `templates` and `static` folders.
  - Database stored in `instance/grocery.db`.

## Features

### Admin Panel
- Login: Username = `admin`, Password = `admin`.
- Admin Dashboard: View stats on categories, products, and users.
- Category Management: Create, update, delete categories.
- Product Management: Create, update, delete products.
- Search: Search for products and categories by name.
- Additional Features: Admin confirmations, success/failure flash messages, and product image uploads.

### User Interface
- Browse products from different categories.
- Add multiple products to the cart.
- Out-of-stock products displayed with disabled add-to-cart button.
- Update and delete items in the cart.
- Grand total with a buy button that empties the cart on checkout.
- Delivery fee offer for orders above ₹500.
- Category and product search functionality.

## Database Schema
- **Category**: One-to-many relationship with **Product**.
- **Product**: Many-to-many relationship with **User** (through **Buy** table).
- **User**: Can make multiple purchases through the **Buy** table.

## Extra Features
- Cart icon added as a logo for easy navigation.
- Product information (category and expiry date) available on the info button.
- Professional look with a custom-designed logo.

## Demo Video
Watch the demo video here: [YouTube Link](https://youtu.be/qdm0NxUCoUg?feature=shared)  

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-link
   ```
2. Navigate to the project directory:
   ```bash
    cd grocery-store-backend
   ```

3. Install dependencies:
   ```bash
    pip install -r requirements.txt
   ```

4. Run the application:
   ```bash
    python run.py
   ```

5. Open your browser and go to http://127.0.0.1:5000
