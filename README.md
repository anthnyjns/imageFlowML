# imageFlowML

Problem Statement(s): 
File transfer and analytics of imagery captured in the course of automated visual inspection applications (particularly aerial imagery from drones in infrastructure applications) continue to severly limit the overall ROI for businesses in this industry. Specific challenges include:
  - Large folder sizes with 100's of high resolution pictures and short videos.
  - Time consuming upload/download times for data transfer and analysis.
  - Tedious and time consuming operations to locate pertinent images.
  - Complications merging source data due to camera file naming conventions.
  - Costly challenges with image mearurements requiring expensive 3rd party applications and/or engineering firm support.
  
Test Objectives: 
1. Demonstrate the potential for utilizing a mix of Python scripts and deep learning model(s) to automate image workflows on an existing, complex data library (like cell towers). 
2. Identify limitations with the developed models and potential causes.
3. Develop recommendations for follow-on testing in this area.

Typical Process Flow:


Example Image State Diagram:


Test Priorities:
1. Create a Convolutional Neural Network (CNN) model for estimating the RAD orientation for a cell tower from a single top-down view image. We will utilize a generic labeling convention with the most north facing array as "A", the next around the compass as "B" and the 3rd as "C". The final output should include the array label, direction it faces, and confidence level.

2. Research if/how a CNN can be used to crop a specific classification criteria and save to a new folder. Test to validate capability and identify challenges and goals for future testing.

3. Utilize the model from step 2 above to create a training set for antenna angle estimates. Utilize a CNN model to estimate the rotation angle (as seen from above) of a properly classified cell tower antenna.

4. Test the capability of a CNN to accurately bin images based on a "gap estimate" between antennas. I will use the diameter of the support stantions (typically 48-51 mm) as the referrence for training.
