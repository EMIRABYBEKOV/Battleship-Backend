
# Battleship

This is the backend Django project for the Battleship game.

## Table of Contents

- [Description](#description)
- [Requirements](#requirements)
- [Installation](#installation)
- [Environment Setup](#environment-setup)
- [Database Setup](#database-setup)
- [Running the Server](#running-the-server)
- [Accessing the Application](#accessing-the-application)

## Description

This repository contains the backend implementation for the Battleship game using Django. It includes all the necessary configurations and instructions to set up and run the server locally.

## Requirements

- Python 3.x
- PostgreSQL

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/EMIRABYBEKOV/Battleship_.git
   cd Battleship_
   ```

2. Create a virtual environment and install the required packages:
   ```sh
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

## Environment Setup

1. Create a `.env` file:
   ```sh
   touch .env
   ```

2. Add your credentials to the `.env` file. Here is an example:
   ```
   DB_NAME=your_db_name
   DB_USER=your_db_user
   DB_PASSWORD=your_db_password
   DB_HOST=your_db_host
   DB_PORT=your_db_port
   ```

## Database Setup

1. Open PostgreSQL:
   ```sh
   psql
   ```

2. Create the database specified in your `.env` file:
   ```sql
   CREATE DATABASE your_db_name;
   ```

3. Run the following command to update your database:
   ```sh
   python3 manage.py migrate
   ```

## Running the Server

Run the following command to start the Django development server:
   ```sh
   python3 manage.py runserver
   ```

## Accessing the Application

The application can be accessed at [http://localhost:8000/](http://localhost:8000/).
