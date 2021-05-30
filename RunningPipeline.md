## Running the data pipeline
* A data pipeline template is defined in an XML file under [nifi](nifi/templates), from operate pallet
click on upload template button:

  ![upload template](manual/04-fix-configuration.png)

* Choose the xml template from [nifi][nifi/templates] then click upload

  ![upload template](manual/06-select-template.png)

* From top menu, drag the template icon to the design area  

  ![add template](manual/01-drag-drop-template.png)
* then select the template
  
  ![add template](manual/02-select-template.png)

* After adding the template, you should see the data pipeline as below, see the warnings in 
yellow you need to fix before running the application
    
  ![Data pipeline](manual/02-fix-warnings.png)
    
* You need to activate the controllers configured in the pipeline by clicking on configuration icon (Gear) 

  ![Configuration](manual/04-fix-configuration.png)
  
* Navigate to controller services tab, you need to modify Neo4J connection pool by setting
    the password, click on configure icon then update the password property by setting it to test
    
  ![service configuration](manual/05-configure-neo4j.png)

* After configuring this service, you need to enable all other services, click on enable icon 
 for each service record 
    
  ![Enable services](manual/07-all-services.png)
  
* Make sure there are no warnings in pipeline 
* You can start the data pipeline now by clicking on start button

  ![running data pipeline](manual/09-start-pipeline.png)
  
* This pipeline waits for a CSV file to be generated under specific path, to generate this file, 
 navigate to jupyter notebook [http://localhost:8888](http://localhost:8888) 
 then you should see under work folder two CSV files: updated_issues.csv and update_emails.csv, you should
 copy them under result folder (create this folder if it is still not created):
 
    ![copy csv](manual/08-create-upload-path.png) 

* Navigate back to NiFi browser, you should see how bytes read and
  transferred between the pipeline processors 

  