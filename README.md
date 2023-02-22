# Laravel PHP 7.4 with PHP-FPM, Nginx, and MySQL Docker Compose

This repository contains a Docker Compose setup for a Laravel PHP 7.4 application with PHP-FPM, Nginx, and MySQL.

## Requirements
* Docker and Docker Compose
* Git
* Laravel 5.7

## Getting started

1. Clone this repository to your local machine:

```$ git clone https://github.com/<username>/laravel-docker-compose.git```

2. Change into the cloned directory:

```$ cd laravel-docker-compose```

3. Build the Docker containers and start the services:
```$ docker-compose up -d```

This command will download the required images and start the containers in the background. The -d flag is optional and runs the containers in the background.

4. Access the Laravel application in your web browser at http://localhost:8000.

## File Structure
```
.
├── Dockerfile
├── docker-compose.yml
├── docker-compose
│   ├── mysql
│   │   ├── data
│   │   └── initdb.d
│   └── nginx
│       └── nginx.conf
├── logs
└── ...
```

## Customizing the setup
You can modify the environment variables, ports, and other settings in the `docker-compose.yml` file.

## Stopping the containers
To stop the running containers, use the following command:
```$ docker-compose down```

## (Re)starting the containers
To restart the containers, use the following command:
```$ docker-compose up -d```

## Contributing
Contributions are welcome! Please fork this repository and open a pull request to add or improve any features.
1. Fork it
2. Create your feature branch (git checkout -b feature/my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin feature/my-new-feature)
5. Create a new Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.
