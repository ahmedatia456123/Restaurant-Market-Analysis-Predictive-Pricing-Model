<p align="left">
  <a href="https://colab.research.google.com/drive/17hybci2ENtSJ4DEXN6jkFJkVQXJQeyES?usp=drive_link">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/, width=150, /></a>

</p>
# Restaurant Price Prediction Project
<div class="post-body entry-content" id="post-body-4166430334267218137" itemprop="description articleBody">
<div class="entry-title">
</div>
<div class="separator" style="clear: both;"><a href="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjI7AHhBQLqc7MoX-1v1zUfE-Dq3kJsukTuI_t4gA62aNJrKnonoY95KV5ZG1tUZ3t7YD2u4z36TA-bcpINfTvlrxdg6P_aYQUigJP9Ui-vW4QKKvl_r2oAbbUoX6rPYlzsm-nCugH9iQ_cBdBFv4qjVoddvCNzr-ZRTU5lOxkEwhB1XsEKoyY2es01kF0/s1600/pexels-igor-starkov-233202-1307698.jpg" style="display: block; padding: 1em 0; text-align: center; "></a></div>
<h2>Introduction to Analyzing the Zomato Dataset</h2>
<p>Analyzing the Zomato dataset offers valuable insights into the restaurant scene in Bengaluru, a city bustling with over 12,000 eateries that cater to a diverse range of culinary tastes from around the world. As new restaurants continue to open daily, the industry remains dynamic, with growing demand that presents both opportunities and challenges. For newcomers, competing with well-established establishments can be tough, especially when many restaurants offer similar fare.</p>

<p>Bengaluru, known as the IT hub of India, has a large population that relies heavily on dining out due to busy lifestyles, making the study of restaurant demographics crucial. This analysis aims to uncover key patterns and preferences, including:</p>

<ul>
  <li><strong>Explore the food and restaurant industry in the city.</strong></li>
  <li><strong>Analyze trends and identify opportunities for market entry or improvement.</strong></li>
  <li><strong>Uncover market characteristics and classify restaurants into five distinct groups.</strong></li>
  <li><strong>Conduct a detailed analysis of each restaurant group.</strong></li>
  <li><strong>Examine customer behavior to understand preferences and dislikes by analyzing reviews from various restaurants.</strong></li>
  <li><strong>Build a predictive model to assist in the pricing process for restaurants based on market pricing trends.</strong></li>
</ul>


<p>By studying these aspects, we can gain a deeper understanding of the restaurant landscape in Bengaluru, helping new and existing restaurants better align with local tastes and demands.</p>

<h2>Objectives</h2>
<p>The primary objective of this data analysis project is to identify the most promising investment opportunities in the restaurant and cafe sector in Bangalore. This involves analyzing various factors that influence the success and customer appeal of these establishments and developing machine learning models to support pricing strategies and enhance customer experience.</p>

<ul>
    <li><strong>Investment Analysis:</strong>
        <ul>
            <li><strong>Identify High-Performing Establishments:</strong> Analyze the data to pinpoint restaurants and cafes with high ratings, significant customer engagement, and strong financial performance indicators. Focus on key attributes such as location, type, and customer reviews to assess which establishments are likely to offer the best returns on investment.</li>
            <li><strong>Evaluate Pricing Strategies:</strong> Develop and implement machine learning models to predict optimal pricing for menu items based on factors such as location, type, and customer feedback. This will help establish competitive pricing that aligns with market expectations and maximizes profitability.</li>
        </ul>
    </li>
    <li><strong>Customer Experience Enhancement:</strong>
        <ul>
            <li><strong>Analyze Customer Preferences:</strong> Utilize the data to understand customer preferences regarding dish likes, cuisines, and other attributes. This will inform strategies to improve the dining experience by focusing on popular dishes, preferred cuisines, and services that enhance overall satisfaction.</li>
            <li><strong>Improve Engagement and Accessibility:</strong> Examine the impact of online ordering and table booking options on customer engagement and satisfaction. Determine how these features contribute to higher ratings and increased customer interactions.</li>
        </ul>
    </li>
    <li><strong>Classify Restaurants:</strong> Classify restaurants into different categories based on their customer characteristics, from lower class to high class.</li>
    <li><strong>Machine Learning Model Development:</strong>
        <ul>
            <li><strong>Predictive Pricing Model:</strong> Build and refine machine learning models to forecast prices for menu items based on historical data, restaurant type, location, and customer reviews. This model will provide insights into setting competitive prices that attract customers while ensuring profitability.</li>
            <li><strong>Enhancement Recommendations:</strong> Generate actionable recommendations for improving customer experience based on predictive analytics and historical trends. This will include suggestions for menu adjustments, service enhancements, and strategic changes to attract and retain customers.</li>
        </ul>
    </li>
</ul>

<h2>Scope</h2>
<p>This analysis covers restaurants listed on the Zomato website in Bengaluru, focusing on over 51,000 entries to identify trends and patterns that impact investment and customer experience. The project encompasses:</p>
<ul>
    <li>Data extraction and preprocessing to ensure accurate and relevant information.</li>
    <li>Exploratory data analysis (EDA) to uncover underlying patterns and insights.</li>
    <li>Classification of restaurants based on customer characteristics and satisfaction levels.</li>
    <li>Development of machine learning models to predict pricing and enhance customer engagement.</li>
</ul>

<h2>Data Features</h2>
<p>The dataset contains various features that provide detailed information about the restaurants. Below is a summary of each feature along with its description:</p>

<table border="1">
    <thead>
        <tr>
            <th>Feature</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>url</strong></td>
            <td>The URL of the restaurant's listing.</td>
        </tr>
        <tr>
            <td><strong>address</strong></td>
            <td>The physical address of the restaurant.</td>
        </tr>
        <tr>
            <td><strong>name</strong></td>
            <td>The name of the restaurant.</td>
        </tr>
        <tr>
            <td><strong>online_order</strong></td>
            <td>Indicates if online ordering is available (Yes/No).</td>
        </tr>
        <tr>
            <td><strong>book_table</strong></td>
            <td>Indicates if table booking is available (Yes/No).</td>
        </tr>
        <tr>
            <td><strong>rate</strong></td>
            <td>The rating of the restaurant.</td>
        </tr>
        <tr>
            <td><strong>votes</strong></td>
            <td>The number of votes or reviews the restaurant has received.</td>
        </tr>
        <tr>
            <td><strong>phone</strong></td>
            <td>The contact phone number of the restaurant.</td>
        </tr>
        <tr>
            <td><strong>location</strong></td>
            <td>The locality or area where the restaurant is located.</td>
        </tr>
        <tr>
            <td><strong>rest_type</strong></td>
            <td>The type of restaurant (e.g., Casual Dining, Fine Dining).</td>
        </tr>
        <tr>
            <td><strong>dish_liked</strong></td>
            <td>Dish recommendations or items liked by customers.</td>
        </tr>
        <tr>
            <td><strong>cuisines</strong></td>
            <td>The types of cuisine offered by the restaurant.</td>
        </tr>
        <tr>
            <td><strong>approx_cost(for two people)</strong></td>
            <td>The approximate cost of a meal for two people.</td>
        </tr>
        <tr>
            <td><strong>reviews_list</strong></td>
            <td>The list of customer reviews for the restaurant.</td>
        </tr>
        <tr>
            <td><strong>menu_item</strong></td>
            <td>The items available on the restaurant's menu.</td>
        </tr>
        <tr>
            <td><strong>listed_in(type)</strong></td>
            <td>The type of listing category (e.g., Dine-out, Drinks &amp; Nightlife).</td>
        </tr>
        <tr>
            <td><strong>listed_in(city)</strong></td>
            <td>The city where the restaurant is listed.</td>
        </tr>
    </tbody>
</table>

<h2>Data Limitations</h2>
<p>Several limitations affect the quality and accuracy of the data:</p>
<ul>
    <li><strong>Insufficient Reviews for Some Classes:</strong> Not all restaurant classes have a sufficient number of reviews to cover all aspects in sentiment analysis. This limits the comprehensiveness of the analysis for some categories.</li>
    <li><strong>Lack of Menu Pricing Details:</strong> Menu items do not contain specific prices, which can hinder accurate pricing predictions. Currently, the data only provides approximate costs for a meal for two people, which may not reflect the true cost of individual menu items.</li>
    <li><strong>Unorganized Address Data:</strong> The address field is not well-organized or clean, requiring human revision for accuracy. Address accuracy is crucial for effective clustering and machine learning model performance, and discrepancies in address data may affect the quality of location-based insights.</li>
</ul>

<h2>Stakeholders</h2>
<p>The stakeholders in this analysis include:</p>
<ul>
    <li><strong>Investors and Restaurant Owners:</strong> These stakeholders are interested in identifying high-performing establishments and optimizing pricing strategies. Insights from this analysis will help them make informed decisions on investments and operational adjustments to maximize profitability.</li>
    <li><strong>Customers:</strong> Restaurant patrons benefit from improved dining experiences and more accurate information about restaurant quality and pricing. Understanding customer preferences and trends will help restaurants better cater to their needs and enhance overall satisfaction.</li>
    <li><strong>Data Analysts and Machine Learning Engineers:</strong> These professionals are involved in building and refining models based on the analysis. The insights generated will support their efforts in developing predictive analytics tools and recommendations for enhancing customer experiences and pricing strategies.</li>
    <li><strong>Marketing and Business Development Teams:</strong> These teams use the analysis results to devise targeted marketing strategies and business development plans. By understanding market trends and customer preferences, they can create effective campaigns and promotional activities to attract and retain customers.</li>
</ul>

<p>By addressing the needs and interests of these stakeholders, this analysis aims to provide actionable insights that drive success in the competitive restaurant market in Bengaluru.</p>

<h2>Data Cleaning and Preparation</h2>

<h3>Missing Data</h3>

<p>To ensure data quality, we first need to address the missing data in the dataset. The following table summarizes the count of missing values for each feature:</p>

