# 12-digit-unicode-reader-from-photos
Extracts 12 digit unicode from image with multiple features

## About
This tool extracts 12 digit aadhar number from multiple feature image for KYC related operation
This algorithm uses
Maximally Stable Extremal Regions (MSER) are used as a method of blob detection in images.<p>*Blob: blob is a region of an image in which some properties are constant or approximately constant; all the points in a blob can be considered in some sense to be similar to each other*.
<p>It is then filttered through a threshold value. Extract the mser detect feature and combine the edges using graph which removes overlap features. This helps to classify different blob feature.
Create a matrix which will hold the combined cordinate points of contour of related features.
<p> Apply OCR on the image created on the basis of  matrix, which will extract strings at the targeted area. Then apply regular expression for the text format required</p>


