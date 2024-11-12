<h1> Getting started</h1>

Schritt 1: 
Fork Git-Repository bedrock-boilerplate
Fork Git-Repository sage-boilerplate

Schritt 2:
git clone [forked bedrock-boilerplate]

Schritt 3:
configure package.json with [forked sage-boilerplate] (repository url and require)
configure .lando.yaml (name and url)

Schritt 4:
lando start
lando composer install

Schritt 5:
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

Schritt 6:
Run lando yarn from the theme directory to install dependencies
Update bud.config.js with your local dev URL
lando yarn build — Compile assets




Developing this Theme



TO DO

Developing container components

