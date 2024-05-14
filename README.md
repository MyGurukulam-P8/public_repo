|Sr. No.| Table of contents|
|:---:|-------------------|
| 1.| [Introduction](#Introduction) 
| 2.| [What is Licence Scanning?](#What-is-Licence-Scanning?)
| 3.| [Why Licence Scanning is required?](#Why-Licence-Scanning-is-required?)
| 4.| [Tools for License Scanning](#Tools-for-License-Scanning)
| 5.| [Comparison about different Tools](#Comparison-about-different-Tools)
| 6.| [Advantages of License Scanning & its tools](#Advantages-of-License-Scanning-&-its-tools)
| 7.| [POC of License Scanning as a CI checks](#POC-of-License-Scanning-as-a-CI-checks)
| 8.| [Best Practices for License Scanning](#Best-Practices-for-License-Scanning)
| 9.| [Conclusion](#Conclusion)
| 10.| [Contact Information](#Contact-Information)
| 11.| [References](#References)


## Introduction

In the world of software development, it's super important to follow the rules when it comes to using other people's code. This means paying attention to the licenses that come with the code you use. One way to make sure you're following the rules is by scanning for licenses in your code as part of your regular checks.

In this guide, we'll cover the basics of license scanning in CI, look at some tools that can help, compare them, and see why this practice is so important for smooth software development

## What is Licence Scanning in CI checks?

License scanning in CI checks refers to the process of automatically analyzing the licenses of third-party dependencies used in a software project as part of the Continuous Integration (CI) pipeline. This involves scanning the source code and dependencies to detect any open-source licenses or proprietary licenses associated with the software components. The purpose is to ensure compliance with licensing requirements and identify any potential licensing conflicts or issues early in the development process. By integrating license scanning into CI checks, developers can mitigate legal risks, maintain license compliance, and streamline the management of software licenses.

## Why Licence Scanning is required as a CI checks?

| **Aspect**                  | **Explanation**                                                                                   |
|:-----------------------------:|---------------------------------------------------------------------------------------------------|
| **Legal Compliance**        | Ensures that the application code follows the rules of licenses attached to third-party components.|
| **Risk Mitigation**         | Identifies and addresses potential licensing issues early to avoid legal disputes and delays.     |
| **Dependency Management**   | Helps keep track of third-party dependencies and ensures they align with the project's licenses.  |
| **Transparency & Accountability** | Provides a clear view of the project's licensing status, promoting responsibility and awareness.|
| **Security Considerations** | Enhances application security by identifying vulnerabilities and prioritizing security updates.  |

## Tools for License Scanning

  ### Commercial Tools:

 - **Black Duck Hub** – The commercial Hub service scans code to identify all embedded open source components, and then automatically searches for known vulnerabilities for remediation. It can send alerts when new vulnerabilities are found in your code.To know more click [blackducksoftware.com](https://www.blackducksoftware.com/products/hub)

 - **FlexNet Code Insight** – Flexera, which acquired licensing compliance vendor Palamida in 2016, commercially offers Flex Code Insight to help automate corporate open source use among developers, legal teams and security staffers. [flexerasoftware.com](https://www.flexerasoftware.com/enterprise/products/software-vulnerability-management/flexnet-code-insight/)

 - **FOSSA** – This is a commercial tool that automatically performs code dependency tracking, license compliance scanning in the background.To know more click [fossa.io](http://fossa.io/)

  ### Open Source Tools:

 - **janitor.git** – Code Janitor is an open-source tool that helps evaluate source code for compliance with open source licenses. From The Linux Foundation, Code Janitor can be used with other products to check code. To know more click [git.linuxfoundation.org](http://git.linuxfoundation.org/janitor.git/)

 - **LicenseFinder** – An open-source tool that detects the licenses of the code being used in your projects, compares those licenses against a user-defined whitelist and then provides an actionable report.To know more click  [github.com/pivotal/LicenseFinder](https://github.com/pivotal/LicenseFinder)

 - **scancode-toolkit** – From nexB, the open source ScanCode suite of utilities scans code for licenses, copyright, and dependencies to find, discover and inventory open source and third-party components used in your code.To know more click [github.com/nexB/scancode-toolkit](https://github.com/nexB/scancode-toolkit) or [scancode-toolkit.readthedocs.io](https://scancode-toolkit.readthedocs.io/en/latest/index.html)

 -  **Licensee** - An open-source tool for identifying licenses within projects. It focuses on detecting license files and metadata and is available as a Ruby gem.To know more click [github.com/licensee](https://github.com/licensee/licensee)

## Comparison about different Open source Tools used

| **Tool Name**          | **Features**                                                                                                          | **Supported Languages**                         | **Ease of Use**                   | **Community Support**        | **Performance**                                      | **Integration with CI/CD**                           |
|:------------------------:|-----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|----------------------------------|-------------------------------|------------------------------------------------------|------------------------------------------------------|
| **Code Janitor**       | - Automated license scanning and compliance management.     |Java, JavaScript, Python      | Easy to configure and use.      | Moderate     | Good, but may lack advanced features.   | Integration available, but may require customization. |
| **Scancode-toolkit**   | - Comprehensive scanning capabilities with detailed reporting.    | Multiple, including Java, JavaScript, Python    | Powerful but may require setup. | Strong | Excellent, with detailed reports and customization.   | Integration available with popular CI/CD platforms.    |
| **Licensee**           | - Focus on identifying license files and metadata within projects. | Ruby, JavaScript, Python  | Simple and straightforward.  | Moderate   | Limited to identifying license files and metadata.    | Limited integration options with CI/CD pipelines. |
| **License Finder**     | - Helps identify licenses for dependencies used in projects.  | Ruby, JavaScript, Python, Java   | Easy to integrate and use.       | Moderate | Good, with reliable license identification.  | Integration available with popular CI/CD platforms. |


## Advantages of License Scanning

| **Aspect**                   | **Explanation**                                                                                         |
|:------------------------------:|---------------------------------------------------------------------------------------------------------|
| **Legal Compliance**         | Mitigate legal risks by ensuring that your project complies with the terms and conditions of the open source licenses associated with its dependencies. This helps avoid potential lawsuits and legal challenges. |
| **Risk Mitigation**          | Identify and mitigate potential security and compliance risks associated with using open source components. Proactively addressing these issues protects the project from vulnerabilities and ensures a more robust and secure software ecosystem. |
| **Efficient Resource Management** | Understand the licensing landscape of your project to make informed decisions about resource allocation. This includes selecting components that align with your project's licensing policies and avoiding unnecessary complications. |
| **Community Engagement**     | Foster positive relationships with the open source community by respecting and complying with the licenses of the software you use. This encourages collaboration, transparency, and mutual respect within the broader developer community. |
| **Enhanced Reputation**      | Demonstrate a commitment to ethical and legal software development practices, enhancing your project's reputation among users, contributors, and potential collaborators. |


## POC of Scan Code - Toolkit for License Scanning on sample source code

To view complete setup and POC steps refer to doc [Scancode_POC.md](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/blob/main/Application%20CI%20Design/Generic%20CI%20operation/Licence%20Scanning/Scancode_POC.md)

## Best Practices for License Scanning

| **Aspect**                            | **Description**                                                                                            |
|:--------------------------------------:|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Automated Scanning Tools**         | Utilize automated scanning tools to streamline the process of identifying and managing open source licenses. These tools can efficiently analyze dependencies, provide detailed reports, and flag potential licensing issues. |
| **Regular Audits**                   | Conduct regular audits of your project's dependencies to ensure compliance with the latest licensing requirements. This helps prevent issues arising from new or updated licenses in the evolving software landscape. |
| **Clear Documentation**              | Maintain clear and comprehensive documentation regarding the licenses of all open source components used in your project. This documentation should be easily accessible to developers, legal teams, and other stakeholders. |
| **Integration with Development Workflow** | Integrate license scanning into your development workflow to ensure that license compliance is considered from the early stages of development. This prevents potential issues from escalating as the project progresses. |
| **Educate Development Teams**        | Educate development teams about the importance of open source license compliance. Provide training on interpreting license information and making informed decisions when selecting and using open source components. |
| **Define License Policies**          | Establish clear policies regarding acceptable license types for your project. Define criteria for evaluating license compatibility to avoid conflicts and ensure a consistent approach to license management. |


## Conclusion

Among these four tools compared, Scancode-toolkit stands out for its comprehensive scanning capabilities and detailed reporting features. It supports multiple languages and provides powerful scanning functionality. While it may require some setup initially, its strong community support and extensive documentation make it a reliable choice for license scanning in source code.

In summary, Scancode-toolkit is recommended for its robust features, versatility, and strong community backing, making it a valuable asset for ensuring license compliance in software projects.




------

# POC

## Introduction

A typical software project often reuses hundreds of third-party packages. License and packages, dependencies and origin information is not always easy to find and not normalized: ScanCode discovers and normalizes this data for you.

Read more about ScanCode here: https://scancode-toolkit.readthedocs.io/.

Check out the Scancode toolkit source code at https://github.com/nexB/scancode-toolkit

## Prerequisites

- ScanCode requires a Python version between 3.8 to 3.12.
  
## System Requirements

- **Hardware :** ScanCode will run best with a modern X86 64 bits processor and at least 8GB of RAM and 2GB of disk space. These are minimum requirements.

- **Supported operating systems:** ScanCode should run on these 64-bit OSes running X86_64 processors:

     1. **Linux:** on recent 64-bit Linux distributions,

     2. **Mac:** on recent x86 64-bit macOS (10.15 and up, including 11 and 12).

     3. **Windows:** on Windows 10 and up,


## Scancode Installation steps

### Install Python

ScanCode app archives come with packaged with all required dependencies except for Python that has to be downloaded and installed separately. 

For support on installing python version 3.11 visit at [python setup link](https://vegastack.com/tutorials/how-to-install-python-3-11-on-ubuntu-22-04/)

### Install shared library file "libgomp.so.1"

- First, ensure that the **libgomp.so.1** library is installed on your system. You can typically install it using your system's package manager. For example, on Ubuntu, you can run:

      sudo apt-get install libgomp1

    ![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/e0badc06-7614-4e1b-916e-ec4c13ad8d2c)
 
- **Verify Library Path:** Check if the libgomp.so.1 file exists in your system's library path. You can use the find command to search for it:

      find / -name "libgomp.so.1" 2>/dev/null

  ![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/23f97eba-e05d-49b0-a7de-7d46dedde2f3)

- **Update LD_LIBRARY_PATH:** If the library exists in a different directory, you can update the LD_LIBRARY_PATH environment variable to include the directory containing libgomp.so.1:

      export LD_LIBRARY_PATH=/path/to/libgomp/directory:$LD_LIBRARY_PATH

   ![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/31b767e1-7dc9-4e40-b415-272d39f09856)

### Tool Installation on Linux

1. Create a Python virtual environment:

    On Debian/Ubuntu systems, you need to install the python3-venv package using the following command before creating a Python virtual environment.

        apt install python3.10-venv

  ![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/ad70cd0c-720b-4ffe-8fa7-229042ea785b)


  then run below command to create venv

       /usr/bin/python3 -m venv venv

   For more information on Python virtualenv, visit this [page](https://docs.python-guide.org/dev/virtualenvs/#lower-level-virtualenv).

2. Activate the virtual environment you just created:

       source venv/bin/activate

3. Run pip to install the latest versions of base utilities:
 
        pip install --upgrade pip setuptools wheel

   ![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/41006d0a-ff87-4867-a957-7b761e8ad965)


5. Install the latest version of ScanCode:

       pip install scancode-toolkit

![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/d28b1507-b29a-4b45-892d-6c882d387487)

Now Scancode is successfully installed and ready to scan any source code!!

## How to Run a Scan

### Deciding Scan Options

These are some common scan options you should consider using before you start the actual scan, according to your requirements.

1. The basic scan options, i.e. ```-c``` or ```--copyright```, ```-l``` or ```--license```, ```-p``` or ```--package```, ```-e``` or ```--email```, ```-u``` or ```--url```, and ```-i``` or ```--info``` cane be selected according to the requirements. 

2. ```--license-score INTEGER``` is to be set if license matching accuracy is desired (Default is 0, and increasing this means a more accurate match). 

3. ```-n INTEGER``` option can be used to speed up the scan using multiple parallel processes.

4. ```--timeout FLOAT``` option can be used to skip files taking a long time to scan.

5. ```--ignore <pattern>``` can be used to skip certain group of files.

6. ```<OUTPUT FORMAT OPTION(s)>``` is also a very important decision when you want to use the output for specific tasks/have requirements. Here we are using ```json``` as ScanCode Workbench imports ```json``` files only.

## Running The Scan

Clone the code:

    git clone https://github.com/OT-MICROSERVICES/salary-api.git

![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/abeb12f0-077d-48f1-9b2e-0921af2f8778)

Now, run the scan with the options decided:

     scancode -clpeui -n 2 --ignore "*.java" --json-pp sample.json salary-api

A Progress report is shown:

![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/d024f381-25f5-464c-8261-010fd8bc8878)


## Code Scan output 

The output stored in sample.json contains the scan results in json format as shown in below image:

![image](https://github.com/OT-MyGurukulam/Snaatak_p8_Documentation/assets/164150159/c5e7fdd8-6486-4383-b00d-619fb0a24b39)

