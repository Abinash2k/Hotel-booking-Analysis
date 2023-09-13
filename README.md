# Hotel Bookings Exploratory Data Analysis

# Objective
I have been provided with a hotel bookings dataset.

Out main objective is performing EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.

# Dataset

I have been given a hotel booking dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

- Hotel: - The name of the hotel where the booking was made.
- is cancelled: - Whether the booking was cancelled (1) or not (0).
- Lead-time: - The number of days between booking and arrival.
- Arrival date year: - The year of the arrival date.
- Arrival date month: - The month of the arrival date.
- Arrival date week number: - The week number of the year for the arrival date.
- Arrival date day of month: - The day of the month for the arrival date.
- Stays in weekend nights: - Number of weekend nights (Saturday or Sunday) the guest stayed.
- Stays in week nights: - Number of weekday nights (Monday to Friday) the guest stayed.
- Adults: - Number of adults in the booking.
- Children: - Number of children in the booking.
- Babies: - Number of babies in the booking.
- Meal: - The type of meal booked.
- Country: - The country of origin of the guest.
- Market segment: - The market segment the booking belongs to.
- Distribution channel: - The distribution channel used for the booking.
- Is repeated guest: - Whether the guest is a repeated guest (1) or not (0).
- Previous cancellations: - Number of previous booking cancellations by the guest.
- Previous bookings not cancelled: - Number of previous bookings that were not cancelled by the guest.
- Reserved room type: - The originally booked room type.
- Assigned room type: - The room type assigned at check-in.
- Booking changes: - Number of changes made to the booking.
- Deposit type: - The type of deposit made for the booking.
- Agent: - ID of the travel agency that made the booking.
- company: - ID of the company if the booking was made on behalf of one.
- Days in waiting list: - Number of days the booking was on the waiting list before being confirmed.
- Customer type: - Type of booking (Contract, Group, Transient, Transient-Party).
- ADR: - Average Daily Rate (total spend divided by number of nights).
- Required car parking spaces: - Number of car parking spaces requested.
- Total of special requests: - Number of special requests made by the guest.
- Reservation status: - Current status of the reservation.
- Reservation status date: - Date at which the last status was set.

Total number of rows in data: 119390
Total number of columns: 32


# Data Cleaning

# (1) Handling null values
Null values in columns company, agent and children were replaced by 0.
Null values in column country were replaced by 'Unknown'.

# (2) Converting columns to appropriate data types
Changed data type of children, company and agent to int type.
Changed data type of reservation status date to date type.

# (4) Creating new columns
Created a new column for total stay by adding stays on weekend nights + stays on weeknights.
Created a new column for total people by adding adults + children + babies.


# Exploratory Data Analysis

Performed EDA and tried answering the following questions:

Q1. What is the cancellation by month?
Q2. How many people prefer what kind of meal?
Q3. How much is the price paid by guests on average per night?
Q4. What is the relation between arrival and waiting in hotel booking?
Q5. What is the relation between lead time and cancellation? 
Q6. Which type of people prefer which hotel the most?
Q7. How is the booking made?
Q8. Which hotel has been booked with no advance, has the refundable option?
Q9. In which month which hotel has the highest booking?
Q10. Which hotel has been booked by the maximum number of people?
Q11. Which are the top 10 countries with maximum night stays?
Q12. What is the percentage of confirmed bookings and cancellations? 

Mainly performed using pandas for dataframes and Matplotlib and Seaborn library for visualization and the following graph and plots were used:

Bar Plot.
Histogram.
Scatter Plot.
Pie Chart.
Line Plot.
Heatmap.
Box Plot

# Conclusions
-Around 60% bookings are for City hotel and 40% bookings are for Resort hotel, therefore City Hotel is busier than Resort hotel. Also the overall 
 adr of City hotel is slightly higher than Resort hotel.

-Both hotels have significantly higher booking cancellation rates

-Most of the guests came from unknown/other countries, with most of guests coming from Britain.

-Guests use different channels for making bookings out of which most preferred way is TA/TO.

-Maximum of bookings via TA/TO .

-Not getting same room as reserved, longer lead time and waiting time do not affect cancellation of bookings.

-July- August are the most busier and profitable months for both of hotels.
and many more.

Challenges
(1) There was a lot of duplicate data.
(2) Data was present in the wrong datatype format.
(3) Choosing appropriate visualization techniques to use was difficult.
(4) A lot of null values were there in the dataset.
