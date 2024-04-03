npm install -D tailwindcss
npx tailwindcss init

agregar   content: ["./src/**/*.{html,js}"], 
a tailwind.config.js


crea archivo src/input.css
con directivos de tailwind

@tailwind base;
@tailwind components;
@tailwind utilities;



Start the Tailwind CLI build process

npx tailwindcss -i ./src/input.css -o ./src/output.css --watch


