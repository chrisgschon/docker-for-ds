# docker-for-ds
An example of how Docker can be used to develop a data science project, with detailed walkthrough and blog post


# 🔑 Walkthrough


# 🆙 Starting with Docker

docker-compose build
docker-compose up -d

docker-compose exec app bash

jupyter notebook --ip 0.0.0.0 --no-browser --allow-root


Build the image locally:

```docker build -t ds . ```


- Then on your host's terminal, run:

```docker run --rm -it -p 8888:8888 ds```

- In the container

```jupyter notebook --ip 0.0.0.0 --no-browser --allow-root```

- using the provided token, enter this into your browser

```http://localhost:8888/?token=URTOKEN```

- run ETL script


✅This is a security measure to make sure websites can't access your code and data!