<table>
    <thead>
        <tr>
            <th>Feature</th>
            <th>Missing Values</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>url</td>
            <td>0</td>
        </tr>
        <tr>
            <td>address</td>
            <td>0</td>
        </tr>
        <tr>
            <td>name</td>
            <td>0</td>
        </tr>
        <tr>
            <td>online_order</td>
            <td>0</td>
        </tr>
        <tr>
            <td>book_table</td>
            <td>0</td>
        </tr>
        <tr>
            <td>rate</td>
            <td>7,775</td>
        </tr>
        <tr>
            <td>votes</td>
            <td>0</td>
        </tr>
        <tr>
            <td>phone</td>
            <td>1,208</td>
        </tr>
        <tr>
            <td>location</td>
            <td>21</td>
        </tr>
        <tr>
            <td>rest_type</td>
            <td>227</td>
        </tr>
        <tr>
            <td>dish_liked</td>
            <td>28,078</td>
        </tr>
        <tr>
            <td>cuisines</td>
            <td>45</td>
        </tr>
        <tr>
            <td>approx_cost(for two people)</td>
            <td>346</td>
        </tr>
        <tr>
            <td>reviews_list</td>
            <td>0</td>
        </tr>
        <tr>
            <td>menu_item</td>
            <td>0</td>
        </tr>
        <tr>
            <td>listed_in(type)</td>
            <td>0</td>
        </tr>
        <tr>
            <td>listed_in(city)</td>
            <td>0</td>
        </tr>
    </tbody>
</table>

<h3>Handling Missing Rate and Rate Distribution and Weighted Rating</h3>

<p>Handling the missing values in the rate column involves several steps:</p>
<ol>
    <li><strong>Calculate Ratings from Reviews:</strong> Derive ratings from the reviews_list column where available. Convert ratings from string format (e.g., 'Rated 3.0') to numeric float format (e.g., 3.0).</li>
    <li><strong>Handle Missing Ratings:</strong> For restaurants with no reviews, estimate their ratings using the average rating of restaurants in the same location.</li>
    <li><strong>Preserve 'NEW' Information:</strong> Create a new column named is_new with values 'yes' or 'no' to retain information about new establishments. This column will be converted to binary values (1 and 0) for modeling purposes.</li>
    <li><strong>Convert Ratings to Numeric Format:</strong> Convert ratings from string format (e.g., '4.6/5') to numeric float format (e.g., 4.6).</li>
</ol>

<p>After checking the distribution of ratings, we observed that many ratings are either 1 or 5, which is unrealistic. Some restaurants have a rating of 5 with only one vote, which can mislead the model. To address this:</p>

<img alt="Rate Distribution" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgofQ0L_HfD1O-tVYovyTF1uMVV8DlB-NEKIg-zyStCW65u53uK5LcPvf_gpE2qi5VzfVRCetz9FNgu7icyoC-OqRPIGYljKGbmErsnnYf7-yJ5QgglwKsGxAycb7c46mPKtkQye-ox-kjOg5Fak5HNfTlMr8LgOZV-dCrAZnwk0R0vdpb1FNCeYMvid3Q/s1600/download.png">

<p>This image shows that many ratings are skewed. We need to use a Weighted Rating to account for this bias.</p>

<p><strong>Weighted Rating Formula:</strong></p>
Weighted Rating = (v × r + m × c) / (v + m)
<p>where:</p>
<ul>
    <li>r = average rating of the item</li>
    <li>v = number of votes for the item</li>
    <li>m = minimum number of votes required to be listed (threshold)</li>
    <li>c = mean rating across all items</li>
</ul>

<h3>Feature Engineering</h3>

<ol>
    <li><strong>Handling Duplicate Rows:</strong> The dataset contains duplicate rows with different numbers of reviews. Clean the URLs to retain only the highest number of reviews for each unique URL. For example, clean the URL to https://www.zomato.com/bangalore/jalsa-banashankari and keep only the rows with the highest number of reviews for each unique URL.</li>
    <li><strong>Dealing with Restaurant Types and Cuisines:</strong>
        <ul>
            <li><strong>Separate Elements:</strong> Split elements in the rest_type, cuisines, and dish_liked columns into individual columns (e.g., rest_type_0, rest_type_1, etc.).</li>
            <li><strong>New Columns:</strong> Create new columns to represent the number of specializations:
                <ul>
                    <li>no_spec: Number of restaurant types per restaurant.</li>
                    <li>no_cuisines: Number of different cuisines per restaurant.</li>
                    <li>no_liked_dishes: Number of liked dishes per restaurant.</li>
                </ul>
            </li>
        </ul>
    </li>
    <li><strong>Handling menu_item and reviews_list:</strong>
        <ul>
            <li>menu_item: Create a new column to count the number of items in each restaurant's menu.</li>
            <li>reviews_list: Convert the reviews to a Python list of tuples and create a new column num_reviews to count the number of reviews per restaurant.</li>
        </ul>
    </li>
    <li><strong>Handling location:</strong> Use the Geopy module to get latitude and longitude based on location information. Prefix location names with 'Bangalore' to avoid matching issues and use these for future spatial analysis.</li>
</ol>

<h3>Final Steps for Encoding</h3>

<ol>
    <li><strong>Create a Cleaned Copy for Encoding:</strong> Make a copy of the cleaned dataset for encoding and further analysis.</li>
    <li><strong>Delete Irrelevant Columns:</strong> Remove columns that are not needed for analysis or machine learning:
        <ul>
            <li>url</li>
            <li>address</li>
            <li>name</li>
            <li>rate</li>
            <li>location</li>
            <li>rest_type</li>
            <li>dish_liked</li>
            <li>cuisines</li>
            <li>reviews_list</li>
            <li>listed_in(city)</li>
            <li>menu_item</li>
            <li>count</li>
        </ul>
    </li>
    <li><strong>Apply Binary Encoding:</strong> Apply binary encoding to:
        <ul>
            <li>online_order</li>
            <li>book_table</li>
            <li>is_new</li>
            <li>is_road</li>
        </ul>
    </li>
    <li><strong>Apply Target Encoding with Smoothing:</strong> Use Target Encoding with Smoothing for categorical columns:
        <ul>
            <li>rest_type_</li>
            <li>cuisine_</li>
            <li>dish_liked_</li>
        </ul>
        Sum each group into a single column for ease of use in models.
    </li>
    <li><strong>Remove Separated Columns:</strong> After summarizing encoded columns, remove the original separated columns to keep the dataset streamlined.</li>
</ol>

<h2>Exploratory Data Analysis</h2>

<h3>Top Restaurants in Terms of Number of Outlets</h3>
<p>The image below illustrates the top restaurants based on the number of outlets in the city:</p>
<img alt="Top Restaurants by Number of Outlets" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhiRzHiGDXArfuT5FZ6FoYFjI9giYIO7JwzDXWDDYwI8YSoX96elmOFF5viuJoqaCfbhSHTKsvRtXcD_0pdk2N6iXKbUcUR_aAV__U_D64K_nFHvyux2aYsKQAznSQfDi8bXdlWBvgE3CcyxtQKS_hSBOxpSdsTzQOQiju6USAYCRZJYrPo5CeGENhsfE8/s1600/download.png">

<h4>Key Findings:</h4>
<ul>
    <li><strong>Café Coffee Day:</strong> Leading with the highest number of outlets.</li>
    <li><strong>Domino's Pizza:</strong> A close second in terms of outlet numbers.</li>
    <li><strong>Five Star Chicken:</strong> Ranking third in the number of outlets.</li>
</ul>

<h3>Top Restaurants in Terms of Votes (Engagements)</h3>
<p>The image below shows the top restaurants based on votes, reflecting customer engagement:</p>
<img alt="Top Restaurants by Votes" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgblQaUPaMazyhBJRjeunC2jT2VSfaeufOob_BLfDtYhjg1jYD19uWdyw0a_-ty99XA05-NpTzuDwMQ5vMOaxZDvXi2k3wd0LETMgVege1ojDXWdab8XtyQXhkbs7tqdoUnkhxmaLjWT1Y8rFUNCcu2kZZ9cHpgbHqlq-FVVFxkpwT836c0u4fgRUu4ALM/s1600/download.png">

<h4>Key Insights:</h4>
<ul>
    <li><strong>Café Coffee Day:</strong> Despite having the highest number of outlets, it also shows strong customer engagement.</li>
    <li><strong>Byg Brewski Brewing Company:</strong> Stands out with significant customer engagement despite fewer outlets.</li>
    <li><strong>Toit:</strong> Known for high engagement with a focused strategy.</li>
    <li><strong>The Black Pearl:</strong> Successful in attracting customers with its niche offerings.</li>
</ul>

<h4>Market Implications:</h4>
<ul>
    <li><strong>Diverse Customer Preferences:</strong> Bangalore's market shows a range of customer preferences. Chains like Café Coffee Day cater to high-volume needs, while establishments like Byg Brewski and Toit offer specialized experiences with high engagement.</li>
    <li><strong>Strategic Focus and Engagement:</strong> Focused establishments with unique experiences achieve higher engagement. For example, Byg Brewski’s brewery setting and Toit’s brewery and dining experience contribute to their high votes.</li>
    <li><strong>Opportunities for Growth:</strong> Investors can explore expanding popular chains and investing in niche concepts with high engagement. Chains with many outlets should enhance customer experience, while specialized establishments might consider scaling up while maintaining their unique appeal.</li>
</ul>

<p>In summary, the Bangalore market features a dynamic blend of high-volume chains and niche establishments. Leveraging insights on customer preferences and engagement can guide strategic growth and investment decisions.</p>
<h2>Restaurant Types Analysis</h2>

<h3>Type Distribution</h3>
<p>The pie chart below shows the distribution of different restaurant types in Bangalore:</p>
<img alt="Type Distribution" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh14y1vVt84vHO0lyKPzA9R5jE6Lj7EoiJs106N9ydhduXAxSrVCYhwwVX5wvGckV67Zgt69hg9mAt_S24E7f0jZiu5AZU9aSSMTqagjfgLDHzHu4drlZcyKJ_VRdaqT124Quw9vjJGryZqGz9Us7fxHPEWOhaXeJqnnE8g2fdlzxHpAXp8VDRIOI-bCrc/s1600/download.png">

<h3>Top Performing Categories in Terms of Votes and Engagement</h3>
<p>The chart below highlights the top-performing restaurant categories based on votes and customer engagement:</p>
<img alt="Top Performing Categories" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg-quLlX0pE-HRTmea-14VeOweGE2LEBlLM0pGAbfMk9x8hAlVhaxyckKPl0kRqfLgwd6IVH9uRxZw3cWaxVx9IFU7K7mQgoza5vOsUfvmArpsoqFACx69s95IZcI17_ntz9TSb_inNB4TWJtKGBHw5MYdaDX9A44nZ28Co9EZiwD3RbOM9e16J4eCVfkk/s1600/download.png">

<h3>Characteristics Comparison by Category</h3>
<p>The radar chart below compares the characteristics of each restaurant type:</p>
<img alt="Characteristics Comparison by Category" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgwEwvUSXE3atBvfziSZ5JcyloNz4y9itkslK6Ft24PjPjpnffbYBFro8c3S6F-5FnQH6xl2d26ZkURgGNR5SXWS9jefeuIQQKy3I7O8Qy_abN3h7Cn2EYiY5e4eTvGXDjRZESkhpbC4-uO54ukc0EN1fN35F8qFOuhHPjZsVDrQOfKVgyTXE3_EBjIUjU/s1600/download.png">

