# IDBac Database Submission and Analysis  

## <ins>IDBac Templates<ins>
[MALDI Plate Map](https://docs.google.com/spreadsheets/d/1ihFy6lQyJtWy9fp46ahMPWk7xLp2tJ3q/edit?usp=sharing&ouid=102573514213912402103&rtpof=true&sd=true)

[Metadata Sheet](https://docs.google.com/spreadsheets/d/1yKsZ2FEw8-cWufvY8l31Ju8NTKujmEtb/edit?usp=sharing&ouid=102573514213912402103&rtpof=true&sd=true)


## <ins>1) Convert raw autoExecute data to mzML via MSConvert.<ins>

#### * *If your files have already been converted to mzML, proceed to step 4a for IDBac analysis or 4b for database deposition* *
   
   1) Select browse to  your Bruker FID file by clicking 'Browse'.
   
   2) Click 'Add' to submit your file to the conversion cue.
   
   3) Select where you would like your file to be saved under "Output Directory".
   
   4) Ensure mzML is selected under 'Options/Output format'.
   
   5) When the previous steps are completed, click 'Start'.

   6) The output of this conversion will be a single autoexecute mzML for the entire plate (this single file will be split in the "Idbac_split_maldi_workflow" section below). 

<img width="938" alt="Picture1" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/ce5975a1-4177-4abe-b3da-fddf437f775d">

<img width="948" alt="Picture2" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/3f05f184-1d17-4d4e-80c8-cd4e92477fcd">

 
 ## <ins>2) Upload files to GNPS2.org
 
   1) Select "File Browser" found on the [GNPS2.org](https://gnps2.org/homepage) homepage.<ins>
   2) Create a new folder and upload your autoexecute mzmL, plate map and metadata sheets.
 


<img width="1096" alt="FileBrowserEx1" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/1bbcc5be-f17f-469b-81f0-864aed4022c6">

<img width="1119" alt="SourceExamples" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/25a5cc68-051f-43ce-bc6c-a9fe08bf1aba">



## <ins>3) Split re-name autoexecute file

This workflow will split your autoexecute data into individually labeled mzML files based on your plate map and well positions. 

   1) Open the [idbac_split_maldi workflow](https://gnps2.org/workflowinput?workflowname=idbac_split_maldi_workflow) 
   2) Select your autoExecute mzML and plate map from the drop down menu.
   3) Submit workflow.

<img width="991" alt="Finalsplitmaldi" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/f40702df-7337-47dc-92d0-fbef29742eee">


## <ins>4) Choose what you would like to do next:<ins>

   a) **IDBac Analysis:** Analyze spectra within your dataset indepedently, or compare against the IDBac protein database (See "Analysis options" below).

   b) **IDBac Protein Database Deposition:** Deposit metadata and spectra of genetically verified isolates into the IDBac database.

 <img width="992" alt="Picture4" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/438b762a-07d1-4dee-bd19-e7dd231bfb92">


## <ins> a) IDBac Analysis

**<ins>Submit workflow:** Select [idbac_analysis_workflow](https://gnps2.org/workflowinput?workflowname=idbac_analysis_workflow) and reference the following image for submission instructions.

*If you do not submit metadata during this step, you will have fewer analysis options.

<img width="994" alt="Analysis submission2" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/f99ab189-0686-4415-b848-bf4da0d8fd7e">


**<ins>Analysis options:** Once the idbac_analysis_workflow is complete, you have the ability to analyze your data through:

   i) Vizualize protein dendrogram: View a dendrogram of your isolates (excluding database seeds). 
   
   ii) Visualize with Metadata: If you selected a metadata column to display, it will appear within this protein dendrogram. NOTE: If you do not select a metadata column to display, a 504 error may be triggered upon clicking this tab.
      
   iii) Spectra summary: This option allows you to compare mirror plots of your spectra.

   iv) Dendrogram similarity: You may view similarity scores between your isolates based on the similarity metric you chose in the analysis workflow submission.
   
   v) Database Search Summary: Here you query protein spectra of your unknown isolate against our database of characterized bacterial strains (based on similairty scores).
   

<img width="986" alt="Finalanalysis" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/378353bc-0ee9-411b-a5c4-83bd6f286826">


## b) IDBac Database Deposition 

**<ins>Submit workflow:** Select [idbacdeposition_workflow](https://gnps2.org/workflowinput?workflowname=idbacdeposition_workflow) and reference the following image for deposition instructions.

<img width="993" alt="Databasesubmissionfinal" src="https://github.com/Wang-Bioinformatics-Lab/GNPS2_Documentation/assets/140128524/514765f1-560e-4dad-8307-c899993b907f">

**<ins>View Database**

To view your deposition, visit the [IDBac Knowledgebase](https://idbac-kb.gnps2.org/).













