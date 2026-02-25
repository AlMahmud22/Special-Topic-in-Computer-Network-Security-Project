Power Plant Earthquake Emergency Shutdown System
Overview

This project simulates an earthquake emergency shutdown system for a power plant using two Raspberry Pi boards and a MongoDB cloud database. The system demonstrates the integration of hardware, software, and cloud services to create a real-time emergency response mechanism.

How It Works

A Control Board (Raspberry Pi + push button) updates an alarm state in a MongoDB cloud database.

An Emergency Board (Raspberry Pi + red and green LEDs) continuously monitors the alarm state.

If the alarm is "true", the red LED turns ON (emergency).

If the alarm is "false", the green LED turns ON (safe state).

Communication between boards happens through HTTP-based REST API calls to the MongoDB cloud database.

Technologies Used

Raspberry Pi 3

Python (RPi.GPIO, pymongo)

MongoDB Atlas (Free-tier cloud database)

Breadboard circuits (LEDs, push button, resistors)

Key Features

Real-time alarm state synchronization

Cloud-based database connectivity

Hardware-software integration

Button debouncing and error handling

Scalable deployment (works from different locations with internet access)

System Requirements

Two Raspberry Pi boards

Internet connection (port 443 open for HTTPS)

MongoDB Atlas cluster

Python with required libraries installed

Limitations

Requires stable internet connection

Dependent on cloud database availability

Possible latency if deployed far from the selected database region

Authors

Group 2

Sadik Al Mahmud

Munaimin Bin Monjour

Course: Special Topic in Computer Networks and Security
Session: 2024/2025-2
