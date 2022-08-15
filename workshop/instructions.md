# Generating Synthetic Sensor Data - Workshop Instructions
<details>
<summary>Table of Contents</summary>
<p>

* [Log into RHODS](#logging-into-rhods)
* [Git Clone the Edge Synthetic Generator Project](#git-clone-the-edge-synthetic-generator-project)
* [Generate Sensor Data](#generate-sensor-data)

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

7. Click on "Start Server"

## Git Clone the Edge Synthetic Generator Project 
1. Click on the Git icon on the left of your JupyterHub notebook. 

2. Click on the **Clone a Repository** button.

    ![](/workshop/images/git_clone.png)

3. Paste the following URL and click **Clone**.
 
    ```
    https://github.com/Enterprise-Neurosystem/edge-synthetic-data-generator.git
    ```
## Generate Sensor Data

1. Now that we've cloned the project, let's generate synthetic sensor data from a notebook. 

2. Open the notebook named `12_generate_sensor_data.ipynb` from the File Explorer tab. 

    ![](/workshop/images/generate_sensor_data.png)

3.  Select the Run menu, then the last option, **Restart Kernel and Run All Cells** which will: 
    * Prompt the pretrained model, `dgan_model_5_48_sensors.pt`, to generate 1000 samples of 12 hour slices of data. 
    * Plot some of the synthetic data. 
    * Attach a timestamp to each instance of synthetic data, thereby making it time series data.
    * Stream a slice of the synthetic data via Apache Kafka to the sensor failure prediction model for ingestion. 

         ![](/workshop/images/restart_kernel.png)










