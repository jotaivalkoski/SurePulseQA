# Compression Testing QA 

Enter the sample creation menu of Sure Pulse
![Sample Creation](images/WhereToEnterSampleCreation.png)

Use the data in `data/Sample 014 Parameters.txt` to fill in the compression sample menu.
![Sample Parameters](images/sample_params.png)

Choose the correct bar setup from the QA.
![Bar Setup](images/choose_bar_setup.png)

Load and parse the data file `data/20160112-014.txt`. Correctly label the time, incident bar voltage column, and transmission bar voltage column.
![Process file](images/load_and_process1.png)

Open trim data and start trimming the Incident bar data. This data needs to be zeroed:

![Zero data](images/apply_zero_modifier.png)

Apply a 600KHz filter and select the incident pulse.
![Select Incident](images/apply_zero_modifier.png)

Proceed similarly for the reflected and transmitted pulse.
![Select Reflected](images/apply_zero_modifier_reflected.png)
![Select Transmitted](images/apply_zero_modifier_transmitted.png)

Save sample into a QA folder.

The expected result should be something like 
![Expected Result](images/expected_result.png)

Repeat for Samples 13 and 15 as well. You should get a cluster of three samples.

## Downsampling

One feature of Sure Pulse is the ability to downsample data to improve processing speed.

![Reduce data size](images/reduce_data_size_button.png)

Reduce the data size to 500 samples.

![Reduced Sample 14 ](images/Reduced_14.png)

## Global filters
Apply a global filter on load to the sample.

![Global Filter](images/global_load_data_filter.png)

Getting results like.

![Globally filtered 14](images/globally_filtered_14.png)

## Trim adjustment

Choose sample 14 in the trim adjustment. Choose stress
![Trim Adjust](images/trim_adjustment.png)

Getting results like.
![Adjusted Trim](images/adjusted_trim.png)
