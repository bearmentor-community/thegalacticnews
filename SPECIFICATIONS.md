# Specifications

## Pages

| Name     | Path              | Description          |
| -------- | ----------------- | -------------------- |
| Home     | `/`               | Homepage             |
| Articles | `/articles`       | List of all articles |
| Article: | `/articles/:slug` | One article page     |
| Users:   | `/users`          | List of all users    |
| Authors  | `/authors`        | List of all authors  |
| Register | `/register`       | Register as new user |
| Login    | `/login`          | Login to user        |
| Logout   | `/logout`         | Logout from user     |

## Endpoints

| Endpoint         | Method | Description       | Query       |
| ---------------- | ------ | ----------------- | ----------- |
| `/`              | `GET`  | Get index         | -           |
| `/articles`      | `GET`  | Get all articles  | `paginated` |
| `/users`         | `GET`  | Get all users     | `paginated` |
| `/auth/register` | `POST` | Register new user | -           |
| `/auth/login`    | `POST` | Login to user     | -           |
| `/auth/logout`   | `GET`  | Logout from user  | -           |

Inspirations:

- [News API](https://newsapi.org)

## Data

## Designs

- [Mockup](https://figma.com)
- [Prototype](https://figma.com)

## Colors

- [Palette](https://www.color-hex.com/color-palette/88436)
- Dark Blue: `#00335a`
- Light Blue: `#5eafdf`
- Dark Purple: `#b06ad4`
- Dark Yellow: `#ffb93c`
