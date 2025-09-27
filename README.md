# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
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
<img width="1920" height="1080" alt="Screenshot 2025-09-27 113050" src="https://github.com/user-attachments/assets/26a574d4-f78e-4710-8831-0c3e4e7a8d2f" />
<img width="575" height="420" alt="Screenshot 2025-09-26 140020" src="https://github.com/user-attachments/assets/18402863-61a5-4627-a329-c2733cb0f72b" />

<img width="1920" height="1080" alt="Screenshot 2025-09-26 140708" src="https://github.com/user-attachments/assets/f550d52a-ea1e-496c-a962-0846748b6dc3" />
<img width="1920" height="1080" alt="Screenshot 2025-09-26 140724" src="https://github.com/user-attachments/assets/bc590270-11ec-4d68-b63e-1c5a9eafe06a" />
<img width="1920" height="1080" alt="Screenshot 2025-09-27 112904" src="https://github.com/user-attachments/assets/a8abd6f6-b194-4760-8777-619b6df4bfd1" />
<img width="1920" height="1080" alt="Screenshot 2025-09-26 142724" src="https://github.com/user-attachments/assets/e05042bf-741a-4aed-bd49-f3582c6acda9" />

<img width="1920" height="1080" alt="Screenshot 2025-09-26 195518" src="https://github.com/user-attachments/assets/164ba86a-3ae7-44a5-88b0-bf68599c42b3" />

<img width="1920" height="1080" alt="Screenshot 2025-09-26 195528" src="https://github.com/user-attachments/assets/54df890b-749c-4c2c-8833-6c5ddfbeac24" />
<img width="1920" height="1080" alt="Screenshot 2025-09-26 195609" src="https://github.com/user-attachments/assets/d740f446-850b-47bd-8528-1eb3e4a48150" />
<img width="1920" height="1080" alt="Screenshot 2025-09-27 112838" src="https://github.com/user-attachments/assets/ba0d7144-b247-4ead-8aec-43c87f244607" />
<img width="1920" height="1080" alt="Screenshot 2025-09-27 112954" src="https://github.com/user-attachments/assets/30c294b5-6fac-4ea6-9fb6-c04e5b823fd2" />
<img width="1920" height="1080" alt="Screenshot 2025-09-27 113004" src="https://github.com/user-attachments/assets/b87acabc-ecb3-460e-9581-b380186ae39d" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

