# License Scanning by Scancode tool

---

## What is Licence Scanning ?

Open source license scanning refers to the process of analyzing software dependencies within a project to identify and manage the licenses associated with each component. The goal is to ensure that the project complies with the terms and conditions set forth by the licenses of its constituent parts. This practice is essential for both legal compliance and maintaining a healthy and sustainable open source ecosystem.


## Benefits of Open Source License Scanning:
Legal Compliance: Mitigate legal risks by ensuring that your project complies with the terms and conditions of the open source licenses associated with its dependencies. This helps avoid potential lawsuits and legal challenges.
Risk Mitigation: Identify and mitigate potential security and compliance risks associated with using open source components. Proactively addressing these issues protects the project from vulnerabilities and ensures a more robust and secure software ecosystem.
Efficient Resource Management: Understand the licensing landscape of your project to make informed decisions about resource allocation. This includes selecting components that align with your project's licensing policies and avoiding unnecessary complications.
Community Engagement: Foster positive relationships with the open source community by respecting and complying with the licenses of the software you use. This encourages collaboration, transparency, and mutual respect within the broader developer community.
Enhanced Reputation: Demonstrate a commitment to ethical and legal software development practices, enhancing your project's reputation among users, contributors, and potential collaborators.


---

## Tools for License Scanning


 ### Open Source Tools:

 - **janitor.git** – Code Janitor is an open-source tool that helps evaluate source code for compliance with open source licenses. From The Linux Foundation, Code Janitor can be used with other products to check code. To know more click [git.linuxfoundation.org](http://git.linuxfoundation.org/janitor.git/)

 - **LicenseFinder** – An open-source tool that detects the licenses of the code being used in your projects, compares those licenses against a user-defined whitelist and then provides an actionable report.To know more click  [github.com/pivotal/LicenseFinder](https://github.com/pivotal/LicenseFinder)

 - **scancode-toolkit** – From nexB, the open source ScanCode suite of utilities scans code for licenses, copyright, and dependencies to find, discover and inventory open source and third-party components used in your code.To know more click [github.com/nexB/scancode-toolkit](https://github.com/nexB/scancode-toolkit) or [scancode-toolkit.readthedocs.io](https://scancode-toolkit.readthedocs.io/en/latest/index.html)

 -  **Licensee** - An open-source tool for identifying licenses within projects. It focuses on detecting license files and metadata and is available as a Ruby gem.To know more click [github.com/licensee](https://github.com/licensee/licensee)


---

## Comparison

| Tool                | Key Features                                           | Integration/Usage       | Primary Purpose                       |
|---------------------|--------------------------------------------------------|-------------------------|---------------------------------------|
| **janitor.git**     | - License compliance checks                           | - Linux Foundation tools | - Evaluate source code compliance     |
|                     | - Open source license evaluation                      | - Other products         | - Integration with other products     |
| **LicenseFinder**   | - License detection                                   | - Standalone             | - Detect licenses in project code     |
|                     | - Whitelist comparison                                | - User-defined whitelist | - Compare against whitelist           |
|                     | - Actionable reporting                                |                         | - Provide actionable license reports  |
| **scancode-toolkit**| - License scanning                                    | - Comprehensive utility  | - Scan code for licenses, copyrights, |
|                     | - Copyright discovery                                 | - Detailed inventory     |   and dependencies                    |
|                     | - Dependency analysis                                 | - nexB tools             | - Inventory open source components    |
| **Licensee**        | - License file detection                              | - Ruby gem               | - Identify project licenses           |
|                     | - Metadata analysis                                   | - GitHub integration     | - Analyze license files and metadata  |


---


## Imp Difference


# Comparison between License Finder and ScanCode

## License Finder

### Purpose and Scope
- Designed to help developers manage and comply with open source licenses in their projects.
- Primarily focused on identifying licenses for project dependencies.

### Functionality
- Scans project dependencies to identify their licenses.
- Helps ensure that all dependencies are compliant with the desired licensing policy.

### Key Features
- Automatic detection of licenses for project dependencies.
- Supports multiple package managers like npm, Bundler, Maven, and more.
- Generates reports on detected licenses.
- Allows customization of license approval policies.
- Command-line interface (CLI) for easy integration into CI/CD pipelines.

### Strengths
- Simplifies the process of managing licenses for project dependencies.
- Easy integration with common development workflows.
- Focuses on ensuring compliance with licensing policies set by the user.

## ScanCode

### Purpose and Scope
- Focused on identifying licenses, copyrights, and package information in codebases.
- Provides detailed insights into licenses and copyrights within the entire codebase, not just dependencies.

### Functionality
- Scans directories, files, and code snippets to detect licenses.
- Provides comprehensive information about license types and terms.

### Key Features
- Extensive and regularly updated license detection database.
- Detailed attribution and origin information.
- Can detect not only licenses but also copyrights and package metadata.
- Open-source tool with a high level of customization.
- Detailed and comprehensive reports.

### Strengths
- Provides deep and granular insights into all aspects of licenses and copyrights in the codebase.
- Suitable for thorough audits and compliance checks.
- Open-source, allowing for transparency and community contributions.

## Key Differences

### Scope and Focus
- **License Finder**: Primarily focuses on managing licenses for project dependencies and ensuring they comply with licensing policies.
- **ScanCode**: Offers a comprehensive scan of the entire codebase, providing detailed license, copyright, and package information.

### Detail and Depth
- **License Finder**: Provides a straightforward way to manage and report on licenses for dependencies.
- **ScanCode**: Delivers in-depth and detailed information suitable for thorough compliance audits.

### Integration
- **License Finder**: Designed to integrate easily with CI/CD pipelines and development workflows, especially with its CLI.
- **ScanCode**: While it can also integrate into workflows, its use is more suited for detailed analysis and audits rather than routine dependency management.

### Customization and Open Source
- **License Finder**: Provides some customization in terms of license policies but is more focused on practical application within development workflows.
- **ScanCode**: Highly customizable due to its open-source nature, allowing for extensive modifications and use in various scenarios.

### Conclusion
**License Finder** is ideal for developers looking to manage and ensure compliance of project dependencies with minimal setup, focusing on practical and routine compliance management. **ScanCode**, on the other hand, is suited for those needing detailed and comprehensive analysis of licenses and copyrights across their entire codebase, making it a robust tool for thorough audits and compliance checks.

---

## Why we use scancode instead of other tool

### Why Use ScanCode:

1. **Comprehensive Scanning**:
   - **Detailed Checks**: ScanCode looks for licenses, copyrights, and dependencies in your code.

2. **Wide License Detection**:
   - **Many Licenses**: It can find many different types of licenses, even uncommon ones.
   - **Custom Rules**: You can add your own rules to detect special licenses.

3. **Open Source**:
   - **Transparency**: The code is open for anyone to see and modify.
   - **Community Support**: Many people contribute to improving ScanCode.

4. **Detailed Reports**:
   - **In-depth Reports**: Creates detailed reports about the code.
   - **Multiple Formats**: Reports can be in different formats like JSON, HTML, and CSV.

5. **Dependency Analysis**:
   - **Third-Party Components**: Finds all third-party parts of the code.
   - **Security Checks**: Helps to find security issues in these parts.

6. **Regular Updates**:
   - **Active Maintenance**: ScanCode is regularly updated with new features.
   - **Quick Adaptation**: Quickly adapts to new and changing licenses.

7. **Integration and Extensibility**:
   - **Easy Integration**: Works well with CI/CD pipelines and other tools.
   - **Modular Design**: Easy to add new features to ScanCode.

---


## Main Purpose of ScanCode:

The main purpose of ScanCode is to help developers and companies:

- Understand and manage open-source licenses in their code.
- Identify copyrights and dependencies.
- Ensure legal compliance with open-source software.
- Avoid potential issues with using third-party software.

ScanCode scans the codebase to find all components and provides detailed reports on the licenses used and any possible legal implications.

---
## Advantages of ScanCode:

1. **Comprehensive Analysis**:
   - Thoroughly scans code for licenses, copyrights, and dependencies.


2. **Open Source**:
   - The code is available for anyone to view, modify, and improve.
   - Benefits from community support and contributions.

3. **Detailed Reports**:
   - Generates in-depth reports on the codebase.
   - Reports can be exported in multiple formats like JSON, HTML, and CSV.

4. **Security and Compliance**:
   - Helps ensure compliance with open-source licenses.
   - Assists in identifying potential security vulnerabilities in dependencies.

5. **Regular Updates**:
   - Actively maintained with frequent updates and improvements.
   - Quickly adapts to new licenses and changes in existing ones.



## POC [ Proof of Concept ]

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

![image](https://github.com/MyGurukulam-P8/public_repo/assets/166389004/fadf84f4-ae58-4310-b733-a9088910e21f)


- **Verify Library Path:** Check if the libgomp.so.1 file exists in your system's library path. You can use the find command to search for it:

      find / -name "libgomp.so.1" 2>/dev/null

  ![image](https://github.com/MyGurukulam-P8/public_repo/assets/166389004/c339f003-dccf-46a8-840c-8f151fabf9ee)


- **Update LD_LIBRARY_PATH:** If the library exists in a different directory, you can update the LD_LIBRARY_PATH environment variable to include the directory containing libgomp.so.1:

      export LD_LIBRARY_PATH=/path/to/libgomp/directory:$LD_LIBRARY_PATH

![image](https://github.com/MyGurukulam-P8/public_repo/assets/166389004/35fd3e84-f1b5-44d9-87db-fd8d46a487b1)

### Tool Installation on Linux

1. Create a Python virtual environment:

    On Debian/Ubuntu systems, you need to install the python3-venv package using the following command before creating a Python virtual environment.

        apt install python3.10-venv

![image](https://github.com/MyGurukulam-P8/public_repo/assets/166389004/3e423545-9f79-4f56-bdaa-baaff75d6f64)


  then run below command to create venv

       /usr/bin/python3 -m venv venv

   For more information on Python virtualenv, visit this [page](https://docs.python-guide.org/dev/virtualenvs/#lower-level-virtualenv).


2. Activate the virtual environment you just created:

       source venv/bin/activate

3. Run pip to install the latest versions of base utilities:
 
        pip install --upgrade pip setuptools wheel
![image](https://github.com/MyGurukulam-P8/public_repo/assets/166389004/f161c46e-fb8e-476b-8252-96e52c0fec20)



4. Install the latest version of ScanCode:

       pip install scancode-toolkit


![image](https://github.com/MyGurukulam-P8/public_repo/assets/166389004/ce44051c-b8a3-47a2-ae15-5b507912214e)


## How to Run a Scan

### Deciding Scan Options

These are some common scan options you should consider using before you start the actual scan, according to your requirements.

1. The basic scan options, i.e. ```-c``` or ```--copyright```, ```-l``` or ```--license```, ```-p``` or ```--package```, ```-e``` or ```--email```, ```-u``` or ```--url```, and ```-i``` or ```--info``` cane be selected according to the requirements. 

2. ```--license-score INTEGER``` is to be set if license matching accuracy is desired (Default is 0, and increasing this means a more accurate match). 

3. ```-n INTEGER``` option can be used to speed up the scan using multiple parallel processes.

4. ```--timeout FLOAT``` option can be used to skip files taking a long time to scan.

5. ```--ignore <pattern>``` can be used to skip certain group of files.

6. ```<OUTPUT FORMAT OPTION(s)>``` is also a very important decision when you want to use the output for specific tasks/have requirements. Here we are using ```json``` as ScanCode Workbench imports ```json``` files only.


----

## Running The Scan

Clone the code:

    git clone https://github.com/OT-MICROSERVICES/salary-api.git



Now, run the scan with the options decided:

     scancode -clpeui -n 2 --ignore "*.java" --json-pp sample.json salary-api

A Progress report is shown:

![image](https://github.com/MyGurukulam-P8/public_repo/assets/166389004/18e0c343-89ff-4225-b7a8-2153d585414f)








