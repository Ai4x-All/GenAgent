- `ImpactSetWidgetValue`: This node is designed to set the value of a widget within a node in a workflow, based on various types of input values such as boolean, integer, float, or string. It dynamically adjusts the widget's value and type according to the provided input, facilitating flexible and interactive adjustments within the workflow.
    - Inputs:
        - `signal` (Required): A signal input that triggers the execution of the node, ensuring the node operates within the workflow's execution flow. Type should be `*`.
        - `node_id` (Required): The unique identifier of the node whose widget value is to be set, enabling targeted updates within the workflow. Type should be `INT`.
        - `widget_name` (Required): The name of the widget within the node to be updated, specifying which widget's value is to be changed. Type should be `STRING`.
        - `boolean_value` (Optional): An optional boolean value to set for the widget, allowing for true/false adjustments. Type should be `BOOLEAN`.
        - `int_value` (Optional): An optional integer value to set for the widget, enabling numerical adjustments. Type should be `INT`.
        - `float_value` (Optional): An optional float value to set for the widget, allowing for decimal adjustments. Type should be `FLOAT`.
        - `string_value` (Optional): An optional string value to set for the widget, enabling text adjustments. Type should be `STRING`.
    - Outputs:
        - `signal_opt`: Returns the input signal, indicating the completion of the widget value update. Type should be `*`.