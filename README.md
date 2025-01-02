# Ethical Hacking: Capture the Flag and Penetration Testing

This repository showcases the comprehensive Capture the Flag (CTF) and penetration testing project conducted as part of the **Ethical Hacking (CMP6176)** module. The project involved exploiting a purposefully vulnerable virtual machine to identify weaknesses and proposing mitigation strategies for enhanced security.

---

## **Project Overview**
This project was designed to simulate a real-world penetration testing scenario, emphasizing the discovery, exploitation, and remediation of vulnerabilities within a target system. The tasks included:
1. **Reconnaissance**: Identifying exploitable services and vulnerabilities.
2. **Exploitation**: Gaining access and demonstrating the impact of the vulnerabilities.
3. **Documentation**: Creating a professional penetration testing report.

### **Key Objectives**
- Demonstrate technical expertise by conducting a structured penetration test.
- Identify security weaknesses and assess their impact on confidentiality, integrity, and availability.
- Recommend actionable mitigation strategies to address identified vulnerabilities.

---

## **Findings and Exploited Vulnerabilities**
### **Exploited Ports and Services**
- **Port 19 (Chargen)**:
  - Vulnerability: Misconfiguration and susceptibility to DDoS amplification.
  - Exploitation: Conducted an amplification attack using hping3.
- **Port 3000 (Grafana 8.2.6)**:
  - Vulnerability: Path traversal allowing unauthorized access to sensitive files.
  - Exploitation: Extracted critical information via crafted directory traversal commands.
- **Port 5041 (Werkzeug 3.0.3)**:
  - Vulnerability: Command injection due to improper input sanitization.
  - Exploitation: Executed arbitrary commands to access sensitive files.
- **Port 8081 (Apache Flink)**:
  - Vulnerability: JAR upload leading to remote code execution.
  - Exploitation: Used Metasploit to initiate a Meterpreter session for full system access.
- **Port 8082 (PHPMyAdmin 4.8.1)**:
  - Vulnerability: Local File Inclusion via URL manipulation.
  - Exploitation: Bypassed whitelist checks to access sensitive server files.

---

## **Technologies and Tools Used**
1. **Kali Linux**:
   - Conducted reconnaissance and exploited vulnerabilities.
2. **Nmap**:
   - Performed port scanning and service version detection.
3. **Metasploit**:
   - Leveraged for JAR file upload and remote code execution.
4. **Nikto**:
   - Identified web server vulnerabilities.
5. **Netcat**:
   - Verified service functionality and potential misconfigurations.
6. **hping3**:
   - Simulated DDoS attacks to demonstrate the impact of vulnerabilities.

---

## **Skills Acquired**
1. **Technical Proficiency**:
   - Conducted detailed reconnaissance and exploited vulnerabilities effectively.
2. **Critical Thinking**:
   - Assessed the impact of vulnerabilities and proposed appropriate mitigations.
3. **Professional Documentation**:
   - Produced a structured and detailed penetration testing report.
4. **Tool Proficiency**:
   - Mastered various tools like Metasploit, Nmap, and Nikto for security assessments.

---

## **Recommendations**
- **Update Software**: Ensure regular updates to address known vulnerabilities.
- **Input Validation**: Implement robust input sanitization to prevent injections.
- **Firewall Implementation**: Restrict access to sensitive ports and monitor traffic.
- **Network Segmentation**: Limit exposure of critical services to reduce attack surface.
- **Intrusion Detection**: Deploy systems like Snort to detect and respond to malicious activities.

---
