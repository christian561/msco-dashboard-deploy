


# Install dependencies 
virtualenv env
.\env\Scripts\activate
set GITHUB_TOKEN='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'
pip install -r requirements.txt

# Set Up Database
python manage.py makemigrations
python manage.py migrate

# Create SuperUser
python manage.py createsuperuser

# Start Server
python manage.py runserver



