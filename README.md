# Hotel Booking Analysis
<img src="https://images.unsplash.com/photo-1564501049412-61c2a3083791?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1632&q=80" alt="image" style="width:1000px;height:400px;">

#### <a href = "https://public.tableau.com/app/profile/bhaskar.kumar5658/viz/HotelBookingDashboard_16774308027600/Dashboard1?publish=yes"> <strong>Check out this Tableau Dashboard</strong> </a><br>

## 1. Project Description
The goal of this project is to analyze a hotel booking dataset and explore important factors that affect the bookings. The dataset includes information on bookings made at a city hotel and a resort hotel, including details such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces. By analyzing this data, we aim to answer questions such as when the best time of year to book a hotel room is, the optimal length of stay for the best daily rate, and whether or not a hotel is likely to receive a disproportionately high number of special requests. This dataset can help us understand the important factors that govern hotel bookings and can inform future strategies for hotel booking management. The dataset has had all personally identifying information removed to ensure privacy.

## 2. Dataset Description
The dataset used for this project consisted of 119,390 rows and 32 columns/features, with both numerical and categorical data types. The columns were named according to the following variables: hotel, is_canceled, lead_time, arrival_date_year, arrival_date_month, arrival_date_week_number, arrival_date_day_of_month, stays_in_weekend_nights, stays_in_week_nights, adults, children, babies, meal, country, market_segment, distribution_channel, is_repeated_guest, previous_cancellations, previous_bookings_not_canceled, reserved_room_type, assigned_room_type, booking_changes, deposit_type, agent, company, days_in_waiting_list, customer_type, adr, required_car_parking_spaces, total_of_special_requests, reservation_status, and reservation_status_date.

Some columns, such as country, agent, and company, contained null values. To address this, we imputed the mode value for the company column and the median value for the agent column. We also removed the company column entirely as it contained too many null values.

Data origininally extracted from: https://www.sciencedirect.com/science/article/pii/S2352340918315191#t0010

## 3. Analysis Summary
The Hotel Booking Analysis project aimed to assist individuals in successfully finding the cheapest available room based on multiple parameters. The provided dataset included booking patterns of both new and returning customers. The project involved several steps, including cleaning the data to ensure no null values were present, data wrangling over the non-null data, and dividing the analysis into multiple parts.

The analysis included City vs. Resort bookings, peak season for bookings, ADR (average daily rates), and cancellations. It was concluded that City hotels have more bookings than Resort hotels based on a dataset spanning three years. Charts were also used to visually understand the findings.

The busiest months for bookings were identified as April to August for both hotel types, with the fewest guests during the winter months. The analysis was done for both combined hotel types and individual hotel types, i.e., for Resort and City hotels.

Multiple factors played a role in cancellations, including lead time, deposit type, market segment, and previous cancellations. Charts were used to analyze the findings. Interestingly, in the case of City hotels, the months with the most bookings (May, June, September, October) also experienced the most cancellations. Guest numbers for Resort hotels slightly decreased from June to September, and both hotel types had very few guests during the winter season.

Overall, the analysis provided valuable insights into the most economically appropriate time for booking and helped teams make informed decisions based on the findings.

## 4. Methodology
Firstly, the data was inspected to determine the data types of each column, such as categorical, numerical, float, and integer. After that, univariate analysis was conducted on each column to understand the distribution of data within each of them. This was followed by bivariate analysis to identify correlations and relationships between different variables. Finally, multivariate analysis was performed to gain a deeper understanding of the data.

To perform the analysis, a Google Colab notebook was used, and Python programming language was utilized. The data was manipulated using Pandas and Numpy libraries, while Matplotlib and Seaborn were used for visualization purposes. Overall, these tools and techniques helped to extract valuable insights from the data, leading to meaningful conclusions.

## 5. Limitations and challenges
<ul>
  <li>Lack of contextual information: The dataset provided only contained limited information about each booking and did not provide any contextual information such as the reason for travel or the purpose of the trip. This made it challenging to draw accurate conclusions about booking patterns.</li>

  <li>Missing data: The dataset contained missing values, which had to be imputed or removed. Imputing missing values could introduce bias into the analysis, while removing them could reduce the amount of data available for analysis.</li>

  <li>Data quality issues: The dataset had some data quality issues, such as inconsistent data formats, incorrect data types, and incorrect values, which required data cleaning and preprocessing.</li>

  <li>Limited timeframe: The dataset contained bookings for a limited timeframe of 3 years, which may not be sufficient to draw long-term conclusions about booking patterns.</li>

  <li>Generalizability: The dataset contained information for only two hotels, one city hotel and one resort hotel, which may not be representative of the broader hotel industry. This limits the generalizability of the conclusions drawn from the analysis.</li>
</ul>

## 6. Conclusion
<ul>
  <li>2016 holds the most numbers of booking as per given dataset.</li>
  <li>Transient customer types have higher cancellations.</li>
  <li>Longer you stay in a resort, lesser adr will be experienced.</li>
  <li>Online TA segment leads the bookings.</li>
  <li>Higher lead time has higher chance of cancellation. Also, history of previous cancellations increases chances of cancellation.</li>
  <li>The City hotel has more guests during spring and autumn, when the prices are also highest, In July and August there are less visitors, although prices are lower. Thus, customers can get good deal on bookings in July and August in city hotel.</li>
  <li>Guest numbers for the Resort hotel go down slightly from June to September, which is also when the prices are highest. Thus, these months should be avoided for bookings.</li>
</ul>

## 7. References
<ol>
  <li> <i>GeekForGeek</i></li>
  <li> <i>Programmiz</i></li>
  <li> <i>AnalysticsVidhya</i></li>
</ol>
