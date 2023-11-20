# Running the Code
The file you've received includes stored output, enabling you to review both the code and its output without immediate execution. For a successful run of our movie recommendation system code, please follow the following steps:

### 1) Using Google Colab:

Our code is optimized for Google Colab. You'll need a Google account to access Google Colab. Alternatively, you can run the code on your own computer or a different server, though be aware that using your own CPU might extend processing times.

### 2) Dataset Preparation:

Obtain the datasets for each streaming platform from the indicated sources. If needed, we can share a Google Drive link with your email. Please ensure that these datasets are organized in your Google Drive following a specific file structure:


```
My Drive
├── data
    ├── amazon
    │   ├── titles.csv
    │   └── credits.csv
    ├── chrunchyroll
    │   ├── titles.csv
    │   └── credits.csv
    ├── darkmatter
    │   ├── titles.csv
    │   └── credits.csv
    ├── disney
    │   ├── titles.csv
    │   └── credits.csv
    ├── hbo
    │   ├── titles.csv
    │   └── credits.csv
    ├── hulu
    │   ├── titles.csv
    │   └── credits.csv
    ├── netflix
    │   ├── titles.csv
    │   └── credits.csv
    ├── paramount
    │   ├── titles.csv
    │   └── credits.csv
    ├── rakutenviki
    │   ├── titles.csv
    │   └── credits.csv
    └── apple
        ├── titles.csv
        └── credits.csv
```
        
### 3) Running the Code:

Open the code file in Google Colab.
Run each cell sequentially. The first cell will mount your Google Drive, and subsequent cells will load the datasets from the specified paths.
Ensure the drive_path variable in the code matches the location where you have stored the data folders in your Google Drive.



