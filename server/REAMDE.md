# .net core build and deploy for heroku
* Reference: https://medium.com/null-exception/deploy-net-core-app-to-heroku-a22a04f107c9

## Steps
1. Create .net core app with Docker
2. Modify Program.cs for running with $PORT env
3. heroku login
4. heroku container:login
5. heroku container:push web --app={myapp}
6. heroku container:release web --app={myapp}
7. heroku logs -f --app={myapp}