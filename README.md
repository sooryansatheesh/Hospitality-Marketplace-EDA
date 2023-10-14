# Hospitality Marketplace Dataset EDA

## Questions to Answer
- What are guests searching for in the city?
- Which inquiries do hosts tend to accept?
- What gaps exist between guest demand and host supply?
- Any other information that deepens the understanding of the data.

## Datasets
There are two datasets from Airbnb:
- **searches.tsv**: Contains a row for each set of searches that a user does for a city.
- **contacts.tsv**: Contains a row for every time that an assigned visitor makes an inquiry for a stay in a listing in the city.

### Searches Dataset
The searches dataset contains the following columns:
- **ds**: Date of the search.
- **id_user**: Alphanumeric user_id.
- **ds_checkin**: Date stamp of the check-in date of the search.
- **ds_checkout**: Date stamp of the check-out date of the search.
- **n_searches**: Number of searches in the search set.
- **n_nights**: The number of nights the search was for.
- **n_guests_min**: The minimum number of guests selected in a search set.
- **n_guests_max**: The maximum number of guests selected in a search set.
- **origin_country**: The country the search was from.
- **filter_price_min**: The value of the lower bound of the price filter if the user used it.
- **filter_price_max**: The value of the upper bound of the price filter if the user used it.
- **filter_room_types**: The room types that the user filtered by if the user used the room_types filter.
- **filter_neighborhoods**: The neighborhoods types that the user filtered by if the user used the neighborhoods filter.

### Contacts Dataset
The contacts dataset contains the following columns:
- **id_guest**: Alphanumeric user_id of the guest making the inquiry.
- **id_host**: Alphanumeric user_id of the host of the listing to which the inquiry is made.
- **id_listing**: Alphanumeric identifier for the listing to which the inquiry is made.
- **ts_contact_at**: UTC timestamp of the moment the inquiry is made.
- **ts_reply_at**: UTC timestamp of the moment the host replies to the inquiry, if so.
- **ts_accepted_at**: UTC timestamp of the moment the host accepts the inquiry, if so.
- **ts_booking_at**: UTC timestamp of the moment the booking is made, if so.
- **ds_checkin**: Date stamp of the check-in date of the inquiry.
- **ds_checkout**: Date stamp of the check-out date of the inquiry.
- **n_guests**: The number of guests the inquiry is for.
- **n_messages**: The total number of messages that were sent around this inquiry.

### Dependencies
-**Pandas** 2.0.3<br>
-**Numpy** 1.24.3<br>
-**Matplotlib** 3.7.1<br>
-**Seaborn** 0.12.2<br>

### How to Use
1.Ensure you have the required dependencies installed.<br>
2.Download the searches.tsv and contacts.tsv datasets from Airbnb.<br>
3.Replace the file paths in the code with the paths to your downloaded datasets.<br>
4.Run the provided Jupyter Notebook cells to perform exploratory data analysis on the datasets.<br>
5.Feel free to explore and analyze the datasets to answer the key questions outlined above.
