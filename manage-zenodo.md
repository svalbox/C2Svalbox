# Zenodo data management

```{figure} ./figs/zenodo-backend_communities.gif
---
name: zenodo-backend_communities
---

Once logged into Zenodo, data managers can access all submission requests in the Zenodo Svalbox community.
Data managers have full access to the data sets and should download all files within a request for manual inspection prior to approval/submission to the Svalbox databases.
```

```{figure} ./figs/zenodo-backend_comment.gif
---
name: zenodo-backend_comment
---

Each data request contains a conversation/discussion portal in which managers can discuss improvements of the data sets with the end users.
Through this portal users can also be notified of revisions that must be made to the data package prior to approval.
```

```{figure} ./figs/zenodo-backend_edit.gif
---
name: zenodo-backend_edit
---

Data managers can freely edit the submission and update metadata.
Make sure to select *Save draft* rather than *Accept and publish* when doing so!
The latter should only be done once the data have been inspected and curated.
```


```{figure} ./figs/zenodo-backend_download.gif
---
name: zenodo-backend_download
---

Downloading data is easy - just download all in the submission at once and save it to your drive.
```

````{admonition} Download, extract and update the config file
:class: tip

Once you have downloaded the full data set and unzipped all folders into the standardised environment, it it time to double check all contents and update the configuration file.
The following steps are recommended:

1. Check the folder structure. Are all images there and in the right folders? Is there GNSS/gcp data? Make sure it is correctly placed. Are the processing reports present in both .html and .pdf formats?
2. Open the Metashape project. Make sure all files are correctly linked, no missing images are present, and only one chunk exists per project. Also generate the processing reports, if needed.
3. Check the export folder. If needed, export the mesh/model in .obj format using CRS = EPSG:32633 (the CRS used by the Svalbox DB).
4. Update the config.yml file. Add in the DOI and update local path links where applicable.

Note the config.yml file path - as it is needed in the next steps.

```{admonition} Data/metadata missing?
:class: warning

Check everything the best you can - you are the last line of defence between faulty data being uploaded to the servers.
If there are large errors in the data, notify the creator and ask them to fix the sources per {numref}`zenodo-backend_comment`.

```
````


````{admonition} Downloaded the full data set?
:class: seealso

Once you have downloaded the full data set and unzipped all folders into the standardised environment, it it time to head over to the [](svalbox:db:management) tutorial.
That tutorial will 

````