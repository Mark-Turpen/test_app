```bash
docker run --rm -it --volume "$(pwd):/csce431" -e DATABASE_USER=test_app -e DATABASE_PASSWORD=test_password -p 3000:3000 dmartinez05/ruby_rails_postgresql:latest

```

```bash
rails db:create
rails db:migrate
rails server --binding=0.0.0.0
rails g scaffold Book title:string
```