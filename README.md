# Network-Links-Clustering-and-Traffic-Forecasting
Master's Graduation Project
# GitHub Repository README

## Network Links Clustering and Utilization Forecasting

This repository contains the implementation of a comprehensive project focused on clustering Vodafone network links using k-means and DBSCAN, along with forecasting their utilization on a monthly, weekly, and daily basis using various time series forecasting models such as ARIMA/SARIMA, Exponential Smoothing, Prophet, MLP, and LSTM.

### Required Libraries

Make sure to install the necessary Python libraries before running the code. You can install them using the following commands:

```bash
!pip install pmdarima
!pip install minisom
!pip install tslearn
!pip install prophet

### Interfaces and Utilities

The project includes utility classes for data extraction and modeling:

#### 1. ExtractorInterface

An abstract class defining methods for extracting, combining, converting, returning, and removing sheets.

#### 2. EmptyDataFrameException

An exception class raised when the values in the dataframe are empty.

#### 3. ModelingUtilities

A utility class providing methods for plotting, calculating metrics (MAPE and RMSE), and splitting datasets into training and validation sets.

### Implementation

The main implementation is divided into three parts:

#### 1. PreProcessor

This class contains methods for extracting date parts, grouping data, and creating datasets for machine learning models.

#### 2. Extractor

An interface for extracting sheets from emails, with implementations for Gmail and Outlook.

#### 3. EmailAttachmentExtractor

A class for extracting email attachments, bodies, and received dates from Outlook emails. It also includes methods for processing zip files, Excel files, and generating international summary sheets.

### Usage

To run the project, execute the `main()` function in the `__main__.py` file. The script will prompt you for necessary inputs, such as the output folder path, mailbox name, and folder name.

Feel free to explore and customize the code to suit your specific requirements. For any questions or issues, please refer to the documentation or open an issue in the repository.

Happy coding!
