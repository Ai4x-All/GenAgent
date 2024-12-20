- `ADE_SigmaScheduleWeightedAverageInterp`: This node is designed to create a new sigma schedule by interpolating between two given sigma schedules based on a specified weight range and interpolation method. It effectively blends the characteristics of both input schedules into a single, new schedule, allowing for dynamic adjustments in the diffusion process.
    - Inputs:
        - `schedule_A` (Required): The first sigma schedule to be interpolated. Type should be `SIGMA_SCHEDULE`.
        - `schedule_B` (Required): The second sigma schedule to be interpolated. Type should be `SIGMA_SCHEDULE`.
        - `weight_A_Start` (Required): The starting weight for the first sigma schedule in the interpolation. Type should be `FLOAT`.
        - `weight_A_End` (Required): The ending weight for the first sigma schedule in the interpolation. Type should be `FLOAT`.
        - `interpolation` (Required): The method of interpolation to be used for blending the sigma schedules. Type should be `COMBO[STRING]`.
    - Outputs:
        - `sigma_schedule`: The resulting sigma schedule after interpolation. Type should be `SIGMA_SCHEDULE`.
