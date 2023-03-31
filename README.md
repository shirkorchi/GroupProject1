# Instagram

# Group Members
- Emma Dolson
- Hannah Kelly
- Shir Kochi
- Kaden Williams
- Donovan Vanderpool

# Problem Description
Our data model represents the social media app, Instagram. The model consists of user accounts, which have associated profiles, content, and followers/following relationships. Each post can have multiple associated media, such as images or videos, which users can interact with through likes, comments, and shares. Instagram also supports messaging between users and the creation of stories, which are temporary posts that expire after a set time period. Tracking user activity helps Instagram generate personalized recommendations and trends to improve user experience. Despite being one of the most popular social media platforms in the world, Instagram does not allow its users to schedule posts in advance or to create communities of niche interests. From a backend perspective, our model demonstrates how users would interact with these two features and new insights Instagram could gain from them.

# Data Model
![image](https://user-images.githubusercontent.com/128431687/229206827-5b3a354d-d66f-47c4-8aea-3a7e74c22aea.png)

A user can have many accounts but an account can only have one user. An account can send and receive many messages but a message can only have one sender and one receiver. The content scheduler can schedule multiple instances of content but an instance of content can only have one schedule. Accounts and content can have many shares but each share can only belong to one account that shares one instance of content. Accounts can make many comments but one comment can only be made by one account. Content can have many comments but one comment can only be added to one instance of content. Accounts and content can have many likes but a like can only belong to one account and one instance of content. Accounts can belong to many communities and communities can have many accounts. Communities can have many community types and community types can have many communities.

# Data Dictionary 
[Data.Dictionary.pdf](https://github.com/shirkorchi/GroupProject1/files/11125146/Data.Dictionary.pdf)

# Queries
TP_Q1: This query converts the user's date of birth into their age as an integer and then returns the names of users who are younger than the input age. A query like this is helpful for censoring content like rated R movie trailers or explicit music for underage users.
![image](https://user-images.githubusercontent.com/128431687/229207632-a2cb0882-bce8-4af6-aca9-3efeb2387121.png)

TP_Q2: This query returns the username of accounts that have more followers than the average amount of followers for all accounts. A manager may be interested in this information to improve its algorithm and search engine. Screen Shot 2023-03-30 at 6 14 42 PM

TP_Q3: This query returns the number of messages a community has sent if the message was sent during the day (12:00-18:00). A query like this is can be helpful in determining when communities are most active or when messaging servers could potentially reach capacity. Screen Shot 2023-03-30 at 10 04 36 PM

TP_Q4: This query returns the number of messages each account has sent in descending order given that the account has more than 500 followers. A manager may be interested in this data to gauge how active a particular account is. Screen Shot 2023-03-30 at 10 15 04 PM

TP_Q5: This query returns the account handles that start with the letter "c," if any, as well as the name of the corresponding user and the community they belong to. A manager may be interested in this data to view information about accounts with related names quickly (by replacing “c” with whichever letter they choose). Screen Shot 2023-03-30 at 10 20 38 PM

TP_Q6: This query returns all attributes pertaining to accounts and the community they're a part of if the account uses content scheduling. A query like this may be helpful in determining certain attributes (type of account, number of posts, etc.) that may play a factor in determining whether or not the account uses the content scheduling feature. image

TP_Q7: This query will list the name and DOB of users that send messages with vanish mode and use content scheduling in order of oldest to youngest. A query like this is useful for tracking the use of some of the new features on Instagram. In more serious cases, this can also help track messages with illegal content back to their sender even if they attempt to hide the message by using vanishing mode. Screen Shot 2023-03-30 at 10 43 56 PM

TP_Q8: This query will list accounts’ ID, handle, and the user’s name and email address associated with the accounts that have no video content posted. A query like this is useful for being able to identify and contact individuals to promote Instagram’s video functionality. Screen Shot 2023-03-30 at 10 48 31 PM

TP_Q9: This query returns the account type and number of times each account type schedules content. A query like this could be helpful for adding possible features that cater towards account types that are frequent users of the content scheduler (ex. If a sports team has games every Saturday at noon, they can schedule a recurring post for each week of the season). Screen Shot 2023-03-30 at 10 51 43 PM

TP_Q10: This query returns the number of shares for each content type. A manager may be interest in this data to determine what type of content is shared the most among users (could be useful for ad monetization, promotions, etc.). Screen Shot 2023-03-30 at 11 02 51 PM

<img width="872" alt="Screenshot 2023-03-30 at 7 16 35 PM" src="https://user-images.githubusercontent.com/128431687/228985461-fb966b2b-ddf2-41c1-adf1-21a9ce91bb04.png">


TP_03:This query demonstrates the number of times messages were sent during the day (12 pm - 6pm) and what community they belonged to. From a managerial aspect, this would be important because it demonstrates the pattern of when group members are more active and what type of groups are interactive at certain times. This can help with knowing when are peak times to post specific ads or to learn when group members are not active and work to make the group interactive during the other times of day.


<img width="1141" alt="Screenshot 2023-03-30 at 7 08 59 PM" src="https://user-images.githubusercontent.com/128431687/228985695-85a9a6b9-153f-4891-acf9-87dcff2ec019.png">

TP_Q6: This query displays all the account info with the community they belong to only for the accounts that use content scheduling. From a managerial aspect, the query is important because it captures the pattern of the groups who use content scheduling. This helps by telling us which groups/accounts do not use it and with that information, we can find out why they don't and what we can do to encourage them to use the feature. 
