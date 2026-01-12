# Customer Task Management System 📋

A Salesforce-based task management application built with Lightning Web Components (LWC) and Apex to help teams organize and track customer-related tasks efficiently.

---

## About This Project

I created this project to learn Salesforce development and build a practical solution for managing customer tasks. The application uses modern Salesforce technologies including Lightning Web Components, Apex controllers, and Lightning Message Service for component communication.

## Features

### Task Management
- Create new customer tasks with priority levels and task types
- View tasks in an organized card layout
- Filter tasks by name, priority, type, and sorting options
- Navigate through tasks with pagination support
- Responsive design that works on desktop and mobile devices

### Technical Highlights
- **Lightning Web Components (LWC)** for building reusable UI components
- **Apex Controllers** with wrapper classes for efficient data handling
- **Lightning Message Service** for real-time component communication
- **Dynamic SOQL queries** that adapt based on user filters
- **100% test coverage** on all Apex classes

## Components

**taskHeader** - Displays current time with greeting and allows creating new tasks

**taskCard** - Shows individual task details with priority badges and status indicators

**filterTask** - Provides filtering options for tasks (name, priority, type, sorting)

**taskList** - Main component that displays filtered tasks in a card grid layout

**paginator** - Handles navigation between pages of tasks

## Technologies Used

- Salesforce Lightning Web Components (LWC)
- Apex (Controllers, Wrapper Classes, Test Classes)
- Lightning Message Service (LMS)
- Salesforce Lightning Design System (SLDS)
- SOQL (Dynamic Query Building)
- JavaScript, HTML, CSS

## What I Learned

Building this project helped me understand:
- Component-based architecture in Salesforce
- Communication between LWC components using Lightning Message Service
- Writing efficient Apex code with wrapper classes
- Dynamic SOQL query construction based on filters
- Responsive design principles using Salesforce design system
- Test-driven development with Apex test classes

## Setup Instructions

1. Clone this repository:
```bash
git clone https://github.com/YOUR-USERNAME/customer-task-manager.git
```

2. Authorize your Salesforce org:
```bash
sfdx auth:web:login -a yourOrgAlias
```

3. Deploy the code to your org:
```bash
sfdx force:source:deploy -p force-app/main/default
```

4. Assign the permission set (if applicable) and open the app from App Launcher

## Project Structure

```
force-app/
├── lwc/
│   ├── taskHeader/
│   ├── taskCard/
│   ├── filterTask/
│   ├── taskList/
│   └── paginator/
├── classes/
│   ├── TaskController.cls
│   ├── TaskControllerTest.cls
│   └── (wrapper classes)
└── objects/
    └── CustomerTask__c/
```

## Testing

All Apex classes have comprehensive test coverage:
- TaskController: 100% coverage
- Wrapper classes: 100% coverage

Run tests using:
```bash
sfdx force:apex:test:run -n TaskControllerTest -r human
```

## Future Enhancements

Some features I'm planning to add:
- Task assignment to specific users
- Due date reminders and notifications
- Task categories with color coding
- Export tasks to CSV
- Dashboard with task analytics

## Contact

Feel free to reach out if you have questions or suggestions about this project.

---

**Note**: This is a learning project I built to practice Salesforce development. It demonstrates real-world development patterns and best practices, though it's not intended for production use without further customization.

---

### Acknowledgments

Thanks to the Salesforce developer community and Trailhead for the learning resources that helped me build this project.