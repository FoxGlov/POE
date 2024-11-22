# POE
Claims System
Here's the updated README file tailored for the MVC version of the Claims Management System (CMS):  

---

# Claims Management System (CMS)

The Claims Management System (CMS) is a web-based application built using ASP.NET MVC. It allows users to submit claims related to hours worked, upload supporting documents, and manage the status of claims (Approve/Reject). This README file outlines the features, setup instructions, and usage guidelines.

---

## Features

- **User Interface**: Intuitive and responsive web interface for submitting and managing claims.
- **File Upload**: Ability to upload supporting documents (PDF, DOCX, XLSX) with a size limit of 5 MB.
- **Claim Submission**: Automatically calculates the total amount to be claimed based on hours worked and hourly rate.
- **Claim Status Management**: Allows coordinators and managers to approve or reject claims with comments while maintaining a detailed claim history.
- **Data Persistence**: Claims and associated data are stored in a relational database using Entity Framework.
- **Upload Directory**: Automatically saves uploaded files to a predefined directory on the server.

---

## Prerequisites

- .NET Core 6.0 or later
- Visual Studio 2022 or later
- SQL Server (for database)

---

## Setup Instructions

1. **Clone the Repository**:  
   Clone the repository to your local machine:  
   ```bash
   git clone https://github.com/your-username/ClaimsManagementSystem.git
   cd ClaimsManagementSystem
   ```

2. **Open in Visual Studio**:  
   Open the solution file (`ClaimsManagementSystem.sln`) in Visual Studio.

3. **Configure the Database**:  
   - Update the connection string in the `appsettings.json` file to match your SQL Server setup.  
   - Run the following commands in the Package Manager Console to apply migrations and seed the database:  
     ```bash
     Update-Database
     ```

4. **Build the Solution**:  
   Build the solution to restore NuGet packages and compile the project.

5. **Run the Application**:  
   Start the application by pressing `F5` or using the Debug menu. The application will launch in your default web browser.

---

## Usage Instructions

### Submitting a Claim

1. Navigate to the **Submit Claim** page.  
2. Fill in the required fields:
   - Lecturer ID
   - Lecturer Name
   - Hours Worked
   - Hourly Rate
   - Work Date (select from the date picker)  
3. Upload a supporting document:
   - Click the **Upload Document** button and select a file.
   - Ensure it is a valid file type (PDF, DOCX, XLSX) and within the file size limit (5 MB).  
4. Click **Calculate Amount** to see the calculated total based on the hours worked and hourly rate.  
5. Click **Submit Claim** to submit the claim. A confirmation message will appear upon successful submission.

### Reviewing Claims

1. Navigate to the **Manage Claims** page (requires Coordinator/Manager login).  
2. Claims are listed with their details.  
3. To approve or reject a claim:  
   - Select a claim from the list.  
   - Provide comments (optional).  
   - Click **Approve** or **Reject**.  

4. View uploaded documents by clicking on their file names to open them using the default application.  

---

## Notes

- **Data Storage**: All claims and uploaded files are stored persistently in the database.  
- **Improvements**: Future enhancements may include:
  - Notification features to inform users of claim status changes.
  - Audit logs for better tracking of changes.

---

## Contributing

Contributions are welcome!  
- Submit issues and feature requests through the repository.  
- Open pull requests with detailed descriptions of the changes.

---

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

---

## Acknowledgments

Thanks to all contributors and libraries that made this project possible.  
This application was built using ASP.NET MVC and Microsoft's documentation.

---

## Contact

For questions or feedback, please contact **your-email@example.com**.

---

### How to Use This README

- Replace placeholders like `your-username` and `your-email@example.com`.  
- Adjust sections as necessary to reflect any project-specific changes.