<h4>Key Findings:</h4>
<ul>
    <li><strong>Type Distribution:</strong> Delivery (48%), Dine-out (39%), Desserts (8%).</li>
    <li><strong>Top Performing Categories:</strong>
        <ul>
            <li>Drinks &amp; Nightlife: Highest in engagement and ratings.</li>
            <li>Buffet and Pubs and Bars: Slightly lower but still notable in engagement and ratings.</li>
        </ul>
    </li>
    <li><strong>Lower Performing Categories:</strong>
        <ul>
            <li>Delivery, Dine-out, and Desserts: Show lower votes and ratings compared to other categories.</li>
        </ul>
    </li>
</ul>

<h4>Market Implications:</h4>
<ul>
    <li><strong>Customer Preferences:</strong> Drinks &amp; Nightlife venues are highly favored, indicating a preference for vibrant social experiences with entertainment and a lively atmosphere. High engagement suggests customers are willing to invest time and money in these experiences.</li>
    <li><strong>Delivery, Dine-out, and Desserts:</strong> These categories, despite being popular, show lower engagement and ratings. Improvements in service quality, food variety, or dining experiences could boost performance.</li>
    <li><strong>Opportunities:</strong>
        <ul>
            <li>Improving Delivery and Dine-out services through quality and uniqueness can enhance performance.</li>
            <li>Diversifying offerings by integrating successful elements from high-performing categories could improve overall appeal.</li>
        </ul>
    </li>
</ul>

<h4>Conclusion:</h4>
<p>The Bangalore market exhibits diverse preferences, with Drinks &amp; Nightlife experiences being highly valued. While there are opportunities to enhance Delivery, Dine-out, and Desserts offerings, focusing on quality and unique experiences can drive higher engagement and satisfaction. Investors should consider these insights for strategic growth and investment opportunities.</p>
<h2>Cost Analysis: The Impact of Booking Tables, Online Orders, and Location on Restaurant Pricing</h2>

<h3>Introduction</h3>
<p>The Indian restaurant and cafe market is characterized by diverse consumer preferences and business models. This analysis examines the influence of booking tables, online ordering, location, and customer feedback (ratings and votes) on pricing strategies within this sector.</p>

<h3>Key Insights</h3>

<h4>Booking Tables and Pricing</h4>
<p>Booking tables at restaurants shows a strong correlation with pricing. Establishments that offer table reservations tend to have higher price points. This is likely due to the premium experience associated with dine-in services, which includes not only the food but also the ambiance and personalized service. Consumers are often willing to pay more for the assurance of a reserved spot, especially in popular or high-demand venues.</p>

<h4>Online Orders and High-Cost Restaurants</h4>
<p>High-cost restaurants often do not offer online ordering services. This is primarily because the experience of dining in such establishments includes being physically present to enjoy the environment and service, which cannot be replicated through home delivery. Additionally, the logistical challenges and potential compromise on food quality during delivery deter high-end restaurants from offering online orders.</p>

<h4>Impact of Location</h4>
<p>Restaurants located on main roads generally exhibit higher pricing compared to those within residential areas. Being in a prime location allows these establishments to command higher prices due to increased visibility and accessibility. Moreover, such locations often attract a broader customer base, enabling them to cover a wider price range to cater to diverse economic segments.</p>

<h4>Votes and Ratings Influence</h4>
<p>While customer votes (the number of reviews) have a limited impact on pricing, ratings (the quality of reviews) significantly influence price levels. An increase in ratings from 3.5 to 4.3 is typically associated with higher prices, as it reflects consumer satisfaction and perceived value. However, beyond a rating of 4.3, prices tend to decrease. This trend suggests that to achieve exceptionally high ratings, restaurants might lower prices to enhance value perception and attract more customers, creating a balance between cost and quality.</p>

<h3>Conclusion</h3>
<p>The dynamics of the Indian restaurant market reveal that consumer preferences and business strategies are intricately linked. High-rated establishments often find themselves adjusting pricing to maintain quality and customer satisfaction. For investors, understanding these nuances can guide strategic decisions in the food service industry, emphasizing the importance of location, service offerings, and consumer engagement in determining pricing strategies.</p>

<h3>Recommendations for Investors</h3>
<ul>
    <li><strong>Focus on Location:</strong> Invest in restaurants with strategic locations that naturally attract more foot traffic and can justify higher pricing.</li>
    <li><strong>Enhance Customer Experience:</strong> Encourage businesses to offer table bookings to capitalize on consumers' willingness to pay for a guaranteed dining experience.</li>
    <li><strong>Balance Pricing and Quality:</strong> For high-rating targets, focus on maintaining quality and adjusting prices to stay competitive without compromising the customer experience.</li>
    <li><strong>Leverage Customer Feedback:</strong> Use ratings and reviews as critical data points for continuous improvement and strategic pricing adjustments.</li>
</ul>

<h3>Visualizations</h3>

<h4>Scatter Plot Analysis:</h4>
<p>The scatter plot below illustrates the relationship between cost, rating, booking table feature, being on the road, and online order feature:</p>
<img alt="Scatter Plot Analysis" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj1Y6Qrs3VFFhYkxnajq0mv27QyOnmVaTWmYdttfBNiTCFVdgmgCUuTTdumAVrMUDKvhW-9TK5NnyTZkeRlh36ny3h-3KtDT0okesyXOQKQzBcLduqvjbL3iG758zfCPINHNKEIh1g9HDVt7XSN04B5jLJggTxPhtKmOZJzGoPOFXIueA_Natwe4DlA0g8/s1600/download.png">

<h4>Box Plots Comparison:</h4>
<p>The group of box plots compares costs for booking tables, online orders, and being on the road:</p>
<img alt="Box Plots Comparison" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgTBlCldzBaIrwjU6xPeQMYYYDCgk54pTXcwjMWc1aiassyuJwu1muJt8lcoRBaz-b3XAMQ0akr7-8SEkoARDOlDRX7d8EMvmrqgPonGXARvyEf8uBARaYrYle7NYoCwOmPPREx-HQmPZq-bQnc3KTYiEcDASsvDQa0qpO_Lv-u2DT30nTChAQmFhpKG8g/s1600/download.png">
<h2>Location Analysis: Understanding Bangalore's Culinary Hotspots</h2>

<h3>Which is the Foodie Area?</h3>
<p>The map below highlights the concentration of dining establishments across Bangalore, showing the most popular foodie areas:</p>
<img alt="Foodie Areas in Bangalore" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiFy5mV4MKmt5Ry-UveTXuOITsnPd4ZF6IibgrB2UyE5OGVB3OlFOXhV91fGec7tiPXRnGIGl3IGTZ_BuR4CgtbM4qXagAmuZ3EwYgWC6LtqeR2jFyr_W84602TmY9D_q6we-8D7XPEkHBLu9FIsiwkQg2UYy-6mgq2e4TudnPQs2wvSqcS3nN0xfacIlo/s1600/download.png">

<h3>Characteristics of Location on Other Variables</h3>

<h4>Location vs Cost Chart (Sorted by Cost)</h4>
<p>The chart below illustrates the relationship between location and cost, sorted by cost:</p>
<img alt="Location vs Cost Chart" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh-9Uj9zUpwDrXOG-Ni-pf3iuXE7oTXotZG9woNcW5trP2m4zK6w68AUIJZR6Ip401WuRrlcKI6QfxtcbaK-4L10f1KzSB9BYGlbfx3rCUNIWiNmbdyC90j4tZFGhOcCthI3W3ouyiiItNwomM6h6vzjKfNum2PhJpvWJNcwLoDl6ZwNjhL4uo3cI75X78/s1600/download.png">

<h4>Location vs Votes Chart (Sorted by Votes)</h4>
<p>The chart below shows the relationship between location and votes, sorted by votes:</p>
<img alt="Location vs Votes Chart" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhDXIb3ItzxWMuIcxsVjkCO0gu4X9UTNbQkEEOqq83HeT_U3CKhiibkV0ygUgdVxyaoU7hUoSXng4zKc6JO2vN8GO7VHRDRui0Rx2-8NxScEynXAeydbTXUhu0OcV20zVUUhkYCTBRun5r-CpPJMRhlGVskJr7HD2oVBB95soud3MiDOc0DkCw2oUD0E6A/s1600/download.png">

<h4>Top Locations Characteristics</h4>
<p>The chart below highlights the characteristics of top locations in Bangalore:</p>
<img alt="Top Locations Characteristics" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgoyQsA4BaCPoXAhQ27t9rSNedlhVR__LIpeIxHaF7BbnEoImgdUDUv7sq6w5oN6c6BNDiRp3W7lsEtzekDPU2c4Ryh_o8ODnLTKFhHd7GtNcVNw3-s7IsgHS_d-cW1_29QFeIP7Juy8FgepPUW0Rpze1jDOTWHxTHBed88HUZ3UATWWn7CYHoJrPnGyV8/s1600/download.png">

<h3>Market Analysis</h3>

<p>Bangalore's dynamic culinary landscape offers various opportunities for strategic investment. By examining the distribution and characteristics of dining establishments across key neighborhoods, investors can make informed decisions.</p>

<h4>Centralized Nightlife Venues</h4>
<p><strong>Drinks &amp; Nightlife:</strong> Concentrated in the heart of Bangalore, these establishments cater to the city's vibrant, tech-savvy young professionals and expats seeking entertainment and social experiences. The central locations offer high visibility and access to a diverse clientele. Investment in these areas should focus on innovative concepts that combine local culture with international trends to attract a wide audience.</p>

<h4>Western Buffet Offerings</h4>
<p><strong>Buffet:</strong> Predominantly located on the western side of the city center, buffets appeal to families and groups. These venues should emphasize diverse culinary options and value for money to attract the surrounding residential communities. Expanding in these areas can capitalize on the demand for family-friendly dining experiences.</p>

<h4>Emerging Restaurant Hubs</h4>
<p><strong>Whitefield, Electronic City, BTM Layout, HSR Layout, Marathahalli:</strong> These neighborhoods account for nearly 30% of the city's restaurants, with Whitefield alone comprising 10%. Known for their vibrant youth culture and burgeoning tech industry, these areas are ideal for casual dining and quick-service restaurants. Investors should focus on creating hip, affordable venues that cater to students, young professionals, and tech workers.</p>

