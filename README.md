<p align="center">
    <img src="https://i.imgur.com/RdUFiBv.png" style="padding: 2rem"/>
</p>

<p align="center">
    <a href="https://packagist.org/packages/nicestdev/mew">
        <img src="https://img.shields.io/packagist/dt/nicestdev/mew" alt="Total Downloads">
    </a>
    <a href="https://packagist.org/packages/nicestdev/mew">
        <img src="https://img.shields.io/packagist/v/nicestdev/mew" alt="Latest Stable Version">
    </a>
    <a href="https://packagist.org/packages/nicestdev/mew">
        <img src="https://img.shields.io/packagist/l/nicestdev/mew" alt="License">
    </a>
</p>

## About Mew

Mew is a small and simple tool and acts as a terminal command forwarder.

## Install

This CLI application is installed using [Composer](https://getcomposer.org):

```bash
composer global require nicestdev/mew
```

Make sure the `~/.composer/vendor/bin` directory is in your systems `PATH`.

## Configuration

Create a .env file in the root path of your project and set the name of the web container. You can find your container names via `docker ps -l`

```bash
PROJECT_NAME=<CONTAINER-NAME>
```

## Usage

Mew will forward all commands to the docker container and shows the output

```bash
mew pwd
mew npm --version
mew artisan optimize
```

## Update

```bash
composer global update nicestdev/mew
```

## Delete

```bash
composer global remove nicestdev/mew
```

## License

Mew is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
