### Section A — Server Log Analysis

**Q1.** What is the username of the primary suspect? What evidence from the server log supports this?
jdoe92. ip address is entirely different, the timestamp is way past work hours, and the data taken was all valuable information.

**Q2.** At what time did the suspect's activity become suspicious? What specifically changed between their daytime and nighttime sessions? (Look at IP addresses AND files accessed.)
The ip went from 192.168.1.102 to 10.45.88.201. the user then had activity 11 hours after normal work time. 

**Q3.** List every file the suspect downloaded during the suspicious session. Why would each of these files be considered sensitive or confidential?
ALL_CLIENT_DATA.zip, FINANCIAL_MASTER.xlsx, SSN_DATABASE.csv
they have all of the cliental data, the master record for the company's finnincial choices, and a data base.

**Q4.** One of the entries in the server log shows a POST request to `/admin/export.php`. What does a POST request mean, and why is this action more concerning than a GET request in this context?
Post means send, alter, or create data on a web server.
its more dangerous because it changes the data rather then just retrieving it. 

---

### Section B — Email Header Analysis

**Q5.** What is the originating IP address of the email? How does this connect to the server log?

**Q6.** Why is the use of ProtonMail significant in this investigation? What does it suggest about the suspect's intent?

**Q7.** The email subject line is blank. Why might a suspect deliberately send an email with no subject? What technique might they be using?

**Q8.** Compare the email timestamp to the server log. What does the timeline suggest about the order of events on the night of April 18?

---

### Section C — File Metadata Analysis

**Q9.** The three large data files (`.zip`, `.xlsx`, `.csv`) all have the same "Created" date and time range. What does this tell you about how they got onto the USB drive?

**Q10.** The "Last Accessed" timestamp on every file is `2026-04-19 08:15:01`. Why are they all identical? What event caused this?

**Q11.** `note_to_self.txt` was created at `23:44:00` and the email was sent at `23:32:00`. Does this timeline make sense given what the note contains? Explain.

---

### Section D — Putting It All Together

**Q12.** Write a 1–2 paragraph **incident summary** describing what you believe happened on the night of April 18, 2026. Use specific evidence (timestamps, filenames, IP addresses) to support your conclusion. This is similar to what a real digital forensics analyst would write in an official report.

**Q13.** What laws or regulations might the suspect have violated? Name at least TWO (examples: CFAA — Computer Fraud and Abuse Act, HIPAA, FERPA, state data breach laws).

**Q14.** If you were the IT security team, what THREE security measures could have prevented or detected this breach earlier?
