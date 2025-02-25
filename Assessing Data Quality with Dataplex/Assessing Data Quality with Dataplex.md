![API Gateway Banner](https://raw.githubusercontent.com/Abhishek-kumar-202063/content/f9a8642976ea21cd234c91239431e41f05264842/gif/12.gif)

<div align="center">

# Connect with Cloud Hustlers Community
</div>

<p align="center">
  <a href="https://whatsapp.cloudhustlers.in" target="_blank">
    <img src="https://raw.githubusercontent.com/Abhishek-kumar-202063/content/f9a8642976ea21cd234c91239431e41f05264842/gif/whatsapp.gif" alt="WhatsApp" width="80">
  </a>
  <a href="https://in.linkedin.com/company/cloud-hustlers" target="_blank">
    <img src="https://raw.githubusercontent.com/Abhishek-kumar-202063/content/f9a8642976ea21cd234c91239431e41f05264842/gif/linkedin%20gif.gif" alt="LinkedIn" width="80">
  </a>
  <a href="https://www.youtube.com/@CloudHustlers" target="_blank">
    <img src="https://raw.githubusercontent.com/Abhishek-kumar-202063/content/f9a8642976ea21cd234c91239431e41f05264842/gif/youtube.png" alt="Youtube" width="80">
  </a>
  <a href="https://instagram.com/cloud_hustlers" target="_blank">
    <img src="https://raw.githubusercontent.com/Abhishek-kumar-202063/content/f9a8642976ea21cd234c91239431e41f05264842/gif/insta.gif" alt="Instagram" width="80">
  </a>
  <a href="https://discord.gg/MdbVq7BJNd" target="_blank">
    <img src="https://raw.githubusercontent.com/Abhishek-kumar-202063/content/f9a8642976ea21cd234c91239431e41f05264842/gif/discord.gif" alt="GitHub" width="80">
  </a>
</p>

# Assessing Data Quality with Dataplex || `[GSP1158]`

### Run the following Commands in Cloud Shell

```bash
export REGION=
```

```bash
gsutil cp gs://cloudhustlers/gsp1158.sh .

sudo chmod +x gsp1158.sh

./gsp1158.sh

echo "----------------------"
echo "                      "
echo "BIGQUERY LINK : https://console.cloud.google.com/bigquery?project=$DEVSHELL_PROJECT_ID&ws=!1m0"

echo "TASK LINK : https://console.cloud.google.com/dataplex/process/create-task/data-quality?project=$DEVSHELL_PROJECT_ID"

echo "----------------------"
echo "                      "
```

- Click `BigQuery` Link Or Go from [here](https://console.cloud.google.com/bigquery?)

- In the SQL Editor, click on `Compose a new query`. Paste the following query, and then click `Run`: ( REPLACE PROJECT_ID WITH YOUR PROJECT )

```bash
  SELECT * FROM `PROJECT_ID.customers.contact_info`
  ORDER BY id
  LIMIT 50
```

- CLICK `TASK LINK` >
- DATAPLEX LAKE : `ecommerce-lake`
- DISPLAY NAME : `Customer Data Quality Job`
- SELECT GCS FILE : `<PROJECT_ID>-bucket/dq-customer-raw-data.yaml`
- SELECT BIGQUERY DATASET : BROWSE > `customers_dq_dataset`
- SELECT BIGQUERY TABLE : `dq_results`
- USER SERVICE ACCOUNT : `Compute Engine default service account`
- `CONTINUE` > START IMMEDIATELY > `CREATE`

---

- CLICK Customer Data Quality Job > [RANDOM NUMBER JOB ID] > LET STATUS BE Succeeded
- BACK TO BIGQUERY LINK > EXPAND PROJECT ID > `customers_dq_dataset` > DOUBLE CLICK `dq_summary` >
- PREVIEW > SCROLL RIGHT TO THE END > IN LAST ROW FIRST COLUMN > MAKE THE ARROW TOWARD UPSIDE
- COPY WHOLE QUERY FROM THAT CELL > PASTE IN `BIGQUERY NEW EDITOR` > `RUN`
- AGAIN IN LAST ROW SECOND COLUMN > MAKE THE ARROW TOWARD UPSIDE
- COPY WHOLE QUERY FROM THAT CELL > PASTE IN BIGQUERY NEW EDITOR > RUN

### Congratulations for Completing the Lab !


</div>
<img src="https://raw.githubusercontent.com/Abhishek-kumar-202063/content/f9a8642976ea21cd234c91239431e41f05264842/gif/baby.gif" align="right" width="400">

<p align="left">
  <a href="https://youtu.be/8bQOoeeif7A">
    <img src="https://img.youtube.com/vi/8bQOoeeif7A/maxresdefault.jpg" width="500">
  </a>
</p>