<h4>High-Spending Customer Zones</h4>
<p><strong>Sankey Road, Lavelle Road, Race Course Road, Infantry Road:</strong> These affluent areas attract customers with higher spending power, making them suitable for upscale dining establishments. Restaurants here should offer gourmet cuisine, exceptional service, and a premium ambiance to meet the expectations of discerning diners. Innovative and exclusive dining concepts will thrive in these high-value zones.</p>

<h4>Engagement-Driven Destinations</h4>
<p><strong>Rajarajeshwari Nagar, Lavelle Road, Church Street:</strong> Known for high engagement and vibrant atmospheres, these areas attract patrons seeking unique culinary experiences. Establishments should focus on creating interactive and memorable dining experiences, such as themed decor, live performances, or fusion menus that highlight both global and local flavors.</p>

<h3>Conclusion</h3>
<p>Bangalore's diverse neighborhoods offer varied opportunities for restaurant investments. By aligning restaurant concepts with the unique characteristics and customer profiles of each area, investors can optimize market reach and profitability. Understanding local consumer behavior, leveraging the city's tech-driven innovation, and maintaining cultural relevance will be key to successful ventures in this bustling metropolis.</p>
<h2>Restaurant Types</h2>

<h4>Chart: Most Common Restaurant Types</h4>
<img alt="Most Common Restaurant Types" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg3dxm4YK2fbzzPEHs520AAQmkamgwW-gmR3KRpDFJrEZwG1-D1ooeoXPyEy3xLdKp7DsTK8fNndnX5fXY0QRsuaDg5gOjgckgELo1CoFAwRWBGZSOiiQOyo_FjdponFMHVWaELhSRCz8DxnmdaMgu01oI74ccV-43q4C_MS9V4k2DhZNBvsEfK4RSWkPA/s1600/download.png">

<h4>Bar Chart: Relation Between Type, Ratings, Votes, and Scaled Number of Outlets</h4>
<img alt="Relation Between Type, Ratings, Votes, and Scaled Number of Outlets" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgt3QbEYY_W7c4dS2ig9CxIqvKOB-s2vcxghyphenhyphen3nJeUNpt-pGh_KUoO1ODtqr2wfYuTgQiUakBB9iJuZzLxItbFHXjTAv_PQpfQ88UvfsZ93x0HoFHRYKMNUl_A67veQumHB5m3tSwpehKOJhS2yrSosyjJRsSBoKIssyLBx3irarrYG3Z9v5jSu9j6gnBQ/s1600/download.png">

<h4>Radar Charts: Characteristics of Each Type</h4>
<img alt="Characteristics of Each Restaurant Type" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhyzpGzlLxgv9Q3h5n3_qOWMxOweSf1d4NSfwLs4U8A8P_4oib2WBmzlJRSTpH1KKrfvetzBl_QOL0QTaM5PTR4DpFqrJQdH5JY1EgzHXJDhSaNaSnlG4ifp9e3GicjKfYwfd7qqJoKaNvv3Q2BlDDFvOvlRb1GuIf5p67FrVDCgJC1S4isZxXsY8ZxXCE/s1600/download.png">

<h3>Specializations in the Food Sector</h3>
<p>Bangalore's food scene is vibrant and diverse, encompassing a wide range of dining options. The market is primarily divided into three main categories:</p>
<ul>
  <li><strong>Quick Bites (40%):</strong> This category includes fast-food outlets and quick-service restaurants. While it constitutes a significant portion of the market, it lacks strong customer engagement.</li>
  <li><strong>Casual Dining and Cafes:</strong> These segments together account for about two-thirds of the food market. Casual Dining and Cafes have higher customer engagement, suggesting that diners prefer a mix of convenience and a pleasant dining atmosphere.</li>
  <li><strong>Irani Cafes:</strong> These are currently trending due to their engaging atmosphere, reasonable pricing, and high ratings (up to 4.4). Irani Cafes offer unique dining experiences, filling a niche in the market with limited competition.</li>
</ul>

<h3>Investment Opportunities</h3>
<ul>
  <li><strong>Fine Dining:</strong> Although this sector is the most expensive and currently has limited customer interest, it presents an opportunity for experienced investors to develop exceptional dining experiences for high-end customers.</li>
  <li><strong>Drinks and Nightlife:</strong> Pubs, microbreweries, and clubs are popular among younger demographics and show strong demand. Investing in these venues can be lucrative due to their popularity and relatively good pricing.</li>
</ul>

<h3>Customer Types and Best Locations</h3>
<ul>
  <li><strong>Young Professionals and Millennials:</strong> This group favors microbreweries, pubs, and clubs. Ideal locations for these venues are busy areas with vibrant nightlife.</li>
  <li><strong>Families and Casual Diners:</strong> Families prefer Casual Dining and Cafes, which are best situated in suburban areas with a community-oriented vibe.</li>
  <li><strong>Wealthy and Special Occasion Diners:</strong> Fine Dining establishments cater to high-income individuals and special events. These should be located in upscale neighborhoods or near cultural landmarks.</li>
  <li><strong>Culture Lovers:</strong> Irani Cafes appeal to those interested in traditional and cultural dining experiences. These cafes perform well in historical areas that complement their cultural theme.</li>
</ul>

<h3>Restaurant Types Distribution</h3>
<p>Below is a table showing the distribution of various restaurant types across different locations in Bangalore. Each location is color-coded for clarity:</p>

<table border="1" cellpadding="5" cellspacing="0">
  <thead>
    <tr>
      <th>Location</th>
      <th>Restaurant Type</th>
      <th>Count</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Quick Bites</td>
      <td style="background-color: #FBB6B6;">385</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Casual Dining</td>
      <td style="background-color: #FBB6B6;">177</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Delivery</td>
      <td style="background-color: #FBB6B6;">117</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Cafe</td>
      <td style="background-color: #FBB6B6;">53</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Dessert Parlor</td>
      <td style="background-color: #FBB6B6;">45</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Food Court</td>
      <td style="background-color: #FBB6B6;">31</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Bakery</td>
      <td style="background-color: #FBB6B6;">27</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Bar</td>
      <td style="background-color: #FBB6B6;">26</td>
    </tr>
    <tr style="background-color: #FDE4E4;">
      <td>Yeshwantpur</td>
      <td>Sweet Shop</td>
      <td style="background-color: #FBB6B6;">15</td>
    </tr>
    <tr style="background-color: #e4e6fd;">
      <td>Wilson Garden</td>
      <td>Takeaway</td>
      <td style="background-color: #B6FBB6;">61</td>
    </tr>
    <tr style="background-color: #e4e6fd;">
      <td>Wilson Garden</td>
      <td>Kiosk</td>
      <td style="background-color: #B6FBB6;">9</td>
    </tr>
    <tr style="background-color: #e4e6fd;">
      <td>Wilson Garden</td>
      <td>Mess</td>
      <td style="background-color: #B6FBB6;">8</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Beverage Shop</td>
      <td style="background-color: #B6FBB6;">43</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Pub</td>
      <td style="background-color: #B6FBB6;">13</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Lounge</td>
      <td style="background-color: #B6FBB6;">8</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Microbrewery</td>
      <td style="background-color: #B6FBB6;">7</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Fine Dining</td>
      <td style="background-color: #B6FBB6;">5</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Confectionery</td>
      <td style="background-color: #B6FBB6;">3</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Dhaba</td>
      <td style="background-color: #B6FBB6;">2</td>
    </tr>
    <tr style="background-color: #E4FDE4;">
      <td>Whitefield</td>
      <td>Pop Up</td>
      <td style="background-color: #B6FBB6;">1</td>
    </tr>
    <tr style="background-color: #fafde4;">
      <td>West Bangalore</td>
      <td>Food Truck</td>
      <td style="background-color: #B6FBB6;">15</td>
    </tr>
    <tr style="background-color: #fdf4e4;">
      <td>Sankey Road</td>
      <td>Club</td>
      <td style="background-color: #B6FBB6;">1</td>
    </tr>
    <tr style="background-color: #f0fde4;">
      <td>Lavelle Road</td>
      <td>Irani Cafe</td>
      <td style="background-color: #f0fde4;">1</td>
    </tr>
    <tr style="background-color: #e4f0fd;">
      <td>Kalyan Nagar</td>
      <td>Meat Shop</td>
      <td style="background-color: #e4f0fd;">1</td>
    </tr>
    <tr style="background-color: #F0E4FD;">
      <td>ITPL Main Road, Whitefield</td>
      <td>Bhojanalya</td>
      <td style="background-color: #D6B6F5;">1</td>
    </tr>
  </tbody>
</table>

<h3>Location types Analysis</h3>
<ul>
  <li><strong>Yeshwantpur:</strong> Diverse and affordable, appealing to the middle class.</li>
  <li><strong>Wilson Garden:</strong> Budget-friendly and fast food, suited for economical diners.</li>
  <li><strong>Whitefield:</strong> Mid-to-high budget, attracting both upper-middle-class and lower-high-class individuals, with a focus on nightlife.</li>
  <li><strong>West Bangalore:</strong> Food trucks offering diverse options, drawing a broad demographic.</li>
  <li><strong>Sankey Road, Lavelle Road, Kalyan Nagar, ITPL Main Road:</strong> Specialized dining experiences catering to niche markets.</li>
</ul>
<h2>Dishes Analysis</h2>

<h3>Most Preferred Dishes by Restaurant Type</h3>
<p>Below is a table showcasing the most preferred dishes for each restaurant type, ranked from most to least popular:</p>

