# Specifications

## Web Pages

| Path                 | Component  | Description          |
| -------------------- | ---------- | -------------------- |
| `/`                  | `Home`     | Homepage             |
| `/404`               | `NotFound` | Page not found       |
| `/register`          | `Register` | Register as new user |
| `/login`             | `Login`    | Login to user        |
| `/logout`            | `Logout`   | Logout from user     |
| `/users`             | `Users`    | List of all users    |
| `/users/:username`   | `User`     | User profile         |
| `/authors`           | `Authors`  | List of all authors  |
| `/authors/:username` | `Author`   | Author profile       |
| `/settings`          | `Settings` | Settings for user    |
| `/articles`          | `Articles` | List of all articles |
| `/:slug`             | `Article`  | Single article       |

## API Endpoints

| Endpoint          | Method | Description             | Query       | Headers         |
| ----------------- | ------ | ----------------------- | ----------- | --------------- |
| `/`               | `GET`  | Get index               | -           | -               |
| `/auth/register`  | `POST` | Register new user       | -           | -               |
| `/auth/login`     | `POST` | Login to user           | -           | -               |
| `/auth/logout`    | `GET`  | Logout from user        | -           | `Authorization` |
| `/auth/settings`  | `POST` | Get user settings       | -           | `Authorization` |
| `/users`          | `GET`  | Get all users           | `paginated` | -               |
| `/articles`       | `GET`  | Get all articles        | `paginated` | -               |
| `/articles/:slug` | `GET`  | Get one article by slug | -           | -               |

Inspirations:

- [The New York Times Developer Network](https://developer.nytimes.com)
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
