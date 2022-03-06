# machinebiennial-data
Anonymised interaction data from ai.biennial.com. 

The data are presented chronologically. The data format is as follows:
\[action\] \[imageid\] \[action\] \[imageid\] \[action\] \[imageid\] \[action\] \[imageid\] ...

Where:
- \[action\] is one of Open, Left, Right, Down, or Undo (O/L/R/D/U). 
- \[imageid\] is an integer representing one image of an artwork at the 2021 Liverpool Biennial. It is accessible at ai.biennial.com/img/gen/512/[imageid].jpg . For instance, image number 47 can be viewed at: https://ai.biennial.com/img/gen/512/47.jpg

The chain (\[action\] \[imageid\] \[action\] \[imageid\] ...) is therefore of the form:

**o46d11r13u11**

This indicates that the user opened with image 46, then went down (i.e. through combined text-text and image-image similarity) to image 11, then right (i.e. through multimodal text-image similarity) to image 13, then pressed 'undo' (labelled as 'back' in the user interface) taking the user back to image 11. 

The most recent co-curated biennials are visible at the following URL:

https://ai.biennial.com/#cocurated 

The web interface can also display a biennial pathway using the same data format explained above - for instance:

https://ai.biennial.com/#biennial-o46d11r13u11
