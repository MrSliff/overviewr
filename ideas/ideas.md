# First thoughts and ideas

## Frontend -> HTML?
- *arrs in different tabs
- List missing Media
    - No API Method for missing movies?
        - Use open overseerr requests for now
    - Configurable
        - Age
        - Released/not released
    - Get (highest rated) download sources and list them
    - Fetch Metadata from Database
- Download Media
    - Call Backend API Methods
- Request missing media
    - If no download sources available, generate text fields for configured tracker and a submit button
    - Reverse Engineer POST Methods, Cookies, API or other missing stuff to do requests at tracker

## Backend -> Python
- Configuration
    - Radarr/Sonarr/Lidarr/Overseerr 
        - API Keys
        - IP:Port / FQDN
    - Configurable "Cronjobs" to fetch data from *arrs
- API Methods (look which are needed)
    - https://radarr.video/docs/api/
    - https://sonarr.tv/docs/api/
    - https://lidarr.audio/docs/api/
    - https://api-docs.overseerr.dev/
- Fetch missing Media
    - Overseerr
        - Can only fetch open requests from overseerr
        - Media before overseerr will be missing
    - Radarr/Sonarr
        - no API method to fetch missing movies?
            - Workaround: fetch all movies and filter by missing
                - bigger library = more resource intensive
- Store Data
    - SQlite or SQL Database 