# YouTube Analytics Project

## Overview
This project provides insights into YouTube channel and video performance using data analysis. It analyzes metrics such as subscriber count, total views, video performance, and monthly trends to help creators and analysts make informed decisions.

## Features
- Scrape data from YouTube using the YouTube Data API.
- Analyze channel statistics (subscribers, views, videos).
- Identify top-performing videos based on views, likes, and comments.
- Monthly performance trends for video views.
- Export analysis as image reports and CSV data files.

## Files
### 1. `YT-Analysis-Project.ipynb`
A Jupyter Notebook containing the code to scrape, clean, and analyze YouTube channel and video data. It also generates visualizations and exports data.

### 2. `Channel_Stats`
Contains metadata for analyzed YouTube channels:
- `Channel_name`: Name of the channel.
- `Subscribers`: Subscriber count.
- `Views`: Total views across the channel.
- `Total_videos`: Number of uploaded videos.
- `playlist_id`: ID of the channel's uploaded videos playlist.

### 3. `Video_details`
Details of individual videos on the channel:
- `Title`: Video title.
- `Published_date`: Date of publication.
- `Views`: Total views.
- `Likes`: Total likes.
- `Comments`: Total comments.
- `Month`: Month of publication.

### 4. Output Files
- **Image Reports**: Graphs and visualizations generated during analysis are saved as image files (e.g., PNG).
- **CSV Data Files**: Processed and summarized data is exported for further use.

## Data Collection
### YouTube Data API
- Data is scraped using the [YouTube Data API v3](https://developers.google.com/youtube/v3).
- Information about channels, playlists, and videos is retrieved, including metrics such as:
  - Subscriber count
  - Total views
  - Video details (e.g., title, likes, views, comments)

### Data Cleaning
- Missing or incomplete data entries are identified and handled appropriately.
- Timestamps are converted to structured date formats for trend analysis.
- Irrelevant columns or redundant data are removed to streamline analysis.
- Data is grouped and aggregated for generating summaries.

## Getting Started
### Prerequisites
Ensure the following Python libraries are installed:
- `pandas`
- `matplotlib`
- `seaborn`
- `google-api-python-client`
- `jupyter`

To install the dependencies:
pip install pandas matplotlib seaborn google-api-python-client jupyter

### Usage
1. **API Key Setup**:
   - Obtain an API key from the [Google Cloud Console](https://console.cloud.google.com/).
   - Replace the placeholder in the notebook with your API key to enable data scraping.

2. **Run the Notebook**:
   - Open the `YT-Analysis-Project.ipynb` file in Jupyter Notebook.
   - Execute all cells to scrape data, clean it, perform analysis, and generate graphs.

3. **Generate Reports**:
   - Save graphs as image files (e.g., PNG).
   - Export processed data to CSV files.

4. **Customize for Your Data**:
   - Replace `Channel_Stats` and `Video_details` with your own datasets in the same format to analyze different YouTube channels or videos.

## Project Highlights
- Scrape accurate and real-time data from YouTube using the official API.
- Clean and preprocess data for robust analysis.
- Provides visual summaries (images) and processed data in CSV format.
- Easily adaptable for other datasets.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing
Contributions are welcome! Feel free to fork this repository and submit pull requests with improvements or additional features.

