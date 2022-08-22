# Generating Synthetic Sensor Data - Workshop Instructions
<details>
<summary>Table of Contents</summary>
<p>

* [Log into RHODS](#logging-into-rhods)
* [Git Clone the Edge Synthetic Generator Project](#git-clone-the-edge-synthetic-generator-project)
* [Generate Sensor Data](#generate-sensor-data)
* [Select Slice](#select-slice)
* [Stream Sensor Data](#stream-sensor-data)

</p>
</details>

## Log into RHODS

1. Go to the [OpenShift console](https://console-openshift-console.apps.ieee.8goc.p1.openshiftapps.com/) and click on **WorkshopAttendees** and log in with your credentials.

    ![](/workshop/images/workshop_attendees.png)

2. Navigate Red Hat OpenShift Data Science (RHODS).

3. Click on **Log in with OpenShift** and then click on **WorkshopAttendees** and log in with your credentials.

    ![](/workshop/images/openshift_login.png)

4. Click on **Allow selected permissions** to authorize access. 

    ![](/workshop/images/authorize_access.png)

5. Once in the RHODS dashboard, click on the **Launch Application** hyperlink in the JupyterHub tile.

    ![](/workshop/images/rhods_jupyterhub.png)

6. Again, click on **WorkshopAttendees** and log in with your credentials and click on **Allow selected permissions**

6. Choose **Standard Data Science** as the notebook image and select a **small** notebook size.

    ![](/workshop/images/jupyterhub_nb.png)

7. Click on **Start Server**

## Git Clone the Edge Synthetic Generator Project 
1. On the left side of the navigation pane, locate the explorer panel. This panel is where you can create and manage your project directories. Go into the root directory of your JupyterLab enviroment by locating clicking the Folder icon.

    ![](/workshop/images/directory.png)

2. Click on the Git icon on the left of your JupyterHub notebook.


3. Click on the **Clone a Repository** button.

    ![](/workshop/images/git_clone.png)

4. Paste the following URL and click **Clone**.
 
    ```
    https://github.com/Enterprise-Neurosystem/edge-synthetic-data-generator.git
    ```
## Generate Sensor Data

1. Now that we've cloned the project, let's generate synthetic sensor data from a notebook. 

2. Open the notebook named `12_generate_sensor_data.ipynb` from the File Explorer tab. 

    ![](/workshop/images/generate_sensor_data.png)

3.  Run the first cell to install the required packages for this workshop by selecting it and clicking on the run button.

    ![](/workshop/images/run_cells.png)

4. Next, in the following cell, replace **None** with the GROUP_ID number provided to you and run it.

    ![](/workshop/images/group_id.png)

5. Afterwards, select and run cells 3-7 to generate synthetic data from a pre-trained model and plot some slices of it.


## Select Slice

1. Once you run the first 7 cells and reach the section titled **Selecting your slice**, enter in your slice number in the following cell. For example, if your slice number is 13, your code should resemble the following:

    ![](/workshop/images/select_slice.png)

2. After inputting your slice number, run the cell to plot the sensor data for that slice:

    ![](/workshop/images/slice_13_plot.png)

3. You are now finished with this part of the workshop. Next, you will be looking at how we 
[predict anomaly failure](https://github.com/Enterprise-Neurosystem/edge-prediction-failure/blob/main/workshop/instructions.md). 











