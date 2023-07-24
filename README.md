[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

<!-- PROJECT HEADER -->
<br />
<p align="center">
  <h3 align="center">🔒 Vaultwarden</h3>

  <p align="center">
    ·
    <a href="https://github.com/Good-Games-Munich/vaultwarden/issues">Report Bug</a>
    ·
    <a href="https://github.com/Good-Games-Munich/vaultwarden/issues">Request Feature</a>
    ·
  </p>
</p>

<!-- ABOUT THE PROJECT -->

## About The Project

Setup for vaultwarden an unofficial Bitwarden compatible server.

## Setup

### Production

Will be documented when github action is documented.

### Development

1. Follow the [Customization](#customization) section and set all variables with `Required in dev` `true`.
2. Run `docker-compose up --build`
3. Navigate to `http://localhost:3300`

### Customization

Create a environment file `touch .env.local`. Override variables in the `{variable name}={variable value}` format. All required variables need to be overridden for the respected environment.

| Variable        | Description                                                  | Required in dev | Required in prod | Default value |
| --------------- | ------------------------------------------------------------ | --------------- | ---------------- | ------------- |
| `SMTP_HOST`     | SMTP host.                                                   | `true`          | `true`           | none          |
| `SMTP_FROM`     | SMTP from email.                                             | `true`          | `true`           | none          |
| `SMTP_USERNAME` | SMTP username.                                               | `true`          | `true`           | none          |
| `SMTP_PASSWORD` | SMTP password.                                               | `true`          | `true`           | none          |
| `HOST`          | URL to be used by the reverse proxy. E.g. `vault.domain.de`. | `false`         | `true`           | none          |

<!-- CONTRIBUTING -->

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git switch -c feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/Good-Games-Munich/vaultwarden.svg?style=flat-square
[contributors-url]: https://github.com/Good-Games-Munich/vaultwarden/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Good-Games-Munich/vaultwarden.svg?style=flat-square
[forks-url]: https://github.com/Good-Games-Munich/vaultwarden/network/members
[stars-shield]: https://img.shields.io/github/stars/Good-Games-Munich/vaultwarden.svg?style=flat-square
[stars-url]: https://github.com/Good-Games-Munich/vaultwarden/stargazers
[issues-shield]: https://img.shields.io/github/issues/Good-Games-Munich/vaultwarden.svg?style=flat-square
[issues-url]: https://github.com/Good-Games-Munich/vaultwarden/issues
