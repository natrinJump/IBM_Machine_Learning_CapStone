# Streamlit App Setup Guide

This guide will walk you through setting up a Streamlit app locally using a sample app provided. Streamlit is a Python library that allows you to create interactive web applications for data science and machine learning projects.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- Your favorite IDE or text editor for Python development.
- Python 3.7 - 3.9
- PIP (Python package installer)

We recommend creating a virtual environment for building Streamlit apps. If you are not familiar with virtual environments, you can learn more about them [here](https://docs.python.org/3/tutorial/venv.html).

## Sample App Download

Download the sample app from the following link: [first_app.zip](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-ML321EN-SkillsNetwork/labs/module_5/first_app.zip)

## Installation and Testing

1. Unzip the downloaded `first_app.zip`.
2. Open your terminal and navigate to the unzipped `first_app` directory:

    ```bash
    cd path/to/first_app
    ```

3. Install the required Python libraries specified in the `requirements.txt` file:

    ```bash
    pip3 install -r requirements.txt
    ```

4. Run the first app with the following command:

    ```bash
    streamlit run app.py
    ```

5. If you are running the app on your local environment, open your web browser and enter the URL [http://localhost:8501](http://localhost:8501).

This will launch the Streamlit app, and you can explore its features locally.

Feel free to modify the app according to your needs, and happy Streamlit development!