<table border="1" cellpadding="5" cellspacing="0">
  <thead>
    <tr>
      <th>Restaurant Type</th>
      <th>1st Preference</th>
      <th>2nd Preference</th>
      <th>3rd Preference</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Quick Bites</td>
      <td>Paratha</td>
      <td>Burgers</td>
      <td>Rolls</td>
    </tr>
    <tr>
      <td>Casual Dining</td>
      <td>Biryani</td>
      <td>Pasta</td>
      <td>Cocktails</td>
    </tr>
    <tr>
      <td>Delivery</td>
      <td>Paratha</td>
      <td>Biryani</td>
      <td>Chicken Biryani</td>
    </tr>
    <tr>
      <td>Cafe</td>
      <td>Pasta</td>
      <td>Burgers</td>
      <td>Coffee</td>
    </tr>
    <tr>
      <td>Dessert Parlor</td>
      <td>Waffles</td>
      <td>Coffee</td>
      <td>Hot Chocolate</td>
    </tr>
    <tr>
      <td>Food Court</td>
      <td>Burgers</td>
      <td>Noodles</td>
      <td>Pasta</td>
    </tr>
    <tr>
      <td>Bakery</td>
      <td>Sandwiches</td>
      <td>Coffee</td>
      <td>Chocolate Cake</td>
    </tr>
    <tr>
      <td>Bar</td>
      <td>Cocktails</td>
      <td>Beer</td>
      <td>Pizza</td>
    </tr>
    <tr>
      <td>Sweet Shop</td>
      <td>Chaat</td>
      <td>Samosa</td>
      <td>Rasmalai</td>
    </tr>
    <tr>
      <td>Takeaway</td>
      <td>Paratha</td>
      <td>Biryani</td>
      <td>Salad</td>
    </tr>
    <tr>
      <td>Kiosk</td>
      <td>Rolls</td>
      <td>Pasta</td>
      <td>Pav Bhaji</td>
    </tr>
    <tr>
      <td>Mess</td>
      <td>Chicken Biryani</td>
      <td>Chicken Fry</td>
      <td>Masala Prawn</td>
    </tr>
    <tr>
      <td>Beverage Shop</td>
      <td>Sandwiches</td>
      <td>Thick Shakes</td>
      <td>Faluda</td>
    </tr>
    <tr>
      <td>Pub</td>
      <td>Cocktails</td>
      <td>Beer</td>
      <td>Pizza</td>
    </tr>
    <tr>
      <td>Lounge</td>
      <td>Cocktails</td>
      <td>Nachos</td>
      <td>Beer</td>
    </tr>
    <tr>
      <td>Microbrewery</td>
      <td>Cocktails</td>
      <td>Craft Beer</td>
      <td>Pizza</td>
    </tr>
    <tr>
      <td>Fine Dining</td>
      <td>Salads</td>
      <td>Pasta</td>
      <td>Cocktails</td>
    </tr>
    <tr>
      <td>Dhaba</td>
      <td>Naan</td>
      <td>Rumali Roti</td>
      <td>-</td>
    </tr>
    <tr>
      <td>Food Truck</td>
      <td>Pizza</td>
      <td>Biryani</td>
      <td>Momos</td>
    </tr>
    <tr>
      <td>Club</td>
      <td>Cocktails</td>
      <td>Salads</td>
      <td>Biryani</td>
    </tr>
    <tr>
      <td>Irani Cafe</td>
      <td>Okra</td>
      <td>Pancakes</td>
      <td>Cocktails</td>
    </tr>
  </tbody>
</table>

<h3>Cuisine Analysis</h3>

<p>The following bar charts and radar charts provide insights into the market dynamics of various cuisines in Bangalore:</p>

<h4>1. Cumulative Share of Each Cuisine</h4>
<img alt="Cumulative Share of Each Cuisine" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg3e7d15Xevycfq8mmTlEZuEFkkbz6rGoVt1fTM3C3K_nkrhBpMgTLiosCdAXm9ntDoojxyqTvSvl4s1J0NPcNajAisS9ksgEyxc_HRfVWaCpeBEadOMyvOEeh4556OpqeNv3_M6pN_sT_QP9XQ7T3YaiAYzq1DlZ8F-NdNQXAHg9nMb5n99LF2_meVagk/s1600/download.png">

<h4>2. Relationship Between Cuisines and Rating, Votes, and Cost (Sorted by Cost)</h4>
<img alt="Relationship Between Cuisines and Rating, Votes, and Cost (Sorted by Cost)" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjMXmxOWSVmkEgdjqbbWp9mEF8f6bzcgBu8LDUe78VQrchjd-RyhPWvSJjTlxR-tWbinZJer9L3Q14hSoPoPCi4kMJdZTQ3W3fiJ4o0qWg6tJlgANHIeNCP8nr5_FGhZ1MENaUyOovx9F1icwPUBcilXq_DiV64uoCJW8sV-0e4JhRnBauXu6pwpL68h9g/s1600/download.png">

<h4>3. Relationship Between Cuisines and Rating, Votes, and Cost (Sorted by Votes)</h4>
<img alt="Relationship Between Cuisines and Rating, Votes, and Cost (Sorted by Votes)" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgXgVwCXO8dTfFyet-d2CHXqAIuqHMSaAMJUpJxyWn7wiK3hSz5ovkO90yuEPJumBYo891FDkcRA3NmPhHed3OF3Y9plmrNKVzaXj5Y3LYcshwtuwAjViEqfWeBoF0K0HJyss9v5ukZHH2K3FDKlhQ8wdRVjNDzZVwvjuAUE7ARDZsMhtSCLUFRJWpuWPk/s1600/download.png">

<h4>4. Characteristics of Each Cuisine (Radar Chart)</h4>
<img alt="Characteristics of Each Cuisine (Radar Chart)" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhEUrSIFnvvnPHCf8STfkScaXZUBTP9gNSvDPnOCIZsa5Yq8TpEtbT0NM7Q66C0g-sIZiH82Tu0Nzq12kj3p8fxQgh3o0-ZwbeF-cenQ0BDQ7P3kF8SftS4lPC2qhbhJ72Ip8fA4Z4Q8DZXrghuFUYUGQTMx-nP60djhJALNkR3crrO9URqv_RidjZcVY8/s1600/download.png">

<p>This analysis examines the market dynamics of various cuisines in Bangalore, focusing on engagement levels, pricing strategies, and investment potential. Bangalore's cosmopolitan nature creates a diverse culinary landscape, offering opportunities for both local and foreign cuisines to thrive.</p>

<h4>Cantonese Cuisine</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Engagement:</strong> High</li>
  <li><strong>Pricing:</strong> Premium</li>
  <li><strong>Target Audience:</strong> Affluent individuals seeking exclusive dining experiences.</li>
  <li><strong>Profitability:</strong> Significant due to high pricing, but the customer base is niche.</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> Invest in Cantonese cuisine by emphasizing targeted marketing and exclusive dining experiences. The high price point limits the customer base but ensures high returns per customer.</li>
  <li><strong>Explanation:</strong> High engagement despite premium pricing indicates strong demand among affluent consumers who value authentic experiences. This niche market can be highly profitable but requires targeted strategies to attract and retain customers.</li>
</ul>

<h4>German Cuisine</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Engagement:</strong> High</li>
  <li><strong>Spreading:</strong> Low</li>
  <li><strong>Pricing:</strong> Lower than Cantonese</li>
  <li><strong>Target Audience:</strong> Middle-income groups looking for authentic yet affordable experiences.</li>
  <li><strong>Profitability:</strong> Balanced between exclusivity and mass appeal.</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> Focus on providing authentic experiences at competitive prices to attract a broad demographic.</li>
  <li><strong>Explanation:</strong> German cuisine’s lower price point and moderate engagement suggest it is accessible to a larger audience compared to high-end options. This balance can attract middle-income groups while maintaining profitability.</li>
</ul>

<h4>Sri Lankan, Parsi, and Russian Cuisines</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Engagement:</strong> High</li>
  <li><strong>Spreading:</strong> Low</li>
  <li><strong>Pricing:</strong> Medium</li>
  <li><strong>Target Audience:</strong> Diners interested in cultural diversity and unique flavors.</li>
  <li><strong>Profitability:</strong> Steady returns with a focus on authenticity and distinctive experiences.</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> Emphasize cultural authenticity and unique offerings to maintain high engagement.</li>
  <li><strong>Explanation:</strong> Medium pricing combined with high engagement indicates a strong interest in diverse culinary experiences. By highlighting authenticity and unique flavors, these cuisines can sustain their appeal and provide steady returns.</li>
</ul>

<h4>Singaporean Cuisine</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Engagement:</strong> Growing</li>
  <li><strong>Spreading:</strong> Low</li>
  <li><strong>Pricing:</strong> Moderate</li>
  <li><strong>Target Audience:</strong> Indian audiences interested in diverse culinary experiences.</li>
  <li><strong>Profitability:</strong> Promising, with increasing appeal due to unique flavor profiles and fusion influences.</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> Leverage strategic marketing, including culinary festivals and pop-up events, to enhance visibility and engagement.</li>
  <li><strong>Explanation:</strong> Singaporean cuisine's emerging popularity aligns with growing interest in diverse food options. Strategic marketing and events can capitalize on this trend and boost engagement.</li>
</ul>

<h4>Foreign vs. Local Cuisines</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Foreign Cuisines:</strong> Generally attract high engagement and can command premium pricing. There is strong market openness to international flavors.</li>
  <li><strong>Local Cuisines:</strong> Despite comprising 30% of the restaurant market, face saturation and reduced engagement. Consumers seek novelty.</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> For local cuisines, focus on innovative approaches such as new regional specialties or fusion dishes.</li>
  <li><strong>Explanation:</strong> The saturation of local cuisines like Northern and Southern Indian reduces consumer engagement. Introducing novel options can rejuvenate interest and offer a competitive edge.</li>
</ul>

<h4>Chinese Cuisine</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Engagement:</strong> Low</li>
  <li><strong>Spreading:</strong> High</li>
  <li><strong>Pricing:</strong> Variable, often affordable</li>
  <li><strong>Target Audience:</strong> Wide-ranging, with a taste for fusion flavors.</li>
  <li><strong>Popularity:</strong> Ranks second to Northern Indian cuisine.</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> Continue investing in Chinese cuisine by leveraging its established popularity and introducing innovative dishes.</li>
  <li><strong>Explanation:</strong> The strong market presence and adaptability of Chinese cuisine, coupled with its affordability, contribute to its sustained popularity. Innovative offerings can further enhance its market position.</li>
</ul>

<h4>African Cuisine</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Engagement:</strong> Low but with potential for growth</li>
  <li><strong>Spreading:</strong> Low</li>
  <li><strong>Pricing:</strong> Variable</li>
  <li><strong>Target Audience:</strong> Health-conscious and adventurous diners.</li>
  <li><strong>Profitability:</strong> High potential due to low competition; aligning with current health trends.</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> Develop a robust marketing strategy focusing on cultural festivals and events to increase engagement and build a loyal customer base.</li>
  <li><strong>Explanation:</strong> Despite currently low engagement, African cuisine's rich flavors and health-oriented offerings align with consumer trends towards diverse and healthy eating. Effective marketing can tap into this potential.</li>
</ul>

<h4>Local Cuisines: Northern and Southern Indian</h4>
<p><strong>Analysis:</strong></p>
<ul>
  <li><strong>Market Share:</strong> 30% of restaurants</li>
  <li><strong>Competition:</strong> High</li>
  <li><strong>Engagement:</strong> Reduced due to saturation</li>
</ul>
<p><strong>Recommendation:</strong></p>
<ul>
  <li><strong>Investment Strategy:</strong> Innovate within local cuisines by introducing new regional specialties or fusion dishes.</li>
  <li><strong>Explanation:</strong> The high level of competition and saturation in local cuisines necessitates differentiation. Innovation is key to capturing consumer interest and staying relevant in the market.</li>
