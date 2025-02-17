# PCB RawProject
The **PCB RawProject** repository provides a **ready-to-use template** for your PCB designs in **Altium Designer**. It includes pre-configured settings that will help you **kickstart your designs** without the hassle of setting everything up from scratch.   
The project is designed to serve as a **foundation** for creating and customizing your own PCB projects, ensuring consistency and ease of use.   
This project is ideal for anyone looking to **save time** in the early stages of PCB design while maintaining high-quality standards in their projects. Whether you're a beginner or an experienced designer, using this template can streamline your workflow and help you focus more on the design aspects.

> [!CAUTION]
> It is absolutely critical that you carefully read every single word of this document, line by line, to ensure you don't miss any details. Nothing can be overlooked.

## **Minimum PCB Design Requirements**
| **Requirement**                           | **Value**  |
|-------------------------------------------|------------|
| Minimum Drilling Hole Diameter            | 0.4mm      |
| Minimum Drilling Hole Diameter (HalfPad)  | 0.7mm      |
| Minimum Clearance                         | 0.2mm      |
| Minimum Trace Width                       | 0.2mm      |
| Minimum Overlay Resolution                | 0.15mm     |
| Minimum Annular Ring                      | 0.15mm     |
| Minimum Copper to Board Edge Distance     | 0.2mm      |
| Minimum Hole-to-Hole Distance             | 0.3mm      |
| Minimum CNC-Route Gap for Internal Cuts   | 0.6mm      |

