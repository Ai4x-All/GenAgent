- `True Random.org Number Generator`: This node interfaces with the RANDOM.ORG API to generate true random numbers based on atmospheric noise. It allows for the generation of integers within a specified range, ensuring randomness through external entropy sources.
    - Parameters:
        - `api_key`: The API key for accessing RANDOM.ORG's services. It's essential for authentication and utilizing the API to generate random numbers. Type should be `STRING`.
        - `minimum`: The lower bound of the range within which random numbers are generated. It defines the smallest possible value of the generated numbers. Type should be `FLOAT`.
        - `maximum`: The upper bound of the range within which random numbers are generated. It defines the largest possible value of the generated numbers. Type should be `FLOAT`.
        - `mode`: Determines the mode of number generation, offering flexibility in how randomness is applied. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `number`: The generated random number as an integer. Type should be `NUMBER`.
        - `float`: The generated random number as a float. Type should be `FLOAT`.
        - `int`: The generated random number, explicitly indicating it's an integer for clarity. Type should be `INT`.