</ul>

<h4>Journal Article Insights</h4>
<p><strong>Study:</strong></p>
<ul>
  <li><strong>Title:</strong> "Restaurants in Little India, Singapore: A Study of Spatial Organization and Pragmatic Cultural Change"</li>
  <li><strong>Findings:</strong> Offers insights into how restaurants adapt to cultural changes and spatial organization.</li>
</ul>
<p><strong>Application:</strong></p>
<ul>
  <li><strong>Strategy:</strong> Apply insights to organize and position restaurants in Bangalore effectively. Understanding spatial and cultural adaptations will enhance the effectiveness of foreign cuisine offerings.</li>
  <li><strong>Explanation:</strong> Adapting restaurant setups based on cultural and spatial insights can improve market positioning and customer appeal.</li>
</ul>

<h2>Conclusion</h2>
<p>Bangalore's diverse food scene presents substantial investment opportunities in both foreign and local cuisines. While foreign cuisines like Cantonese, German, Singaporean, and African offer promising prospects due to their unique appeal and engagement, local cuisines require innovative approaches to capture consumer interest in a saturated market. Strategic investments in marketing and unique culinary experiences are crucial for success.</p>
<h2>Classification Analysis of Restaurants</h2>

<p>This analysis aims to classify restaurants into distinct categories: Low, Mid, Upper Mid, Lower High, and High Class, using unsupervised machine learning techniques. K-Means clustering was applied, and Principal Component Analysis (PCA) was utilized for 2D visualization of the clusters. The features used for clustering include: 'book_table', 'dish_liked', 'rest_type', 'cuisines', 'votes', and 'approx_cost(for two people)'.</p>

<h3>K-Means Clustering</h3>

<p>K-Means clustering was employed to group restaurants into five distinct clusters. The choice of cluster configuration was tested to ensure the desired results were achieved. The following line plot illustrates the progression of the clustering process and the final results:</p>

<img alt="K-Means Clustering Line Plot" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjG1yhOQU3rN4iMhsoOtApDTbdR2MAFZYg0TvDksvil_OEnuvGkMB5hcBiHaGaY3y1fnk4AkISFh77xOvS1JvmNOIxzB6SLAmjIM-aGHj0xD0nHhKKWuHU0MalLMM793jox5vmUjppr2dQkIadXLuHLf066ZvTUt9W7991T4VrF_4RDwZW5kv6sgnk37-w/s1600/download.png">

<h3>Cluster Validation</h3>

<p>To confirm the clustering results, a scatter plot was used to visualize the proximity of clusters in a 2D space:</p>

<img alt="K-Means Clustering Scatter Plot" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhPFYzvXu41es0-TswhyphenhyphenDvj2GfUZ78umxrbT1CuLj7-s7Gl6uVVmq5T5ZTsXcR8BRF_DvHD9v2XkH2DW0zPglgHXKBw5_zItdDNwqmiGn7IUlld2FZhiKVTRM_2l9AZaTHDzZl19G4IhMRgOI2bSzS6HbWZcrw2jst6nCpz7rNU0Vu0OsTGcEQ3z_IVJkk/s1600/download.png">

<p>Principal Component Analysis (PCA) was utilized to reduce the dimensionality of the data and visualize the clusters in a 2D plane. The following plot shows the clusters in the PCA-reduced space:</p>

<img alt="PCA Visualization of Clusters" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgB3-mBRWYYHvMYC6w8rVQAohVwb0iHCjcj6PLtWVTzBuCxzMQLr-w1trte_YM9V1k1bTB7dCLZ_nM9YkKM811z6_HcQX1yocrivus6uPXrctPITnySV8inY7BSaBqbq49lLbyLPqhErHbd0Q-G5RL4ss4iIhy38yX4F9I0X8zL8f0_OddYZsyhcb7tQ-g/s1600/download.png">

<h3>Cluster Quality</h3>

<p>The silhouette score test was performed to assess the quality of the clusters. The results indicate the cohesiveness and separation of the clusters:</p>

<img alt="Silhouette Score Plot" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEga_yHruhJyr-GmPUqzkCmWSw0tGpGvkpEtNauF_1lyeu6Erc5bj4Ur6GtW-gdhSfD098o_A99QVngNfHG77KWMvmWPNpCOfecGvEDTjccsnNUfF53wieHCcVC_CIAXlqHZKFOicnVYkwsfIxRZ_DveyZRp_L2-qShgcih_dShcr_N2QemwyTXmf2_oBQI/s1600/download.png">

<h3>Characteristics of Clusters</h3>

<p>Radar charts were used to visualize the characteristics of each cluster, providing insights into their distinct attributes:</p>

<img alt="Radar Charts of Cluster Characteristics" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgRGZnqRxzojoFxranA-SZJyVbT30gLHyxh4R0da99VarZPLvzddG20YlyD45YyQVUVJGQU8KbGIbhY5SfnLLcJlTsbZjkdWIGsBUCszjwgedNkITk0cAaCx4qWyOlT0D7cEZsvs61DGc8uef1StEv1cc2xT0gREksfnwYyd0Ccnjsl2eL1Uj2ILw-89w0/s1600/download.png">

<h4>Summary of Findings:</h4>

<ul>
    <li><strong>Low Class:</strong> Characterized by high traffic and spreading across the city. These restaurants offer balanced online order features, very low variety in specialization and dishes (cuisines), low pricing, and low ratings. They do not offer table booking.</li>
    <li><strong>Mid Class:</strong> Exhibits balanced traffic, high online order capabilities, above-average variety in dishes, but low variety in specializations. Pricing is higher than the Low Class but still low. These restaurants have low ratings and do not offer table booking.</li>
    <li><strong>Upper Mid Class:</strong> Shows high traffic and engagement but very low variety in specialization, high variety in dishes, average pricing, and rating. These restaurants offer table booking.</li>
    <li><strong>Lower High Class:</strong> Characterized by low traffic but very high engagement. They have average variety in specializations, high variety in dishes, above-average pricing, high ratings, and average table booking with low online orders.</li>
    <li><strong>High Class:</strong> Features very low traffic and low engagement, no online order capabilities, above-average table booking, average rating, very expensive pricing, high variety in dishes, and high variety in specialization.</li>
</ul>

<p>Overall, the analysis provides a comprehensive classification of restaurants, allowing for targeted marketing strategies and investment decisions based on the restaurant's class.</p>
<h2>Customer Behavior Analysis with Review Aspect Sentiment Analysis</h2>

<h3>Overview</h3>
<p>
    In analyzing customer behavior in Bengaluru's restaurant industry, our findings reveal that the number of reviews is skewed toward higher-end establishments, which is expected since budget restaurants typically prioritize affordability over experience and quality. To accurately compare customer sentiments across different restaurant categories, it's essential to set a clear price range that defines each class.
</p>
<p>
    Interestingly, there's a noticeable drop in the number of reviews in the range of approximately 1,500 to 2,300 reviews. This unusual pattern warrants further investigation to understand its underlying causes.
</p>
<p>
    Additionally, word cloud analysis shows that the overall experience is as crucial as the food itself, sometimes even more so, particularly in higher-end establishments. However, it's important to note that these conclusions are primarily relevant to higher-class restaurants due to the bias in the data toward these types of establishments.
</p>

<h3>Tools and Techniques</h3>
<p>
    For this analysis, I used <strong>SpaCy</strong> and <strong>NLTK</strong> to balance speed with accuracy, enabling a swift but reliable sentiment analysis of the review data.
</p>

<h3>Price Range and Review Distribution</h3>
<p>
    I visualized the relationship between the number of reviews and the number of restaurants for each price point using a line chart with a confidence interval.
</p>
<img alt="Price Range and Review Distribution" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj8uAFHr_jlQAXq512gwlN_SSVleOgrWL9FJ_EIU1qX20q98UsW1Fr9JIAo3MWTO1TpoQmlG5_Z2CS_-EYWGpx6NadvXvjoQr2Hn0mKyQjkwc7QIggYJS-cYiry8QrarUpY24JPMnIxofqmffQNbrAUv-dikk2fQTfu_XlzX-EQhiH1zLQ80Vvt6eKSRNk/s1600/download.png">

<h3>Word Cloud Analysis: Most Repeated Nouns in Reviews</h3>
<p>
    An analysis of the most repeated nouns in reviews was conducted and visualized using a word cloud. This analysis helps to understand what aspects customers focus on the most in their reviews.
</p>
<img alt="Word Cloud of Most Repeated Nouns in Reviews" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEigts0ZQ5vcR2132j0DyHeWSIMPxpJDkFKrPRj8F8FyXLdccOQ_XUwkS0MnSPx3IzVL1lev2in6bWhLmhSlRCWn9gkoQonGgAKx3q0QfQYrqOrwRVubC2jH8nO4H5xZbVJbc5lLwCHcTxRgsnxM4TAP-kofJ50StxfYLTDakIVtwy8xMzNc07CwFSnAeLU/s1600/download.png">

<h3>Price Range Analysis: 1,700–2,300 INR</h3>
<p>
    Over 90% of the classes in this price range cater to Mid, Upper-Mid, and High-Class groups. However, the engagement and ratings are lower because the area is equally divided between High-class and Mid-class residents. This makes it challenging to meet both groups' expectations in terms of quality and budget.
</p>
<p><strong>What classes fall in this price range?</strong> The following pie chart illustrates the distribution of different classes within this price range.</p>
<img alt="Class Distribution in Price Range 1,700-2,300 INR" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgVnBXHUI52wdmSZAKFlwNI-NSMANgWfO21yBTl5i2jeyHn2SS8dDtgkaWDWjOLh1q-EcAwXz20oOGymDgha3jhW9Zt6Ndi8rRjCdRgbpFKjHGb2hWn3hd9FnRJQruXDJabqdlXN1KGp-4ybgySqxbhpaQuIkNRdjytCqTXnib6qsMT_bi776ZlVTxx9Is/s1600/download.png">

<h3>Analysis of Restaurant Types and Pricing for 1,700–2,300 price range</h3>
<p>
    The following analysis explores the frequency of each type of restaurant within each class and the average price for High and Mid-Class establishments. This analysis helps to identify which types of establishments are most prevalent in this price range and how their pricing strategies differ.
