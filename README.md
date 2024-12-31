This is a Packet Sniffer Application based on Java, Networking and Swing UI
Designed for TCP, UDP and ICMP packet filtering, which can be extended to other protocols.

## Features:
1. Works perfectly in Windows OS (to be checked in MacOS)
2. Can be used to check detail of every packet
3. Option to store data in SQLite DB


## Tools used:
1. JDK (1.8)
2. Eclipse IDE
3. Wireshark
4. Jpcap
5. Winpcap

## Steps for Setting Up and Using Jpcap for Java Packet Sniffer Tool:

1. After installing Jpcap, locate the "Jpcap.dll" and "jpcap.jar" files on your system.
2. Open your system's environment variables settings. Add a new entry to the "PATH" or "CLASSPATH" variable, including the path to the directory containing the Jpcap files.
3. Find "Jpcap.dll" and copy it to either "[JRE directory]\bin" or "[JRE directory]\lib\ext\x86".
4. Copy "jpcap.jar" to "[JRE directory]\lib\ext". Also, copy "jpcap.jar" to "[JDK directory]\jre\lib\ext"
5. In the Java project, navigate to "Properties" and then "Libraries."
6. Click the "Add JAR/Folder" button and add the "jpcap.jar" file to the project's external libraries.
7. Jpcap requires elevated privileges (ROOT/Administrator) to access raw network data, as mentioned in the provided instructions.

## Components:
- Network Data:
  Network analysis is the core functionality of the packet sniffer. We capture network packets in each interface, parse packet headers for further analysis.
- Database (SQLite Database):
  An SQLite database is utilized to store captured network packet data, metadata, and analysis results. This database is used to save packet capture information for later analysis, historical tracking, and reporting. SQL queries are employed to retrieve specific data from the database, aiding in packet analysis.
- User Interface (Swing UI):
  A Swing-based graphical user interface (UI) is designed and built to provide users with an interactive and user-friendly interface for controlling and monitoring the packet sniffer tool.
  The UI can offer features like starting and stopping packet capture, displaying captured packet data, configuring capture filters, and presenting analysis results.
- Threads:
  Threads are employed to manage concurrency and ensure the efficient operation of the packet sniffer tool. Thread management helped in handling tasks concurrently for packet capture, processing, database storage and UI responsiveness without blocking or freezing.

![image](https://github.com/user-attachments/assets/33e2377c-e16e-4324-adcb-0344361cf8b0)


  
