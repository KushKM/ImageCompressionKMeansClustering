# Image Compression Using K-Means Clustering

Authors:
Kush Momaya, Jeric Pascua, Sarah Armstrong, Pysey Ung, Eli Line-Im

## Project Proposal - Image Compression

Our team project group proposal is about the compression of images through the K-means Clustering algorithm. K-means clustering is an algorithm in which objects are classified into different classes based on some sort of distance measure that is calculated between the objects. The clusters are then optimized through the reduction of their number or the change in their center. Image compression is the process of reducing the amount of space that an image takes through the reduction of unique colors. Additionally, the image must remain at a reasonable quality throughout the compression. We would like to explore the effectiveness of K-means Clustering across three different types of categories of images such as animals, buildings, and human faces. We would decide a number of clusters for each image and reduce that number until we see a significant decrease in the quality of the image. To optimize the number of clusters we would use the elbow method, where we plot the number of clusters, compared with a measure of variance to see which k would have the least impact on the reduction of quality. We would do this by using a for loop to calculate the SSE for a range of k-values for each image, and plotting the k-value and its related SSE. We would then compare the optimal k-value with what image appears to keep the important characteristics of the image. Furthermore, for each category, we would like to explore different images and discover the impact that changing the value of k has on each photo. From this, we can take the mean of k from each category, and compare the average k across all three categories. Our initial look at our data would be vectorizing the images and comparing their RGB values to see what kind of variance exists in the values for each image. We can then look at what this tells us about the k-values, both within categories and between categories. 

#### **Dataset:** https://drive.google.com/drive/folders/15OMJmn_gXL473LKGaDbD9ssrF8-GhgeA?usp=sharing

##### Also located in original_images folder

## Contributions:

Kush Momaya: Used the K-means algorithm to compress and analyze 2 building images, constructed elbow graphs for each, performed EDA by vectorizing every image and plotting their respective bar charts. Performed data cleaning and preprocessing for the data by creating dataframes for each image to create visualizations. This involved analysis of color patterns when looking at EDA graphs and construction of initial hypotheses regarding the effects of image compression.

Pysey Ung: Conducted K-means image compression on human face and building images, constructed elbow graphs for each, and analyzed the results of the different k-values and optimal cluster size. Retrieved images to add to the dataset.

Sarah Armstrong: Used K-means clustering on human face images along with their respective elbow graphs and analyses, retrieved images to add to the dataset

Jeric Pascua: K-Means image compression on nature and building images, exploratory data analysis using elbow graphs, and visual analysis comparing the results of each K-value effect on the original images, retrieved images to add to the dataset

Eli Line-Im: Ran K mean algorithm on two nature images along with creating an elbow graph for each of the two nature images, as well as conducting their respective analysis. Retrieved images to add to the dataset.

## Techniques
We are using pandas and numpy for parts of our EDA and generating our elbow graphs so we can visualize our results and perform various calculations. Matplotlib helps with visualizing the data as well. The skimage library is what allows us to import and use the image in tandem with the sklearn library from which we import the k-means clustering algorithm. Finally we use the cv2 library to import images and vectorize them alongside pandas for the EDA part.

## Data Collection & Cleaning
We read in the images through