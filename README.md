# rfidpy

The `rfidpy` library is designed to facilitate the interface between Raspberry Pi 5 and RFID technology.

## Usage
Raspberry pi 5 interface with RFID (MFRC522) reader.

## Requirements

Make sure to install the following libraries before using `rfidpy`:

- [spidev](https://pypi.org/project/spidev/)
- [gpiod](https://pypi.org/project/gpiod/)
- [time](https://docs.python.org/3/library/time.html)
- [logging](https://docs.python.org/3/library/logging.html)

These libraries are mandatory for the proper functioning of `rfidpy`.

## Installation
To install rfidpy, you can use the following command:
```pip install rfidpy ```

## Sample Program

Here's a simple example of how to use the `rfidpy` library in a Python program:

```python
from rfidpy import SimpleMFRC522

reader = SimpleMFRC522()

while True:
    id, text = reader.read()
    print(id)
```
## Run program
```python3 test.py```