</p>
<img alt="Frequency and Pricing of Restaurant Types in 1,700-2,300 INR Range" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgkIbunu6WMOAtMS7esLqXLhWDeUg9yR4zqg56IgJewNvpp91zycKHrMYd8TvK3WoRtgzWv4RgC_zLgD0MxUTVvo3EBXtWeKJUKH131uB7gRmRv2KprF4XXt6kXQz9CrP22HORnAYhCE1QByZ83glcLMol2dwKPs3S0GgrHU5VPQentetqKiSHV_iEvfZI/s1600/download.png">

<p>High class has the highest share in this price range, with Dine-out being the most common type among all categories.</p>

<h3>Average Price Analysis for all Classes Types</h3>
<p>Now, let’s look at the average price for Classes types in this range.</p>
<img alt="Average Price for High and Mid-Class Types" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgELbchS4R9dRceEuuDFtQDRnoc_rgHAwl1GkN5lKBDH2w8YtgJ0O3k8ScnO69FNQWbRuLW5NhLRCzRFv1wZfOa9Y1cCrg2HJnUZThtVnTrJ81i7u-P0Sxylxktq5YWsLYeyz3Tz3Jl39dgStkZWXjLaRFomlxUqxycCXZBDQu-Lqoj7KMOyH9wQkVBhZQ/s1600/download.png">
<img alt="Average Price Comparison for High and Mid-Class Types" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEizfUSREMacyMkrDZApKgKOXChY8-e2IDbn-WnRMxUnmhgiT4mpehhXAq032aKcOz-I41YfM8xGuY9Tw65IZQgG9vnTuyhgVWxXDPYeZzzQyWVTn-Jsrd101hHuiMVEEWtApCEa31UGo0iUD05HdMUVeyo1QbY1_cQE0Q-YHvX6krbItiX_qDCRC-HKSSw/s1600/download.png">

<h3>Review Analysis by Class in this range 1,700–2,300</h3>
<p>
    Next, we analyze the reviews to understand customer opinions on ambiance, service, food quality, price, special features, and cleanliness for each type in this class.
</p>
<h4>For High-Class</h4>
<img alt="Radar Chart for High-Class" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjozbczX7A0UFfITXpOvGAXPxZfOWyeHuZCIs8n4oeVwYLZMwpfpE0ZRxLZqH9S8w0ITd8B8i7t5L2_JYP-gPRXi-307VuLVv4vS0FPAP2KBFjC0KQgoS0qT7JkYjSs17IjeEUY9fIZfaYb9jyIrDTJ48WXu_CltLzV4UcsL-WGxmwe6r5eIxcM5_U1WSo/s1600/download.png">

<h4>For Lower-High Class</h4>

<img alt="Radar Chart for Lower-High Class" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiDF8m4v2rPSIue8coZ0TYe3boifJ8wNFb-g3FhSYLt6qwwwOtkJ8RgnwoBCERkD4dQEbbrIm1c_M-NCQbqzdyARJ6io8M7bUC-dmrk2heY5YpuwB2CpgCKHpw0Uf5S77mjLopfaXYQqXT-jQhwlwSJX60v918GgIiQ1zY-TZliED_rxyABkOI0E_tDuAw/s1600/download.png">

<h4>For Mid-Class</h4>

<img alt="Radar Chart for Mid-Class" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhvsRP34kq73Wph4QNV2D87dd-BcJ2O2pwgS3MzLVKLvC626WzQ4BzwVVnSmbY8Uo7NSN2WmnrdJ51UatoKeO4IFD9_gH7cvqjMiXtYBwuv9BHNWkbwmkmUKwR9eL2WrfBLm0f0diAfbiDRxRALFLuvt9RTmvA5vIxZhuxxRIOOCRepw72Nn7xY-jJQkMk/s1600/download.png">

<h4>For Lower-Mid Class</h4>

<img alt="Radar Chart for Lower-Mid Class" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjK6sPhtv98vat_6k7JV0LNy0cB4fsZpqyyvTIdLkihTmGM6rCbKjTCZuSs7XkyDCdOltepCnruXDyys_NitTdISmjjt5S_gKJ0HYSSbodoGx3HizWNmKUuOeMGIplVJf35ySiiMUpGQ6Qf3DqrQDF2fEseeLIi7tgcmNen5mEOn3rn6OUrRGZaGNMOn9E/s1600/download.png">
<p>The review analysis presented here should be viewed with caution due to inherent biases. The data is skewed towards specific customer segments, as not everyone chooses to leave reviews. Additionally, the analysis prioritized speed over accuracy, making it a useful starting point but not a comprehensive assessment of all review data.</p>

<h3>Price Range Analysis (1500-2300 INR):</h3>
<p>In the 1500-2300 INR price range, we've identified that this segment spans multiple customer classes, creating challenges in meeting diverse expectations. If restaurants focus on enhancing food quality and the overall experience to satisfy higher-end customers, prices might become unsatisfactory for lower-end customers, and vice versa.</p>

<p>However, establishments within this price range that cater to the lower-high class, particularly in categories like Dine-out, Drinks &amp; Nightlife, and Pubs and Bars, tend to perform better. Despite this, overall review sentiment remains less positive compared to other segments, highlighting the difficulty of catering to a diverse customer base within this range.</p>

<h3>Recommendations:</h3>
<p>For investors targeting this price range, it is essential to carefully select the location and decor to align with the desired customer class. Additionally, the marketing team should intensify efforts to effectively target the right customer segment.</p>
<h3>What are Reviews Insights About Each Class on All Price Ranges?</h3>

<p>The radar chart below shows the aspect sentiment analysis for each class:</p>

<h4>Higher Class</h4>
<p><img alt="Higher Class Radar Chart" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj2yH4zzrixDeJr4mOCwztFN0u6aucxWGCJJ4hJ2MQSLSmjlhXE9HUjv5e27a_3zR0sHLNwx5PIZ3Ag3DftMdG3GmRGiHt9XeqFO3zE4s2fRI2IQ0FZCz9OzvFr84BFCTzok_aRME707BsL9EUSod4TENMhhamxJbEgI49qaHBqxcLBr8sdd63GgPG0oNA/s1600/download.png"></p>

<h4>Lower-High Class</h4>
<p><img alt="Lower-High Class Radar Chart" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgDKhTrnm1KRhbGHnd3TVxuKdAwpT4bV_KTQDS0O-pgjQRi1u4cQgOvtXiv2Vg0o69mQ6JmRhcUONqXXBCr_UL-yPUw5-GuAUCG6tj4vw_ElQtdZ8ncSM-DvgF7czResy4Y_j5JzEjA7dFUHCVCk3R12PVsMCk0plo_65IMIDps19eKcvwwaP3QG5Fu0j8/s1600/download.png"></p>

<h4>Upper-Mid Class</h4>
<p><img alt="Upper-Mid Class Radar Chart" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj192XNw-1kjToUPaXfq1wCb_t8iUpi8sdC3GyxGekw5TC4sBXmXZmQrqepStRO0k5yQ68orZp7fpntHxO7YpclF068TDgeu1iNtz3eMrFqA0J4Jp0Odc-3Qs5zMCp4E0XJKGm-cNZfI6pl26t0iumf-m-Sf_u7X-nC6kXmpZF1l_7hl52TfZcofTuiSSc/s1600/download.png"></p>

<h4>Middle Class</h4>
<p><img alt="Middle Class Radar Chart" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjbn6lfLUBOG6lZlRC_n8nXJgE5kUIT8LppZmW42m-ckGJbHFe9-w5YV6p6WpKQXmzcwgf4c6p5RNfwiuFbj3p-Ut7kwvuacEchv-66fMX3mREBfEHk5oKnjctNWyNKmBKsxyvMjL6TKN2V6_T4cFYemxhK9uR-7lNJSAklJwMhTOloyPnHV6m_d4ksjmU/s1600/download.png"></p>

<h4>Lower Class</h4>
<p><img alt="Lower Class Radar Chart" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgw0DMj5higLTKO1pH6mYhmHbN6nn0ZGbHOTuNrKbGgCY2jdNBcNd-85grt_SiiSDikZpx0GzG3weDiqezkqVFqUS7zkYUPHFlfW2DTnz_XpWk6uF1XA52YQ_vqWJH_dS1RzYg5bIho6MDqyltNmvrA4XJzJzNJxy377SkYjdsunnVWBSxhqc_GYanmMQo/s1600/download.png"></p>

<h3>Analysis of Customer Satisfaction by Class and Type</h3>

<h4>High Class:</h4>
<p>For the high class, there is a noticeable similarity in customer satisfaction across Delivery, Cafes, and Drinks &amp; Nightlife categories. This similarity might be due to the convenience and premium experience these options offer, catering well to the preferences of this segment. However, Buffet services stand out with higher satisfaction levels compared to other types, possibly because they offer a variety of options that appeal to this class. On the other hand, Dine-out experiences show poor satisfaction, particularly regarding pricing, likely because the high prices may not align with the perceived value for this class.</p>

<h4>Recommendations for Investors:</h4>
<p>For investors targeting the high class, focusing on enhancing the buffet experience could be promising. It’s also advisable to reconsider pricing strategies for Dine-out services to better meet the expectations of this segment.</p>

<h4>Lower-High Class:</h4>
<p>In the lower-high class, there is a similarity in satisfaction levels across Dine-out, Pubs &amp; Bars, and Drinks &amp; Nightlife categories, but all of these show lower satisfaction regarding pricing. This may be because the pricing in these categories doesn't match the perceived value for this group. Desserts also show poor satisfaction, indicating a potential area for improvement.</p>

<h4>Recommendations for Investors:</h4>
<p>Investors could focus on improving pricing strategies, food quality, special features, and cleanliness in Dessert offerings. Additionally, enhancing the Buffet experience with better pricing and cleanliness could attract this class.</p>

<h4>Upper-Mid Class:</h4>
<p>The upper-mid class shows similarities in satisfaction across Delivery, Cafes, and Dine-out categories, with generally acceptable satisfaction except for pricing. However, Desserts and Drinks &amp; Nightlife categories show poor satisfaction, particularly regarding pricing and cleanliness. The best satisfaction levels are seen in Pubs &amp; Bars and Buffets.</p>

<h4>Recommendations for Investors:</h4>
<p>For this segment, maintaining the high standards in Pubs &amp; Bars and Buffets is key. Meanwhile, improving pricing and cleanliness in Desserts and Drinks &amp; Nightlife could yield better satisfaction.</p>

<h4>Mid Class:</h4>
<p>The mid class displays poor satisfaction in Drinks &amp; Nightlife and medium satisfaction in Pubs &amp; Bars. In contrast, Buffets receive high satisfaction, but cleanliness is a concern. For Drinks &amp; Nightlife and Pubs &amp; Bars, satisfaction with food quality, services, and special features is moderate, suggesting areas for potential improvement.</p>

