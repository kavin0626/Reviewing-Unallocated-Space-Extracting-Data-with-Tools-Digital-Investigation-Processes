# EX:5-Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
```
NAME:KAVINRAJ.S
REG NO:212223100019
```
## REQUIREMENTS:
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report


<img width="1918" height="1067" alt="Screenshot 2025-09-20 134717" src="https://github.com/user-attachments/assets/e4cf419f-7538-4013-bf9e-1792ae0bc2de" />




<img width="958" height="1013" alt="Screenshot 2025-09-20 194257" src="https://github.com/user-attachments/assets/51efc752-a6ad-48e5-a62c-1f975468002c" />



<img width="944" height="965" alt="Screenshot 2025-09-20 194325" src="https://github.com/user-attachments/assets/9d0452ff-ef20-415a-8697-bd3c3603bf29" />

<img width="611" height="464" alt="Screenshot 2025-09-20 194339" src="https://github.com/user-attachments/assets/2fd1f605-a97d-45f8-bd18-357344d7fd80" />

<img width="549" height="490" alt="Screenshot 2025-09-20 194351" src="https://github.com/user-attachments/assets/2efb8c6f-3604-4093-ba23-696f76a45047" />

<img width="557" height="439" alt="Screenshot 2025-09-20 194417" src="https://github.com/user-attachments/assets/19ae64ad-bd42-4a56-b4f0-b139018d7edf" />

<img width="487" height="356" alt="Screenshot 2025-09-20 194431" src="https://github.com/user-attachments/assets/0845625b-a726-41a1-818e-ba4b4b855898" />

<img width="599" height="483" alt="Screenshot 2025-09-20 194451" src="https://github.com/user-attachments/assets/7a0c6a8b-2fa6-4793-8661-c014a05dda14" />



<img width="712" height="907" alt="Screenshot 2025-09-20 194842" src="https://github.com/user-attachments/assets/c7a47a50-4aff-4b22-914c-e39bc024f91a" />



## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

