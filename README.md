# Cryptocurrencies

# Overview:
A recongized investment bank is entering the cryptocurrency market and is interested in learning how to implement this new type of currency in it's portfolio options. A report is created using unsupervised machine learning, clustering algorithms, and visualizations to display which cryptocurrencies are currently on the trading market and how they can be classified for different types of investment strategies.

# Results:
To begin, the cryptocurrency data is preprocessed, meaning that the data is cleaned up to include only information which is deemed valid and necessary for creating a streamlined report. Null values are dropped as are columns with data which will not effect the integrity of the analysis. A cleaned cryptocurrency dataframe is stored and looks as follows:

<p align='center'>
          <img src="https://github.com/Shelka4444/Cryptocurrencies/blob/main/Images/Cleaned_DF.png" alt="Crypto DataFrame" width = 600>
                                            </p>
                                            
Using the StandardScaler algorithm, the cryptocurrency dataframe is scaled in preparation for the Principal Componenent Analysis (PCA) algorithm. PCA reduces the dimensions of the dataframe to, in this case, three principal components (PC1, PC2, PC3). Reducing dimensions not only assists the machines running the algorithms to run faster and more efficiently by transforming a large dataset into consolidated relational data without compromising the directionality of the original datasource.   
                                            
<p align='center'>
          <img src="https://github.com/Shelka4444/Cryptocurrencies/blob/main/Images/PCA_DF.png" alt="PCA DataFrame" width = 500>
                                            </p>  
Next, an Elbow Curve is used to determine the best value for K (see visualization below). In this case, k=4 is the appropriate value.

<p align='center'>
          <img src="https://github.com/Shelka4444/Cryptocurrencies/blob/main/Images/Elbow_Curve.png" alt="Elbow Curve" width = 800>
                                            </p>
                                       
The K-Means algorithm is then applied to cluster the cryptocurrencies from the scaled and reduced PCA dataframe. The predicted clusters are concatenated into a new dataframe: 
                                       
<p align='center'>
          <img src="https://github.com/Shelka4444/Cryptocurrencies/blob/main/Images/Clustered_DF.png" alt="Clustered DataFrame" width = 800>
                                            </p>             
                                            
Finally, several visualizations are rendered using the clustered dataframe. 

A 3d visualization of the clustered dataframe is created using Plotly Express:

<p align='center'>
          <img src="https://github.com/Shelka4444/Cryptocurrencies/blob/main/Images/Scatter_3D.png" alt="3D Scatter Plot" width = 800>
                                            </p>     
                                      
The data is once again cleaned and formatted into a table showing only 532 tradable cryptocurrencies: 

<p align='center'>
          <img src="https://github.com/Shelka4444/Cryptocurrencies/blob/main/Images/Current_Tradable_Table.png" alt="Tradable Table" width = 800>
                                            </p>
                                            
The scaled tradable cryptocurrencies table is further sorted for Total Coins Supply and Total Coin Mined. A final scatter plot displays the relationship between these two variables.:

<p align='center'>
          <img src="https://github.com/Shelka4444/Cryptocurrencies/blob/main/Images/Scatter_2D.png" alt="Supply and Mined Scatter Plot" width = 800>
                                            </p>  
                                      

# Summary:
Using several unsupervised machine learning algorithms, the crypocurrency market is efficiently analyzed for hidden patterns. The large dataset is formatted, tabulated, and visualized to showcase 532 viable up-to-date trading options. The investment bank should take further measures to assess which classifications of cryptocurrencies would be most appealing to current clients and future investors.                                                         
                                                         
                                                         
