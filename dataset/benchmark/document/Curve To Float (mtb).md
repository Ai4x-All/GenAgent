- `Curve To Float (mtb)`: This node specializes in transforming a FLOAT_CURVE into a FLOAT or FLOATS. It abstractly focuses on the conversion process, leveraging the curve's structure to produce either a singular value or a sequence of values, tailored to the interpolation requirements.
    - Inputs:
        - `curve` (Required): Represents a curve defined by a series of points, each with X and Y coordinates, serving as the primary data structure for generating FLOAT or FLOATS output through interpolation. Type should be `FLOAT_CURVE`.
        - `steps` (Required): Specifies the number of intervals for interpolating Y values along the curve, affecting the granularity of the FLOATS output or the precision of the FLOAT output. Type should be `INT`.
    - Outputs:
        - `floats`: A list of interpolated FLOAT values derived from the input FLOAT_CURVE, based on the specified number of steps. Type should be `FLOATS`.
        - `float`: A single interpolated FLOAT value from the input FLOAT_CURVE, suitable for scenarios requiring a singular value. Type should be `FLOAT`.