<h4>Recommendations for Investors:</h4>
<p>Investors should focus on improving cleanliness in Buffets and enhancing the overall experience in Drinks &amp; Nightlife and Pubs &amp; Bars, particularly in food quality and special features.</p>

<h4>Low Class:</h4>
<p>The low class has the least number of reviews, but the analysis shows significant satisfaction in Delivery, Desserts, Dine-out, Cafes, and Buffets. However, Buffet pricing shows very poor satisfaction, and Dessert pricing has only medium satisfaction. Overall, there is low satisfaction with Desserts across all aspects, and Drinks &amp; similar venues show medium to poor satisfaction with pricing across all classes.</p>

<h4>Recommendations for Investors:</h4>
<p>For the low class, investors should focus on addressing pricing concerns in Buffets and Drinks with all types and improving the overall Dessert experience, including pricing and quality. These could be potential areas for gaining a competitive advantage.</p>
<h2>Prediction of Price Using Machine Learning</h2>

<p>In this section, we explore different machine learning models to predict restaurant prices. The process involves several steps, including data preparation, model selection, and performance evaluation.</p>

<h3>Data Preparation</h3>

<ol>
    <li><strong>Data Cleaning:</strong>
        <ul>
            <li>Removed columns: url, address, name, rest_type, dish_liked, cuisines, reviews_list, review_sentiment_list, menu_item.</li>
            <li>Applied binary encoding to columns: online_order, book_table, is_new, is_road.</li>
          <li>Appplying Ordinal Encoding for Classes</li>
          <li>Remove highest resturant in cost because it is outlier and effect the model negatively</li>
            <li>Split the data into training and test sets to prevent target encoding leakage.</li>
        </ul>
    </li>
    <li><strong>Target Encoding:</strong>
        <ul>
            <li>Applied target encoding to categorical features: rest_type_0, rest_type_1, cuisines_0, cuisines_1, cuisines_2, cuisines_3, cuisines_4, cuisines_5, cuisines_6, cuisines_7, dish_liked_0, dish_liked_1, dish_liked_2, dish_liked_3, dish_liked_4, dish_liked_5, dish_liked_6, listed_in(type), listed_in(city), location.</li>
            <li>Summarized each group of columns into single columns and created a feature map to replace values in the test set.</li>
        </ul>
    </li>
    <li><strong>Correlation Analysis:</strong>
        <ul>
            <li>Reviewed heatmap for correlation between features.</li>
        </ul>
        <img alt="Heatmap" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiZ6UmB3-gZzh9r9wuoy_IMV0qPSXUmKTs9jUdT3HgaVntJWSdsixqucrLQ0S55ZAHI7jSwIdNFFpLZKC0mHsmOG2d6nkCnCnqZ6Iw5Vc1v073q63X_g14NWlSZ5u3OMGNq6k3wLQoayKXObrJYfX3eoEEzdP0Kjv5An_Zt8Y4TqQ37ixGDOGunOjCW2Hk/s1600/download.png">
    </li>
    <li><strong>Variance Inflation Factor (VIF):</strong>
        <ul>
            <li>Reviewed VIF scores to address multicollinearity. Key features with high VIF values were considered for feature selection.</li>
        </ul>
        <table>
            <thead>
                <tr>
                    <th>Feature</th>
                    <th>VIF</th>
                </tr>
            </thead>
            <tbody>
                <tr><td>online_order</td><td>2.580422</td></tr>
                <tr><td>book_table</td><td>3.697239</td></tr>
                <tr><td>rate</td><td>100.615671</td></tr>
                <tr><td>votes</td><td>1.767582</td></tr>
                <tr><td>location</td><td>31.621818</td></tr>
                <tr><td>approx_cost(for two people)</td><td>12.031427</td></tr>
                <tr><td>listed_in(type)</td><td>15.694212</td></tr>
                <tr><td>listed_in(city)</td><td>58.392958</td></tr>
                <tr><td>is_new</td><td>1.153140</td></tr>
                <tr><td>weighted_rating</td><td>394.177513</td></tr>
                <tr><td>is_rate_valid</td><td>20.250555</td></tr>
                <tr><td>is_road</td><td>1.334013</td></tr>
                <tr><td>count</td><td>4.735270</td></tr>
                <tr><td>lat</td><td>100721.311388</td></tr>
                <tr><td>lon</td><td>101671.964833</td></tr>
                <tr><td>num_spec</td><td>23.435287</td></tr>
                <tr><td>num_dish_liked</td><td>40.287972</td></tr>
                <tr><td>num_reviews</td><td>1.244345</td></tr>
                <tr><td>num_menu_item</td><td>1.360053</td></tr>
                <tr><td>num_cuisines</td><td>34.303792</td></tr>
                <tr><td>cluster</td><td>6.643466</td></tr>
                <tr><td>classes</td><td>29.319548</td></tr>
                <tr><td>rest_type</td><td>15.245586</td></tr>
                <tr><td>cuisines</td><td>25.992990</td></tr>
                <tr><td>dish_liked</td><td>35.868954</td></tr>
            </tbody>
        </table>
    </li>
    <li><strong>Selected Features:</strong>
        <ul>
            <li>Based on VIF and heatmap analysis, the final features selected were: rest_type, cuisines, approx_cost(for two people), classes, num_spec, num_cuisines, num_dish_liked, listed_in(type), listed_in(city), num_reviews, book_table, online_order, votes, is_rate_valid.</li>
        </ul>
    </li>
    <li><strong>Standardization:</strong>
        <ul>
            <li>Applied StandardScaler to normalize feature values, ensuring that larger values have a comparable effect to smaller values.</li>
        </ul>
    </li>
</ol>

<h3>Model Performance</h3>

<ol>
    <li><strong>Random Forest:</strong>
        <ul>
            <li>Configuration: 600 estimators.</li>
            <li>Results:
                <ul>
                    <li><strong>Training Score:</strong> 0.9685</li>
                    <li><strong>R² Score:</strong> 0.7961</li>
                    <li><strong>MAE:</strong> 111.75</li>
                    <li><strong>MSE:</strong> 26100.80</li>
                    <li><strong>RMSE:</strong> 161.56</li>
                </ul>
            </li>
        </ul>
        <img alt="Random Forest Results" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhQNVrUKo_fyM9yWtTY5RMumso9xHzTstR6eC1lIipaOeq8DbRaN4ROoodKZgJhyphenhyphenvhOBkDBCgeZdfe_-BKOOyufDdQi6def6afV1gFPO7-nz0uGlby8C7GsEtSPaguhV2j5WsMmIM3-9wV3kULgPamM6hVt6nexG35Nwd9OGTyiEnW29Xt7_RcU9suY2f4/s1600/download.png">
    </li>
    <li><strong>XGBoost:</strong>
        <ul>
            <li>Configuration:
                <ul>
                    <li>objective: 'reg:squarederror'</li>
                    <li>learning_rate: 0.1</li>
                    <li>max_depth: 6</li>
                    <li>alpha: 10</li>
                    <li>n_estimators: 100</li>
                    <li>eval_metric: 'rmse'</li>
                </ul>
            </li>
            <li>Results:
                <ul>
                    <li><strong>MAE:</strong> 110.13</li>
                    <li><strong>MSE:</strong> 25320.74</li>
                    <li><strong>RMSE:</strong> 159.12</li>
                    <li><strong>R² Score:</strong> 0.8022</li>
                </ul>
            </li>
        </ul>
        <img alt="XGBoost Results" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhplF5GZhW7QVFBu_DLqlgvjD7LZtwqJc3yd1_DT-lxSQf3YbeEju-1sT4UTlGR4hOYMCCVPQFgqn9gPfnUIzvzSmKPtjPdxVNwoeKFAB0eE-IPxYxQwxoMnZrs0WXwLCgoR09rm82woFmMQAJMCRduOil8v5bABESbLc2i9BM7Y1aQQiuD7rmVjbIQl_8/s1600/download.png">
    </li>
    <li><strong>Neural Network:</strong>
        <ul>
            <li><strong>Model Structure:</strong>
                <ul>
                    <li>Input Layer: Dense layer with 13 units, activation function: tanh</li>
                    <li>Hidden Layer 1: Dense layer with 32 units, activation function: tanh, BatchNormalization, Dropout (0.18)</li>
                    <li>Hidden Layer 2: Dense layer with 64 units, activation function: tanh, BatchNormalization, Dropout (0.18)</li>
                    <li>Hidden Layer 3: Dense layer with 32 units, activation function: tanh, BatchNormalization, Dropout (0.18)</li>
                    <li>Output Layer: Dense layer with 1 unit</li>
                </ul>
            </li>
            <li><strong>Model Configuration:</strong>
                <ul>
                    <li>Optimizer: AdamW, learning rate: 0.1</li>
                    <li>Loss Function: Mean Squared Error</li>
                    <li>Epochs: 100000</li>
                    <li>Batch Size: 1024</li>
                </ul>
            </li>
            <li>Results:
                <ul>
                    <li><strong>MAE:</strong> 112.15</li>
                    <li><strong>MSE:</strong> 27070.94</li>
                    <li><strong>RMSE:</strong> 164.53</li>
                    <li><strong>R² Score:</strong> 0.7885</li>
                </ul>
            </li>
        </ul>
        <img alt="Neural Network Results" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj1B1Y0677pn8sP93GEnYOdJ1Z02hlNvvi10xqEpD70kLBswRGtLc3OsnJ8Qxx4RW_ll7-yGgetVyJCT4YG7szA48I0qekqvR73iF0RG11IGnD4RVuD0fx9cQSRRbE23whuTVNimbdaV0VwAGE1o-bd5m_ffSwpNjTSYmUMsqJsAOBcDNKCy-gGq7f8-e4/s1600/download.png">
    </li>
</ol>

<h3>Future Improvements</h3>

<ol>
    <li><strong>Increase Review Volume and Enhance Aspect Analysis:</strong> Gather more reviews and utilize advanced aspect analysis using a paid LLM model. This will add more complexity to the model, leading to more accurate predictions.</li>
    <li><strong>Improve Address Accuracy:</strong> Obtain more precise addresses or correct existing ones. This will help reveal detailed location information, which can significantly impact price predictions.</li>
    <li><strong>Incorporate Detailed Menu Pricing:</strong> Instead of predicting an approximation for the entire menu, obtain detailed menus with item-specific prices. This approach will enhance the accuracy of price predictions.</li>
    <li><strong>Expand Data Collection:</strong> Collect additional data to improve the overall model performance and prediction accuracy.</li>
</ol>
<div style="clear: both;"></div>
</div>
