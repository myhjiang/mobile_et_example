# Mini Examples for Analyzing Mobile Eye-tracking Data

Some mini examples of an exploratory analysis for mobile eye-tracking data collected in a mixed-methods approach for GI user research. 

This is a part of MSc. Thesis *A Solution to Analyze Mobile Eye-tracking Data for GI User Research* by Yuhao (Markie) Jiang, ITC-University of Twente, Enschede, The Netherlands, June 2020

## Analysis based on

- [my automated fixation mapping tool](https://github.com/myhjiang/et_mapping)
- [my think-aloud processing tool](https://github.com/myhjiang/aws_ta)
- [Plot.ly](https://plotly.com/python/)

## What it does

- processing: fixation mapping to real-world objects and screen contents 
- visualizing the mapped fixations: distribution and sequence
- visualizing fixations together with verbalizations and location data.

## Data

For file size limitations, the data folder does not contain video / audio data. 

The data folder contains:

- `export_fixation.tsv` fixation file exported with Tobii Pro Lab
- `mapped_fixation.tsv, replaced_mapped_fixation.tsv, screen_replaced_mapped_fixation.tsv, grouped_screen_replaced_mapped_fixation.tsv` mapped fixations,  outputs and processed outputs from [my automated fixation mapping tool](https://github.com/myhjiang/et_mapping)
- `gps.csv` GPS measurements along the segment
- `segment_protocol.tsv` transcribed think-aloud protocol segments
- `sync_fixation_protocol.tsv, sync_fixation_gps.tsv, sync_protocol_gps` synchronized files

## Notebooks

- `visual_attention.ipynb`  exploring the distribution and sequence of visual attention
- `fixation_protocol.ipynb` exploring fixations together with protocols
- `location_combined.ipynb` exploring fixations and protocols together with location data 

Detailed descriptions can be found within the notebooks.
***GitHub cannot show Plot.ly interactive plots properly in Notebooks. It's recommanded to use those notebooks locally***

### Notebook dependencies

- plotly (go, express and io)
- pandas
- numpy
- re
- bisect

## Example visualizations
**the plots folder contains all the plots generated in the notebooks (as static png)**  
- fixations on a map 
![fixation on a map](https://github.com/myhjiang/mobile_et_example/blob/master/plots/fixation_gps.PNG)  
- fixations and protocols on the same timeline
![fixation and protocols](https://github.com/myhjiang/mobile_et_example/blob/master/plots/fixation_protocol.PNG)

