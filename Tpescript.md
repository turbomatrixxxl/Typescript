# install

npm install -g typescript

# compilare

tsc test.ts

# monitorizare in timp real

tsc test.ts -w
tsc test.ts -watch

# initializare

tsc --init

# Run a compile based on a backwards look through the fs for a tsconfig.json crearte fisiere js

tsc

# Emit JS for just the index.ts with the compiler defaults

tsc index.ts

# Emit JS for any .ts files in the folder src, with the default settings

tsc src/\*.ts

# Emit files referenced in with the compiler settings from tsconfig.production.json

tsc --project tsconfig.production.json

# Emit d.ts files for a js file with showing compiler options which are booleans

tsc index.js --declaration --emitDeclarationOnly

# Emit a single .js file from two files via compiler options which take string arguments

tsc app.ts util.ts --target esnext --outfile index.js

# additional

npm init -y
npm i --save-dev @web/dev-server
