# Install
docker-compose build --no-cache
docker-compose up -d
docker exec -i db_example_wp mysql -u root -p'root!10000' wordpress < db/wordpress_db.sql

# Remove
docker-compose down
docker volume rm wordpress-example_db
docker volume rm wordpress-example_wordpress