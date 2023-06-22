# New York City Airbnb popularity prediction 🌃📈

## Welcome!  <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30">

Welcome and thank you for stopping by. This project focuses on a regression problem, aiming to demonstrate the various steps involved in developing a Machine Learning pipeline (pre-implementation stage), rather than emphasizing the intricacies of the modeling itself.

## Table of contents

- [Motivation](#motivation)
- [About the data](#about-the-data)
- [Description](#description)
- [About the data](#about-the-data)
- [Results](#results)
- [Dependencies](#dependencies)
- [Contributing](#contributing)

## Motivation

The objective of our model is to **predict the popularity of accommodations**, utilizing the objective variable `reviews_per_month`. This target variable serves as a reliable proxy for popularity since Airbnb incentivizes users to leave reviews on the platform. Consequently, reviews play a crucial role in decision-making when selecting accommodations from the numerous available options.

## About the data

The dataset comprises properties listed on Airbnb in New York in 2019. Each record in the dataset is associated with a unique identifier (id) and includes 15 attributes related to each property. Among these attributes, 6 are categorical, while 9 are numeric, encompassing both discrete and continuous values. The attributes provide information about the host, geographic location, property type, price, restrictions, and reviews. The dataset is substantial, containing nearly 49,000 records before any processing is performed. Below is a summary of the variables of the dataset:

|variable |class     |description |
|:--------|:---------|:-----------|
|id                              |   int64  | Listing ID |
|name                            | character | Listing name|
| host_id                        |  int64  | Host ID|
| host_name                       |  character | Host name|
| neighbourhood_group             | character | Neighbourhood location|
| neighbourhood                   | character | Neighbourhood area|
| latitude                        | float64 | Latitude coordinates|
| longitude                       | float64 | Longitude coordinates|
| room_type                       | character | Listing space type (Entire home/apt, Private room, Other)|
| price                           | int64  | Price in dollars|
| minimum_nights                  | int64  | Count of nights minimum|
| number_of_reviews               | int64  | Number of reviews|
| last_review                     | character | Latest review|
| reviews_per_month               | float64 | Number of reviews per month|
| calculated_host_listings_count  | int64  | Count of listing per host|
| availability_365                | int64  | Number of days when listing is available for booking|

The data set is public and can be found in [kaggle](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data).

## Results

Please go to [Notebook](https://github.com/AguilarRaul/Airbnb_price/blob/main/notebooks/airbnb_regression.ipynb).

## Dependencies

1. I have created an environment `environment.yaml`, for the project to be reproduced locally. To create this environment locally, go to the root of this repository and run:

    ``` bash
    conda env create -f environment.yaml
    ```

2. Activate it by running:

        conda activate Airbnb

## Contributing

Interested in contributing? We are glad you are interested, please check out the [contributing guidelines](https://github.com/AguilarRaul/Airbnb_price/blob/main/CONTRIBUTING.md). Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.

## License

This project was created by Raul Aguilar Lopez. The materials of this project are licensed under the MIT License. If re-using/re-mixing please provide attribution and link to this webpage.
