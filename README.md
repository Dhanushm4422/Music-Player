
# Step 1: Navigate to the project directory
cd C:\Dhanush\Open-Source-Music-Player-main

# Step 2: Activate the virtual environment
.\musicEnv\Scripts\activate

# Step 3: Install dependencies (optional, but recommended)
pip install -r requirements.txt

# Step 4: Apply database migrations
python manage.py migrate

# Step 5: Create a superuser (you will be prompted to enter username & password)
python manage.py createsuperuser

# Step 6: Collect static files (optional, needed if using static files)
python manage.py collectstatic --noinput

# Step 7: Run the Django development server
python manage.py runserver
