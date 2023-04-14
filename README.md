# Cognite API and MQTT Integration

This Jupyter Notebook demonstrates how to use the Cognite Python SDK to interact with Cognite Data Fusion (CDF) and send data to an MQTT broker.

## Overview

This notebook covers the following topics:

1. Importing the necessary libraries and initializing the Cognite client.
2. Listing and retrieving assets from CDF.
3. Listing, retrieving, and searching for time series in CDF.
4. Retrieving time series data points.
5. Creating a new time series in CDF.
6. Writing data points to a time series.
7. Deleting a time series.
8. Data manipulation with pandas and numpy:
   - Retrieve data points for a specific time series.
   - Convert data points to a pandas DataFrame.
   - Manipulate data using pandas and numpy.
   - Create a new time series to store manipulated data.
   - Write the manipulated data back to the new time series.
9. Egress 1-minute downsampled aggregate data to MQTT:
   - Retrieve 1-minute downsampled aggregate data for all time series.
   - Egress the data to an MQTT broker every minute.
10. Egress 1-minute downsampled aggregate data to MQTT, organized by asset hierarchy:
    - Retrieve 1-minute downsampled aggregate data for all time series.
    - Organize the data into MQTT topics based on the asset hierarchy.
    - Egress the data to the MQTT broker every minute.

## Usage

1. Replace the placeholders like `your-api-key`, `your-project`, `your-mqtt-broker`, and `your-mqtt-topic` with the appropriate values for your use case.
2. Make sure the necessary libraries (`cognite-sdk`, `pandas`, `numpy`, and `paho-mqtt`) are installed.
3. Run the code cells in the Jupyter Notebook, making sure to follow the instructions in the Markdown cells.

## Requirements

- Python 3.7+
- Cognite Python SDK
- pandas
- numpy
- paho-mqtt
