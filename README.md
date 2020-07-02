# MongoDB Atlas Java Sample Project

This repository contains an example application that connects
to a MongoDB instance using the Java MongoDB Driver. You can
use this example application as a starting point for a Java
application that connects to MongoDB Atlas.

## Prerequisites

1) To build and run this project, you will need IntelliJ IDEA Community
Edition for MacOS, Windows, or Linux. You can download it 
[here](https://www.jetbrains.com/idea/).

2) A working installation of the [Java 8 JDK](https://developers.redhat.com/products/openjdk/download).

3) A working installation of the [Maven](https://maven.apache.org/) build system. (Your IntelliJ installation should include this)

It is also helpful, but not necessary, to have a working installation of
[Git](https://git-scm.com/downloads) version control.

Some of these tools may come pre-installed in your programming environment.

## Getting Started

The following instructions explain how to get this project
connected to your instance of MongoDB Atlas.

### 1. Download the Repository

To get started with this sample project, download this repository to your
programming environment. You can either download this project using Git
version control:

```bash
git clone git@github.com:mongodb-university/atlas_starter_java.git
```

Or you can download a ZIP archive using your browser
[from GitHub](https://github.com/mongodb-university/atlas_starter_dotnet/archive/master.zip).
If you download this project as a ZIP archive,
[unzip the archive](https://www.wikihow.com/Unzip-a-File) before proceeding.

### 2. Open the Project

1. In IntelliJ, select `File > Open... `

2. Navigate to the directory containing this project.

3. Select the directory `atlas_starter_java`.

4. Click `OK`.

### 3. Configure Maven

1. In IntelliJ, click to expand the `atlas_starter_java` directory.

2. Right click on the directory named `src`.

3. Select `Mark Directory as` from the context menu.

4. Select `Sources Root`.

### 4. Configure your Atlas Credentials

1. Expand `atlas_starter_java > src > main > java > mongodb > Main`.

2. Double-click `Main`.

3. On the following lines in `Main`, replace the Atlas connection URI with your own from the Atlas UI.

```java
    // TODO:
    // Replace the placeholder connection string below with your
    // Altas cluster specifics. Be sure it includes
    // a valid username and password! Note that in a production environment,
    // you do not want to store your password in plain-text here.
    String mongoUri = "<Your Atlas Connection String>";
```

4. Replace the `<password>` section of the Atlas connection URI you just pasted into `Main` with your password!

### 5. Run the Project

1. Right click `Main`.

2. Select `Run 'Main.main()'` from the context menu.

Congratulations! You have just connected to MongoDB Atlas using the Java MongoDB Driver!
Try modifying the code to experiment with the Driver and MongoDB!

## Troubleshooting

Are you having trouble getting connected to your MongoDB Atlas instance? Double-check the following:

1. Have you replaced the `mongoUri` variable with a valid connection string provided by the Atlas UI?

2. Have you [whitelisted your current IP address](https://docs.atlas.mongodb.com/security-whitelist/) in the Atlas UI?

3. Do you have a [working installation of Java](https://stackoverflow.com/questions/18888220/how-to-check-whether-java-is-installed-on-the-computer)?
