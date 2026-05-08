# Syntecxhub_PortScanner_PasswordManager
Syntexhub Week 1 Tasks
# Syntecxhub Internship Projects

## 👨‍💻 Intern: Sagar Ali

Syntecxhub Internship
Task 1 Report
Project: TCP Port Scanner (Python)
1. Objective
To build a TCP port scanner using Python that:
•	Scans a target host 
•	Checks open/closed ports 
•	Accepts port range input 
•	Handles errors and timeouts 
•	Displays results in terminal 
________________________________________
2. Tools Used
•	Python 3 
•	socket library 
•	Kali Linux / terminal 
•	nslookup (DNS resolution tool) 
________________________________________
3. Target Selection (DNS Lookup)
Command used:
nslookup scanme.nmap.org
Result:
•	Server: 192.168.100.1 
•	Domain resolved to IP: 45.33.32.156 
 
•	nslookup output showing domain → IP resolution 
________________________________________
4. Port Scanner Execution
Command used:
python3 port_scanner.py
Input given:
Target IP: 192.168.100.1
Start Port: 20
End Port: 100
 
________________________________________
5. Results
Scan Output:
•	Most ports: CLOSED 
•	Open ports detected: 
o	🔓 Port 53 (DNS) 
o	🔓 Port 80 (HTTP) 
output:
[CLOSED] 20-52
[OPEN] 53
[CLOSED] 54-79
[OPEN] 80
[CLOSED] 81-100
 
 
________________________________________
6. Observations
•	Port 53 is typically used for DNS services. 
•	Port 80 indicates HTTP web service. 
•	Most other ports were closed or filtered. 
•	Scanner successfully detected open services on target host. 
________________________________________
Source Code Port_Scanner.py:
 

Task 2 Report
Project: Secure Password Manager (CLI + Encryption)
1. Objective
To develop a secure command-line password manager using Python that:
•	Stores credentials securely using encryption (Fernet) 
•	Allows adding, viewing, and deleting entries 
•	Saves data in an encrypted file (vault.enc) 
•	Demonstrates basic cryptography + file handling 
________________________________________
2. Tools & Technologies Used
•	Python 3 
•	cryptography (Fernet encryption) 
•	JSON module 
•	File handling (OS module) 
•	Kali Linux terminal 
________________________________________
3. Working Process
 Program Execution
python3 password_manager.py
________________________________________
4. Features Demonstrated
🔹 Add Entry
•	Website: www.muet.edu.pk 
•	Username: sagar 
•	Password: kali 
 Data successfully encrypted and stored
________________________________________
🔹 View Entry
Displays decrypted stored credentials:
•	Site: www.muet.edu.pk 
•	Username: sagar 
•	Password: kali 
________________________________________
🔹 Delete Entry
Removes stored credentials securely:
•	Website deleted successfully 
________________________________________
🔹 Empty Vault Check
After deletion:
No data found
________________________________________
5. Execution Output Summary
✔ Add operation successful
✔ View operation shows decrypted data
✔ Delete operation removes data correctly
✔ Vault becomes empty after deletion
✔ Program exits safely
________________________________________
6. Screenshots 
<img width="1878" height="783" alt="image" src="https://github.com/user-attachments/assets/949a5c47-6133-4588-bca0-380d43e68f55" />


7. Security Concept Used
•	Uses Fernet symmetric encryption 
•	Data stored in encrypted file (vault.enc) 
•	Key stored separately (key.key) 
•	Prevents direct readable access to credentials 
________________________________________
8. Key Learning Outcomes
•	File encryption & decryption in Python 
•	CLI-based application development 
•	Secure data storage concepts 
•	Basic cryptographic implementation


