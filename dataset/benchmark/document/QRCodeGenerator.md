- `QRCodeGenerator`: The QRCodeGenerator node is designed to generate QR codes based on specified text inputs, offering customization options such as size, version, error correction level, box size, and border size. It encapsulates the process of QR code creation, making it accessible for various applications that require embedding information within a QR code format.
    - Inputs:
        - `text` (Required): The 'text' parameter is the input string to be encoded into the QR code. It is crucial as it determines the content that the QR code will represent. Type should be `STRING`.
        - `size` (Required): Specifies the final size of the generated QR code image in pixels. It affects the visibility and scannability of the QR code. Type should be `INT`.
        - `qr_version` (Required): Determines the version of the QR code, which indirectly controls the size and the amount of data that can be encoded. Type should be `INT`.
        - `error_correction` (Required): Sets the error correction level of the QR code, affecting its resilience to damage and the amount of data that can be restored. Type should be `COMBO[STRING]`.
        - `box_size` (Required): Defines the size of each box (or pixel) in the QR code, influencing the overall size of the QR code. Type should be `INT`.
        - `border` (Required): Specifies the width of the border around the QR code. A larger border can improve scannability but increases the overall size of the QR code. Type should be `INT`.
    - Outputs:
        - `image`: The output is an image of the generated QR code, ready for use in various applications. Type should be `IMAGE`.
