# WordPress Docker Setup

This project sets up a WordPress environment using Docker. It provides an easy way to develop and test WordPress sites locally.

## Features

- WordPress and MySQL containers
- Persistent data storage
- Easy configuration with `docker-compose`
- Customizable for plugins and themes development

## Requirements

- [Docker](https://www.docker.com/) installed on your system
- [Docker Compose](https://docs.docker.com/compose/) installed

## Setup Instructions

1. Clone this repository:

    ```bash
    git clone https://github.com/your-repo/wp-docker1.git
    cd wp-docker1
    ````

2. Start the Docker containers:

   ```bash
   docker-compose up -d
   ```

3. Access WordPress in your browser:

   Open [http://localhost:8000](http://localhost:8000) in your browser.

4. Stop the containers when done:

   ```bash
   docker-compose down
   ```

## File Structure

```
wp-docker1/
├── docker-compose.yml   # Docker Compose configuration
├── wp-content/          # WordPress content directory (themes, plugins, uploads)
├── .env                 # Environment variables
└── README.md            # Project documentation
```

## Customization

* Modify the `docker-compose.yml` file to change ports or add additional services.
* Add your custom themes and plugins to the `wp-content/` directory.

## Troubleshooting

* If you encounter issues, check the container logs:

  ```bash
  docker-compose logs
  ```

* Ensure that ports `8000` (WordPress) and `3306` (MySQL) are not in use by other applications.

## License

This project is licensed under the MIT License.