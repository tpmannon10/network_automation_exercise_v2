# Python Coding Exercise for Network Automation Engineer

Problem Statement:

Your company is implementing a Zero-Touch Provisioning (ZTP) solution for network devices. The goal is to automate the process of downloading, parsing, and deploying configuration files to networking hardware (e.g., routers, switches, Wi-Fi access points). As a Network Automation Engineer, you are tasked with developing a Python application that simulates this process. Ensure that the application can run on any OS and without the need for any user to install dependencies by creating a custom Docker Image. Include a high-level network diagram that makes clear to the reader how the applicaiton fits within the network architecture.

Task Description:

Fetch Configuration Files from a Cloud Server: • Write a function that makes an API call to a simulated cloud server to fetch network configuration files. Assume the API returns JSON-formatted configuration data. • For this exercise, you can simulate the API response by reading a local JSON file that contains various network settings (DHCP, DNS, VLAN, etc.).

Parse the Configuration File: • Develop a function that parses the JSON data to extract various network settings, such as: • DHCP reservations • DNS settings • VLAN configurations • Firewall and ACL settings • IP assignments and routing

Organize Network Configurations: • Create a Python class NetworkConfig that holds the parsed configurations and provides methods to display or modify them. This class should handle different network settings logically and allow easy retrieval and modification.

Simulate Deployment to Network Devices: • Write a function deploy_configuration that takes the NetworkConfig object and simulates deploying these settings to different types of network devices (router, switch, access point). Since there is no access to actual devices, the function should output a log of deployment steps, indicating success or failure.

Error Handling and Validation: • Ensure proper error handling for scenarios such as API call failures, missing configuration sections, or incorrect data types. • Validate the configurations to ensure they meet certain criteria (e.g., valid IP address format, non-overlapping VLANs, etc.).

Application Delivery: • Create a customer Docker Image of the application, ensuring the application can best ran on any OS without the need for the user to install any dependency software/applications.

Documentation and Code Quality: • Provide clear documentation within the code, including docstrings for all functions and methods. • Ensure the code is modular, readable, and follows best practices (e.g., PEP 8). • Include a README file that contains a high level diagram showing the role the application plays within the network architecture and makes clear to the user where and how config files are sourced/accessed. The README should also contain any specific configuration/settings required by the user. 

Expected Output:

• Properly parsed and organized network configurations. • Simulated deployment logs that clearly state what configurations are being applied and where. • Error handling scenarios demonstrated (e.g., missing configuration data).

Evaluation Criteria:

• Correctness of the code. • Ability to parse and manage data efficiently. • Understanding of network settings and configurations. • Code quality, readability, and documentation. • Handling edge cases and error scenarios gracefully. • Ease of deployment.

Instructions:

• Provide your Python application as a single Docker Image file along with all supporting documentation. • A link to your Docker Image in Docker Hub will also be acceptible.
