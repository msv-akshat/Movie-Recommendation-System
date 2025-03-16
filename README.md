# Movie-Recommendation-System

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: MADAMSETTY SAI VENKAT AKSHAT

*INTERN ID*: CT08UFI

*DOMAIN*: JAVA

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

## Project Overview

The Movie Recommendation System processes user-item interaction data, such as movie ratings, to recommend movies to users. The system uses a Tanimoto Coefficient for similarity calculation and Mahout's collaborative filtering model to generate the recommendations.

## Key Features

Item-based Collaborative Filtering: The recommender suggests items based on the similarity between items (movies).

Tanimoto Coefficient Similarity: This similarity measure is used to calculate how similar two items are.

Movie Title Mapping: The system maps movie IDs to titles for easy interpretation of results.

## Technologies Used

Apache Mahout: Provides the framework for collaborative filtering algorithms.

Java: The primary language used for the implementation.

CSV: The data is stored in CSV format, which includes movie ratings and movie information.

## Setup Instructions

### 1. Clone the Repository

Start by cloning this repository:

```bash
git clone https://github.com/yourusername/movierecommendator.git
cd movierecommendator
```

## 2. Add Required Libraries

Download the necessary .jar files for Apache Mahout, Commons Math, Guava, and SLF4J and place them in the lib/ directory.

-Apache Mahout Core

-Guava

-SLF4J

Make sure you have the following JARs in the lib/ folder:

-commons-math3-3.2.jar

-guava-15.0.jar

-mahout-core-0.8.jar

-mahout-integration-0.8.jar

-mahout-math-0.8.jar

-slf4j-api-1.7.5.jar

-slf4j-nop-1.7.5.jar

## 3. Compile the Project
Navigate to the project root and run:

```bash
javac -cp "lib/*" -d bin src/com/predictionmarketing/convert/MovieDataConvert.java src/com/predictionmarketing/itemrecommend/ItemRecommend.java
```
This compiles the Java files and places the .class files in the bin/ folder.

## 4. Run the Data Conversion
The MovieDataConvert class converts the original dataset u.data into a CSV format (movies.csv). Run it first to process the data.

```bash
java -cp "bin;lib/*" com.predictionmarketing.convert.MovieDataConvert
```

## 5. Run the Recommendation Engine
After conversion, run the recommendation system to generate movie recommendations.

```bash
java -cp "bin;lib/*" com.predictionmarketing.itemrecommend.ItemRecommend
```

The system will output the movie recommendations along with similarity scores.
