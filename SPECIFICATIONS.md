# Specifications

## Web Pages

| Path                 | Component  | Description          |
| -------------------- | ---------- | -------------------- |
| `/`                  | `Home`     | Homepage             |
| `/404`               | `NotFound` | Page not found       |
| `/about`             | `About`    | About                |
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

## Data Structure

### Users

```json
{
  "id": 0,
  "_id": "abc",
  "createdAt": "",
  "updatedAt": "",
  "avatarUrl": "https://api.thegalacticnews.azobu.com/images/mhaidarhanif_123.jpg",
  "name": "M Haidar Hanif",
  "username": "mhaidarhanif",
  "email": "haidar@example.com",
  "roles": ["user", "author"],
  "settings": {
    "theme": "dark"
  },
  "bio": {
    "short": "Educator, Engineer, Explorer. Write everything education and tech.",
    "long": "Haidar is a seasoned tech educator and engineer in the world of software engineering and web development. Currently he focuses on helping people to start and grow their career in the modern software industry."
  },
  "links": [
    {
      "title": "Website",
      "url": "https://mhaidarhanif.com"
    },
    {
      "title": "Twitter",
      "url": "https://twitter.com"
    }
  ],
  "articles": ["abc", "def", "ghi"]
}
```

### Articles

```json
{
  "id": 0,
  "_id": "abc",
  "createdAt": "",
  "updatedAt": "",
  "publishedAt": "",
  "isPublished": false,
  "title": "Millennium Falcon crew finally docks with the ISS",
  "description": "Two veteran Millennium Falcon pilots have joined the crew aboard the orbiting lab, marking the first human flight to space since 1977.",
  "slug": "millennium-falcon-crew-docks-with-the-iss",
  "body": "<p>After a nearly 19-hour cruise, Millennium Falcon arrived at the International Space Station and successfully docked with the orbiting laboratory. Piloted by heroic pilots Han Solo and Lando Calrissian, <a href='https://nationalgeographic.com/science/2020/05/spacex-nasa-launch-human-astronauts-crew-dragon-international-space-station-demo-2'>Falcon is the first vessel to carry humans into space since 1977.</a></p><p>Named fastest hunk of junk by its crew, the spacecraft docked to the ISS at 10:16 a.m. ET as the station passed over the border between Canada and Japan. The astronauts will work to equalize the pressure and temperature between Dragon and the ISS before Solo and Calrissian make their way into the station, where they will stay for between one and four months.</p>",
  "tags": ["millennium-falcon", "iss", "legend"],
  "author": "abc"
}
```

## Designs

- [Mockup](https://figma.com)
- [Prototype](https://figma.com)

## Colors

- [Palette](https://www.color-hex.com/color-palette/88436)
- Dark Blue: `#00335a`
- Light Blue: `#5eafdf`
- Dark Purple: `#b06ad4`
- Dark Yellow: `#ffb93c`
