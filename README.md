# Project Description

This project looks at the PM 2.5 and particle distribution data collected from a sensor during the folllowing experiments
- Cooking stir fry meals (3 trials)
- Using a 3D printer (3 trials)

  ** Disclaimer this is more of a informal experiment so the results and data gathering do not follow the strictest protocols, bear this in mind when interpreting the results


## Data 

The data collected for this project is stored in the data folder and is separated by the type of ezperiment. There is also a section for ambient data that was taken when I was gone from my apartment 

## Equipment Used

- Raspberry Pi 4
- PMSA003I
  - Air Quality
  - PM 2.5 +- 10 ug/m^3
- HTU21D-F 
  - Temperature/Humidity

## Running this yourself

If you have the necessary equipment to run this you must:
- Have a raspeberry pi with Blinka !(guide here)[https://learn.adafruit.com/circuitpython-on-raspberrypi-linux/installing-circuitpython-on-raspberry-pi]
- clone the sensor_code folder from this repository
- Change into the new directory you downloaded
- Create a virtual environment
  ```bash
  python -m venv venv
  ```
  - Activate it
  ```bash
  source env/bin/activate
  ```
  - Install the requiremente
  ```bash
  pip install -r requirements.txt
  ```

  - Then run the code
    ```bash
    python sensor_test.py
    ```

    ** Note this file the data is sent to is hardcoded so you will need to edit the file_name variable in the file to change this
  

