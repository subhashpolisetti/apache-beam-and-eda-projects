
# Apache Beam Pipeline for Movie Data Processing

## **Project Overview**
This project demonstrates the use of Apache Beam to process movie data, including filtering, transforming, and windowing operations. The pipeline simulates streaming data and applies composite transforms and triggers to handle real-time processing.

## **Key Features**
- **Composite Transforms:** Encapsulates multiple steps into reusable components.
- **ParDo:** Processes individual elements with custom logic.
- **Windowing and Triggers:** Divides data into fixed time intervals and processes it with a trigger.
- **Simulated Streaming:** Generates dynamic streaming data for real-time processing.
- **Dynamic Outputs:** Results are written to Google Drive for easy access.

## **Pipeline Steps**
1. **Data Simulation:** Generate a sequence of movie-related data.
2. **Parse Data:** Convert raw CSV lines or generated data into structured dictionaries.
3. **Windowing:** Apply fixed windowing (60-second intervals) for data grouping.
4. **Composite Transforms:** Filter movie data and extract relevant fields (title and country).
5. **Formatting:** Use custom ParDo transforms to format the output.
6. **Output:** Save the processed results to a text file in Google Drive.

## **Technologies Used**
- **Python**: Programming language for implementation.
- **Apache Beam**: Distributed data processing framework.
- **Google Colab**: Interactive notebook environment.
- **Google Drive**: Storage for input and output files.

## **File Structure**
- `input/netflix_titles.csv`: Input dataset containing Netflix movie and TV show details.
- `output/movies_output.txt`: Processed output file saved in Google Drive.

## **How to Run**
1. **Setup Environment**:
   - Install Apache Beam: `!pip install apache-beam`
   - Mount Google Drive: `from google.colab import drive; drive.mount('/content/drive')`

2. **Run the Pipeline**:
   - Execute the Python script in Google Colab.
   - Replace `input/netflix_titles.csv` with your dataset if required.

3. **View Results**:
   - Check the output file in your Google Drive under `output/movies_output.txt`.

## **Expected Output**
Each line in the output file represents a movie's title and its country:
```
Title_0: Country_0
Title_1: Country_1
...
```

## **Customization**
- Modify the `ProcessMovies` transform to extract additional fields.
- Adjust windowing parameters to fit your data processing needs.
- Replace simulated data with a live data source or batch dataset.



**Happy Coding!**
