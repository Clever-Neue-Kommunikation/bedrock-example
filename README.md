<h1> Getting started</h1>

<strong>Step 1: </strong>
Fork Git-Repository bedrock-boilerplate</br>
Fork Git-Repository sage-boilerplate

<strong>Step 2: </strong>
git clone [forked bedrock-boilerplate]

<strong>Step 3: </strong>
configure package.json with [forked sage-boilerplate] (repository url and require)
configure .lando.yaml (name and url)

<strong>Step 4: </strong>
lando start</br>
lando composer install

<strong>Step 5: </strong>

# Create a WordPress config file
lando wp config create \
  --dbname=wordpress \
  --dbuser=wordpress \
  --dbpass=wordpress \
  --dbhost=database \
  --path=wordpress

# Install WordPress
lando wp core install \
  --url=https://my-first-wordpress-app.lndo.site/ \
  --title="My First Wordpress App" \
  --admin_user=admin \
  --admin_password=password \
  --admin_email=admin@my-first-wordpress-app.lndo.site \
  --path=wordpress

<strong>Step 6: </strong>
Run lando yarn from the theme directory to install dependencies
Update bud.config.js with your local dev URL
lando yarn build — Compile assets




Developing this Theme



TO DO

Developing container components

