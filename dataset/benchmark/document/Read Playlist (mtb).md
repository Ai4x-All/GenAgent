- `Read Playlist (mtb)`: The Read Playlist node is designed to facilitate the reading of playlists from a specified path, allowing for the retrieval of playlist contents based on the provided name and index. It supports conditional execution and persistence options to enhance flexibility in playlist management.
    - Inputs:
        - `enable` (Required): Determines whether the reading of the playlist is enabled or not, acting as a conditional execution flag. Type should be `BOOLEAN`.
        - `persistant_playlist` (Required): Indicates whether the playlist should be read from a persistent storage location, affecting the path from which the playlist is loaded. Type should be `BOOLEAN`.
        - `playlist_name` (Required): The name of the playlist to read, which can include formatting for dynamic naming based on the index. Type should be `STRING`.
        - `index` (Required): An integer used to format the playlist name dynamically, allowing for indexed playlist management. Type should be `INT`.
    - Outputs:
        - `playlist`: The contents of the read playlist, returned as a list of playlist items. Type should be `PLAYLIST`.
