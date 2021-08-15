# RBSM

## Short description about what is RBSM ?

RBSM is a simple social media API-only application based on Ruby lang. This app is used only on one small environment so no authentication is required. Where the user can input data, create a new post with a limit of 1000 characters and a maximum of one attachment. Users can also make comments, check some posts that contain certain hashtags and users can also see trending hashtags for the past 24 hours.

# Prerequisites to run the application locally

There are several things that need to be prepared to run this application locally, including:

## Requires

you can click the **link** for more detail.

1. Ruby with version `2.7.0` above. <a href="https://github.com/rbenv/rbenv">Link</a>
2. MySQL <a href="https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-20-04">Link</a>


## Setup

1. Open your terminal and clone the App :

```sh
git clone https://github.com/hafizulf/rbsm.git
```

2. Install `bundler` to get app dependencies :

```sh
cd rbsm
gem install bundler
# check if the bundle is installed properly
bundle -v
# your bundle version
```

3. Install gem from `Gemfile` with this command :
```sh
bundle install
```

4. **Import database**, make sure mysql is running :

```sh
cd db_schema
mysql -u username -p < database.sql
[Enter your password]
```

5. Run the app with this command :
```sh
cd ..
ruby app.rb
```

6. Access the App from your browser :
```
http://localhost:4567
```