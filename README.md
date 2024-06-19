# Army Encoder Django App

This Django application encodes messages based on whether the day is odd or even. The user can select the day type and input their message, which will be encoded accordingly.

## Encoding Rules
- **Odd Days:**
  - `A` = 01
  - `B` = 02
  - `C` = 03
  - ...
  - `Z` = 26

- **Even Days:**
  - `A` = 501
  - `B` = 502
  - `C` = 503
  - ...
  - `Z` = 526

## Requirements

- Python 3.x
- Django 3.x or higher

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/bsshreesha2003/armyencoder.git
    cd indian_army
    ```

2. **Create and activate a virtual environment:**
    ```bash
    python -m venv myvenv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages:**
    ```bash
    pip install django
    ```

4. **Create and apply migrations:**
    ```bash
    python manage.py migrate
    ```

5. **Run the development server:**
    ```bash
    python manage.py runserver
    ```

## Usage

1. Open your web browser and go to `http://127.0.0.1:8000/`.

2. You will see a form where you can input a message and select the day type (odd or even).

3. Click the "Encode" button to encode the message.

4. The encoded message will be displayed on a new page.

## Project Structure

- `indian_army/` - The main Django project directory.
- `app58/` - The Django app containing the encoding logic.
  - `templates/encoder/` - Directory for HTML templates.
  - `forms.py` - Contains the form used for input.
  - `views.py` - Contains the view logic for encoding the message.
  - `urls.py` - URL configurations for the encoder app.
- `manage.py` - Django's command-line utility.

## Example

### Input
- **Message:** "Attack submarine near Karachi"
- **Day Type:** Odd

### Output
