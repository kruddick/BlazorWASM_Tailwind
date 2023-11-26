dotnet new blazorwasm-empty -o BlazorWithTailwind
npx tailwindcss init

mkdir wwwroot/css/style
touch wwwroot/css/style/tailwind.css

add:
@tailwind base;
@tailwind components;
@tailwind utilities;

change tailwind.config.js:
content: ['./**/*.{razor,html}']

from project folder:

npx tailwindcss -i ./wwwroot/css/style/tailwind.css -o ./wwwroot/css/tailwind.css --watch