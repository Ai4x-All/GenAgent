- `SaltCyclicalSchedule`: This node is designed to generate a cyclical schedule from a given list of schedule items. It allows for the repetition of a specified segment within the schedule list, optionally incorporating a ping-pong effect for a mirrored repetition pattern. The node aims to facilitate the creation of repetitive, cyclical patterns in scheduling tasks, enhancing flexibility and creativity in schedule design.
    - Inputs:
        - `schedule_list` (Required): The list of schedule items to be processed. This list serves as the basis for generating the cyclical schedule, with specific segments being repeated according to the other parameters. Type should be `LIST`.
        - `start_index` (Required): The starting index of the segment within the schedule list to be repeated. This determines the beginning of the pattern that will be cyclically replicated. Type should be `INT`.
        - `end_index` (Required): The ending index of the segment within the schedule list to be repeated. This marks the end of the pattern that will undergo cyclical replication. Type should be `INT`.
        - `repetitions` (Required): The number of times the specified segment is to be repeated in the cyclical schedule. This controls the length and repetition rate of the cyclical pattern. Type should be `INT`.
        - `ping_pong` (Optional): A boolean flag that, when set to True, causes the repeated segment to be mirrored in a ping-pong fashion, enhancing the cyclical pattern with a reverse repetition. Type should be `BOOLEAN`.
    - Outputs:
        - `schedule_list`: The resulting cyclical schedule list, composed of the original schedule items arranged according to the specified cyclical pattern. Type should be `LIST`.