> [!TIP]
> The **design rules** in this project are suitable for most **local PCB manufacturing** companies. However, it is recommended to consult and place your PCB orders through the **Telegram group** below for affordable and reliable PCB printing services:  
[CheapProject Telegram Group](https://t.me/CheapProject)

## **Connection Matrix Configuration**
In this project, the "Connection Matrix" settings in Altium Designer have been configured in such a way that no pin can remain unconnected. This ensures that all pins and ports are appropriately linked to their corresponding components or circuits, eliminating the possibility of unconnected pins in the PCB design.

![MatrixConnection](Images/ConnectionMatrix.png)


### Connection Verification

Through this configuration, Altium automatically verifies and ensures that every pin is connected to the appropriate component or system in the design. If a pin is left unconnected, it will be flagged, and the designer will be alerted. This eliminates potential errors caused by missing connections and ensures a more robust and functional design.

### Error Reporting

Color coding is used to show the status of each connection:

- **Red**: Fatal Error — A critical issue with the connection.
- **Orange**: Warning — A potential problem that needs attention.
- **Green**: No Report — No issues detected.
- **Yellow**: Error — A minor issue or misconfiguration detected.

This configuration helps in ensuring that the design adheres to best practices and prevents any unconnected pins from being overlooked during the design process.

## **Net Scope Configuration**
According to the settings configured in the **Options** section, all **Power Ports** and **Net Labels** are treated as **local** in this design. This configuration is important, especially in a **hierarchical design**, where multiple schematic sheets are involved.

![NetScope](Images/NetScope.png)

In hierarchical designs, multiple sheets represent different sections or modules of the circuit. The **local** setting for Power Ports and Net Labels means that their scope is limited to the sheet or module in which they are defined. This ensures that:

- **Power Ports** will be confined to their respective sheets and will not interfere with or be incorrectly referenced by other sheets. Each sheet can have its own local power ports, which simplifies the design and prevents cross-sheet confusion.
- **Net Labels** will similarly be treated locally within each sheet. This prevents issues where nets are incorrectly connected across different sheets due to misidentified or globally scoped labels.

By setting Power Ports and Net Labels as local, the design follows a strict hierarchical structure, where connections between sheets are well-defined and easy to manage, avoiding unintended cross-connections or misinterpretations of net names across different sheets.

This approach helps maintain a clean and organized design, especially in large or complex PCB projects that involve multiple schematic sheets and hierarchical levels.

# Resources
- [Altium Library](https://github.com/aKaReZa75/Altium-Library)  
  ---  
   All PCB designs across all repositories and projects are built using this Altium Designer component library. It contains a wide range of verified footprints, schematic symbols, and 3D models, ensuring consistency and accuracy in PCB designs. If you're working on a new PCB, using this library will save you time and minimize errors.

- [PCB & Electronics Design Training](https://github.com/aKaReZa75/PCB)  
  ---  
  This repository is dedicated to **learning PCB design and electronics from scratch**. It covers everything from circuit theory to practical PCB layout techniques, including routing strategies, best practices, and component placement. Whether you're a beginner or an experienced designer, this resource will help you **improve your PCB design skills and create professional-quality boards**.

# 💻 How to Use Git and GitHub
To access the repository files and save them on your computer, there are two methods available:
1. **Using Git Bash and Cloning the Repository**
   - This method is more suitable for advanced users and those familiar with command-line tools.
   - By using this method, you can easily receive updates for the repository.

2. **Downloading the Repository as a ZIP file**
   - This method is simpler and suitable for users who are not comfortable with command-line tools.
   - Note that with this method, you will not automatically receive updates for the repository and will need to manually download any new updates.

## Clone using the URL.
First, open **Git Bash** :
-  Open the folder in **File Explorer** where you want the library to be stored.
-  **Right-click** inside the folder and select the option **"Open Git Bash here"** to open **Git Bash** in that directory.

![open Git Bash](Images/Step0.png)

> [!NOTE] 
> If you do not see the "Open Git Bash here" option, it means that Git is not installed on your system.  
> You can download and install Git from [this link](https://git-scm.com/downloads).  
> For a tutorial on how to install and use Git, check out [this video](https://youtu.be/BsykgHpmUt8).
  
-  Once **Git Bash** is open, run the following command to clone the repository:

 ```bash
git clone https://github.com/aKaReZa75/PCB_RawProject.git
```
- You can copy the above command by either:
- Clicking on the **Copy** button on the right of the command.
- Or select the command text manually and press **Ctrl + C** to copy.
- To paste the command into your **Git Bash** terminal, use **Shift + Insert**.

![Clone the Repository](Images/Step1.png)

- Then, press Enter to start the cloning operation and wait for the success message to appear.

![Open the Library File](Images/Step2.png)

> [!IMPORTANT]
> Please keep in mind that the numbers displayed in the image might vary when you perform the same actions.  
> This is because repositories are continuously being updated and expanded. Nevertheless, the overall process remains unchanged.

> [!NOTE]
> Advantage of Cloning the Repository:  
> - **Receiving Updates:** By cloning the repository, you can easily and automatically receive new updates.  
> - **Version Control:** Using Git allows you to track changes and revert to previous versions.  
> - **Team Collaboration:** If you are working on a project with a team, you can easily sync changes from team members and collaborate more efficiently.  

## Download Zip
If you prefer not to use Git Bash or the command line, you can download the repository directly from GitHub as a ZIP file.  
Follow these steps:  
1. Navigate to the GitHub repository page and Locate the Code button:
   - On the main page of the repository, you will see a green Code button near the top right corner.

2. Download the repository:
   - Click the Code button to open a dropdown menu.
   - Select Download ZIP from the menu.

  ![Download Zip](Images/Step7.png)  

3. Save the ZIP file:
   - Choose a location on your computer to save the ZIP file and click Save.

4. Extract the ZIP file:
   - Navigate to the folder where you saved the ZIP file.
   - Right-click on the ZIP file and select Extract All... (Windows) or use your preferred extraction tool.
   - Choose a destination folder and extract the contents.

5. Access the repository:
   - Once extracted, you can access the repository files in the destination folder.

> [!IMPORTANT]
> - No Updates: Keep in mind that downloading the repository as a ZIP file does not allow you to receive updates.    
>   If the repository is updated, you will need to download it again manually.  
> - Ease of Use: This method is simpler and suitable for users who are not comfortable with Git or command-line tools.

# 📝 How to Ask Questions
If you have any questions or issues, you can raise them through the **"Issues"** section of this repository. Here's how you can do it:  

1. Navigate to the **"Issues"** tab at the top of the repository page.  

  ![Issues](Images/Step3.png)

2. Click on the **"New Issue"** button.  
   
  ![New Issue](Images/Step4.png)

3. In the **Title** field, write a short summary of your issue or question.  

4. In the "Description" field, detail your question or issue as thoroughly as possible. You can use text formatting, attach files, and assign the issue to someone if needed. You can also use text formatting (like bullet points or code snippets) for better readability.  

5. Optionally, you can add **labels**, **type**, **projects**, or **milestones** to your issue for better categorization.  

6. Click on the **"Submit new issue"** button to post your question or issue.
   
  ![Submeet New Issue](Images/Step5.png)

I will review and respond to your issue as soon as possible. Your participation helps improve the repository for everyone!  

> [!TIP]
> - Before creating a new issue, please check the **"Closed"** section to see if your question has already been answered.  
>   ![Closed section](Images/Step6.png)  
> - Write your question clearly and respectfully to ensure a faster and better response.  
> - While the examples provided above are in English, feel free to ask your questions in **Persian (فارسی)** as well.  
> - There is no difference in how they will be handled!  

> [!NOTE]
> Pages and interfaces may change over time, but the steps to create an issue generally remain the same.

# 🤝 Contributing to the Repository
To contribute to this repository, please follow these steps:
1. **Fork the Repository**  
2. **Clone the Forked Repository**  
3. **Create a New Branch**  
4. **Make Your Changes**  
5. **Commit Your Changes**  
6. **Push Your Changes to Your Forked Repository**  
7. **Submit a Pull Request (PR)**  

> [!NOTE]
> Please ensure your pull request includes a clear description of the changes you’ve made.
> Once submitted, I will review your contribution and provide feedback if necessary.

# 🌟 Support Me
If you found this repository useful:
- Subscribe to my [YouTube Channel](https://www.youtube.com/@aKaReZa75).
- Share this repository with others.
- Give this repository and my other repositories a star.
- Follow my [GitHub account](https://github.com/aKaReZa75).

# 📜 License
This project is licensed under the GPL-3.0 License. This license grants you the freedom to use, modify, and distribute the project as long as you:
- Credit the original authors: Give proper attribution to the original creators.
- Disclose source code: If you distribute a modified version, you must make the source code available under the same GPL license.
- Maintain the same license: When you distribute derivative works, they must be licensed under the GPL-3.0 too.
- Feel free to use it in your projects, but make sure to comply with the terms of this license.
  
# ✉️ Contact Me
Feel free to reach out to me through any of the following platforms:
- 📧 [Email: aKaReZa75@gmail.com](mailto:aKaReZa75@gmail.com)
- 🎥 [YouTube: @aKaReZa75](https://www.youtube.com/@aKaReZa75)
- 💼 [LinkedIn: @akareza75](https://www.linkedin.com/in/akareza75)
