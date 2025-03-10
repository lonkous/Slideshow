# Slide 1 Intro 

Script:
"Good [morning/afternoon], everyone. Thank you for taking the time to be here today. My name is Elias Kupeczki, and I am thrilled to present my project: 'Development of a Customer App for Retail Companies with Odoo as the Backend.'.

In today's presentation, I will take you through the documentation and the development journey of the app. The key points we will cover include an overview (Überblick), the project timeline (Zeitplan), the project methodology (Projektmethode), the implementation process (Umsetzung), the final results (Resultat), and a reflection on the lessons learned (Reflexion).
 

# SLIDE 2 overview

First, let's take a look at the current situation (IST Situation).

Currently, the retail company is using Odoo as their ERP system. While Odoo offers all their  required features for  example inventory, sales, and customer management, there is no native mobile app for customer-facing interactions. This leaves customers with limited access to product information, as it is only currently available in store. 

the customers cannot engage with the business via a mobile platform, which means the company is missing an opportunity to provide a more convenient and accessible experience for their users.

The goal is to develop a mobile customer app using Ionic and Angular, which will directly integrate with Odoo for real-time data syncing. The app will enable customers to view all the  newest products and their information on their mobile devices.

In addition, the app will allow customers to manage their account details, including their address, phone number, and password. To enhance the in-store experience, the app will also feature a QR code that can be scanned at the checkout for easy identification.

One key feature is the offline functionality, which will allow customers to access their QR code and track their loyalty points even when there’s no internet connection. However it is important to  note that the offline mode is only read only.


# Slide 3 Projektmethode

Kanban is a flexible and visual project management approach that helps teams manage their workflow and ensure efficient delivery. It is especially effective in agile environments, where continuous improvement and adaptability are key to project success. The main principle of Kanban is to visualize the work process, track progress, and ensure that tasks flow smoothly from one stage to the next.

For my project, I have structured my Kanban board into several key stages:

  Backlog: This is the collection of all features, tasks, and ideas for the app that are yet to be worked on. It’s essentially the what will be done, where we store everything that might be needed throughout the project.

  To-Do: These are the tasks that we have planned for the next iteration(my case a day). At this stage, the tasks have been prioritized, and we are ready to start working on them in the upcoming cycle.

  In Progress: This column represents tasks that are actively being worked on. Team members move tasks here as they start working on them, providing a clear picture of what’s currently being done. WIP is very import here as only one thing will ever be in progress at a time.

  Testing: Once a task has been implemented, it moves into the Testing phase. This is where we ensure that the feature works as expected, with rigorous quality assurance and bug testing to make sure everything functions perfectly.

  Done: Finally, once a task passes testing and meets the quality standards, it moves to the Done column. This indicates that the task is completed, and no further work is required on it.

Relevance for the Project

Kanban is highly relevant to our project because it allows us to manage the development of the customer app in an organized and transparent way. By breaking the work into manageable tasks and visually tracking progress, we can easily see the status of each feature or bug fix. This method also supports flexibility, allowing us to adjust priorities and shift tasks as needed, especially when new requirements or challenges arise during development.

Even though there were moments during the project where I fell behind on certain tasks or encountered delays, Kanban helped me get back on track. The visual representation of the workflow made it clear where I stood in terms of progress. When I noticed tasks piling up in the “To-Do” or “In Progress” columns, I could quickly assess which areas needed my immediate attention. Kanban allowed me to re-prioritize and focus on the tasks that would help me catch up in the most efficient way, ensuring that I could maintain the overall momentum of the project.

Moreover, Kanban helps us ensure that nothing falls through the cracks and that we maintain a steady flow of work, reducing bottlenecks and optimizing productivity across the team.


# Slide Tools

For the development of my customer app, I used a range of tools to streamline the process, manage dependencies, and ensure efficient testing and deployment. Each tool played a specific role in enabling a smooth workflow and ensuring the app's functionality across different platforms.

Node.js & NPM: Node.js provided the JavaScript runtime environment necessary for running development scripts, while NPM (Node Package Manager) was essential for managing dependencies, including Angular CLI, Ionic CLI, and additional libraries like the QR generator.
Ionic Framework & CLI: Ionic allowed me to develop a cross-platform mobile application with a single codebase. It provided UI components that adapted to both Android and iOS, and its CLI simplified project management, component generation, and debugging.
Angular Framework: As the core framework for the app, Angular provided a structured component-based architecture, enabling scalability and maintainability through features like services and guards.
Firefox & Selenium: Firefox was my primary browser for testing, and Selenium helped automate UI testing by simulating user interactions across different scenarios.
Testing Devices: I conducted mobile testing on a Samsung Galaxy S9 and a Google Pixel 7 Pro to evaluate the app’s performance across different hardware capabilities.
Java 21: Java was required to install and manage the app on Android devices. While iOS deployment required additional Apple-specific tools and a developer license, I primarily focused on the Android platform during development.

# Slide MVC

The Model-View-Controller (MVC) architecture is a widely used design pattern that helps organize code in a structured and maintainable way. It separates concerns into three main parts:

  Model: This represents the data in the application. In my app, the model consists of services that handle data related to products, orders, and users. These services interact with the database but are only accessed through the controller.
  View: The view is the user interface of the app. It consists of HTML and CSS, along with modern UI components provided by Ionic, to ensure an intuitive and responsive experience for users.
  Controller: The controller acts as the logic layer of the app. It is responsible for handling user interactions, processing API requests, and ensuring the correct data is displayed. In my app, this is managed through TypeScript files in each component, which call the services to load or modify data.