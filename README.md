# SayalGUI
The Sayal Sanjesh Water Meter Administration GUI is a Python application developed using the PySide6 library and Qt Designer. It serves as a user-friendly interface specifically designed for administering water meters produced by Sayal Sanjesh.
The primary goal of this GUI is to streamline the process of managing water meters by providing a comprehensive set of features and functionalities. With its intuitive design and user-friendly interface, the application simplifies administrative tasks related to water meter management for Sayal Sanjesh.

 # Key Features:

* User Authentication: The GUI includes a secure login system to ensure that only authorized personnel can access and modify water meter data, ensuring data privacy and security.

* Meter Registration: The application allows users to register new water meters by entering relevant information such as meter serial number, installation date, location, and customer details. This data is securely stored in a database linked to Sayal Sanjesh's water meter production system.

* Meter Data Visualization: The GUI provides visual representations of water meter data, including consumption patterns, usage trends, and historical records. Administrators can easily analyze and monitor water usage patterns to identify any anomalies or issues.

* Customer Management: The application enables efficient management of customer information, including contact details, billing addresses, and payment history. Administrators can easily search, add, edit, and remove customer records as required, ensuring accurate and up-to-date information.

* Meter Maintenance and Repairs: The GUI allows administrators to schedule and track maintenance tasks, repairs, and replacements for water meters. It provides notifications and reminders for upcoming maintenance activities, ensuring timely actions to maintain the quality and efficiency of the water meters.

* Reporting and Analytics: The application generates comprehensive reports and analytics based on water meter data. These reports can include information on meter performance, water consumption trends, revenue analysis, and other relevant metrics. This data helps in making informed decisions and optimizing operations.

* Data Import and Export: The GUI supports importing and exporting data in various formats, such as CSV or Excel files. This feature enables seamless data exchange with other systems or third-party applications, improving interoperability and data integration.

* Customization and Localization: The GUI can be customized to align with Sayal Sanjesh's branding and specific requirements. Additionally, it supports localization, allowing the application to be translated into different languages, making it accessible to a wider range of users.

> **Warning**: this project was created using PySide6 and Python 3.9, using previous versions can cause compatibility problems.

 # Running
> Inside your preferred terminal run the commands below depending on your system, remembering before installing Python 3.9> and PySide6 "pip install PySide6".
> ## **Windows**:
```console
python main.py
```
> ## **MacOS and Linux**:
```console
python3 main.py
```
# Compiling
> ## **Windows**:
```console
python setup.py build
```

# Project Files And Folders
> **main.py**: application initialization file.

> **main.ui**: Qt Designer project.

> **resouces.qrc**: Qt Designer resoucers, add here your resources using Qt Designer. Use version 6 >

> **setup.py**: cx-Freeze setup to compile your application (configured for Windows).

> **themes/**: add here your themes (.qss).

> **modules/**: module for running PyDracula GUI.

> **modules/app_funtions.py**: add your application's functions here.
Up
> **modules/app_settings.py**: global variables to configure user interface.

> **modules/resources_rc.py**: "resource.qrc" file compiled for python using the command: ```pyside6-rcc resources.qrc -o resources_rc.py```.

> **modules/ui_functions.py**: add here only functions related to the user interface / GUI.

> **modules/ui_main.py**: file related to the user interface exported by Qt Designer. You can compile it manually using the command: ```pyside6-uic main.ui> ui_main.py ```.
After expoting in .py and change the line "import resources_rc" to "from. Resoucers_rc import *" to use as a module.

> **images/**: put all your images and icons here before converting to Python (resources_re.py) ```pyside6-rcc resources.qrc -o resources_rc.py```.
