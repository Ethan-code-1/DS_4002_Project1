# DS_4002_Project1

Authors: Seble Alemu (cnd3ru@virginia.edu), Janna Serrao	(jhs5gq@virginia.edu), Ethan Ogilvie (ebo4dq@virginia.edu)

Project Topic: Using Sentiment Analysis to Predict Movie Rating Based on Amazon Prime User Reviews
- We utilized amazon review text to try and predict the star rating a user would assign to a product based solely on the body of text associated with a review. 
<h2>Section 1: Software and Packages</h2>
<b>Software:</b> Rivanna OnDemand or Vscode <br>
<b>Platform:</b> Jupyter Notebook<br>
<b>Packages:</b> you will need to install the following packages if they are not already available
 <table>
  <tr>
    <th>Package</th>
    <th>Purpose</th>
  </tr>
  <tr>
    <td>numpy</td>
    <td>math operations, store data as an array</td>
  </tr>
  <tr>
    <td>pandas</td>
    <td>clean + process + explore data</td>
  </tr>
   <tr>
    <td>json</td>
    <td>to read json data files</td>
  </tr>
   <tr>
    <td>matplotlib</td>
    <td>create plots</td>
  </tr>
   <tr>
    <td>seaborn</td>
    <td>create plots</td>
  </tr>
   <tr>
    <td>nltk</td>
    <td>produce sentiment score analysis</td>
  </tr>
   <tr>
    <td>VADER</td>
    <td>produce sentiment scores and parse through text data</td>
  </tr>
   <tr>
    <td>Skit-learn</td>
    <td>to form predictive model and test it</td>
  </tr>
</table> 

<h2>Section 2: Documentation Tree</h2>

View via <a href = "https://miro.com/app/board/uXjVLk8cn0k=/?share_link_id=197416515122">this link! </a>

<h2>Section 3: Instructions to Reproduce Results</h2>

1. Download Needed Scripts and Data:

Create a folder in your hard drive to store files locally for this project (a suggested folder name is “Amazon_Rating_Model”). Once the folder is made, go to the DATA folder of this repository and download the both the  movies_metadata_reduced.jsonl and  json_file_size_reductio﻿n.ipynb. These data files are reduced in size and cleaned from the original datasets, since the process to do so is very finicky and time consuming. If you are interested in recreating this project with the original data set, or understanding the initial sampling process to create this data set, please see “Guide to Original Dataset” section below. Otherwise, please move on to step 2.

Guide to Original Dataset: Download the original raw data files from the  from <a href = "https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023/tree/main">the amazon repository here </a> located as follows: Amazon-Reviews-2023/raw/review_categories/Movies_and_TV.jsonl and Amazon-Reviews-2023/raw/meta_categories/meta_Movies_and_TV.jsonl. Save them to the folder you just created to run this project. Next, go to the SCRIPTS folder of the repository and download json_file_size_reduction.ipynb to save to your custom folder for this project. Using your software of choice, open the file and run each code chunk in order. A random sample of movies and their reviews has been taken from the dataset. This is to streamline the process of data analysis and model building as the data set is extremely large and cumbersome. The sample data includes product reviews that are matched to the product key ID assigned from the item metadata. After grouping reviews to the appropriate movie, a random 99% of the groupings were dropped. This allowed the data to fit within the data storage limits of the GitHub repository (<2GB). The resulting dataset contains all the reviews associated with roughly 7,500 movies (1% of the total movies in the dataset).
  
2. Running the Analysis script.

Go to the SCRIPTS folder from this repository. Download the file [jproject 1 analysis.ipynb] and save to the custom folder you created for this project. Open the file in your choice code editing software (we recommend using Vscode or using UVA Rivanna OnDemand to run Jupyter Notebook). Take note of libraries you may not have installed, they are listed in the first code chunk.  See the table above for the names of the necessary packages to install. Once libraries are installed, run the first code chunk to make sure you have all libraries needed. Before continuing, check the file path assigned to the objects “file_rev” and “file_meta.” This is how the script recognizes your dataset. Make sure the filepath matches the path saved locally on your computer. If the script is saved to the same folder as the data files, you should only need to have the string of the filename. After you have checked this, run the next code chunk, as well as the rest of the code chunks in the file. 

As results load, take time to review the comments in the code to understand each step. At the end of the file are the figures, which you can find blown up as individual images in the OUTPUT folder of this repository.


3. Review the Results

You can evaluate the success of your results by checking the figures produced with those stored in the OUTPUT folder. If you are confused by the variables analyzed in the final predictor model results, which only came from review dataset, please check the Data Appendix in the DATA folder.

Questions? Error messages? Concerns? Feel free to contact the authors! Our emails are found at the top of this file.

