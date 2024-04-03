
# Running Locally

## virtual enviroment
py -3.12 -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt

## install django locally and other libraries
pip install django

## make directory structures
django-admin startproject mysite

## run local server
python manage.py runserver

python manage.py startapp appname



# cookie cutter

pip install cookiecutter
cookiecutter https://github.com/pydanny/cookiecutter-django
pip install -r requirements/base.txt


# tailwind 
cd your_project
npm install -D tailwindcss
npx tailwindcss init

# tailwind.config.js
module.exports = {
 content: [
        // Main Templates
        './your_project/templates/*.html',
        './your_project/templates/**/*.html',

        // Add other app's templates here
        //  './your_project/your_app/templates/*.html',
        // './your_project/your_app/templates/**/*.html',
    ],


  theme: {
    extend: {},
  },
  plugins: [],
};



# static/css  tailwind.css

@tailwind base;
@tailwind components;
@tailwind utilities;


# Build, run in another terminal
npx tailwindcss-cli@latest build ./your_project/static/tailwind.css -o ./your_project/static/css/style.css --watch

npx tailwindcss-cli@latest build ./dj_templates/static/tailwind.css -o ./dj_templates/static/css/style.css --watch