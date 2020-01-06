first install npm and nodejs

then install create-react-app
after run create-react-app frontend
here frontend is project name

first build image

docker build -t sri596/reactsample:1 -f Dockerfile.dev .


to run container


docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app -d sri596/reactsample:1

volumes 
-v /app/node_modules means don't map this folder to container
