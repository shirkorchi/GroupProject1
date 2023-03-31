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

<img width="872" alt="Screenshot 2023-03-30 at 7 16 35 PM" src="https://user-images.githubusercontent.com/128431687/228985461-fb966b2b-ddf2-41c1-adf1-21a9ce91bb04.png">


TP_03:This query demonstrates the number of times messages were sent during the day (12 pm - 6pm) and what community they belonged to. From a managerial aspect, this would be important because it demonstrates the pattern of when group members are more active and what type of groups are interactive at certain times. This can help with knowing when are peak times to post specific ads or to learn when group members are not active and work to make the group interactive during the other times of day.


<img width="1141" alt="Screenshot 2023-03-30 at 7 08 59 PM" src="https://user-images.githubusercontent.com/128431687/228985695-85a9a6b9-153f-4891-acf9-87dcff2ec019.png">

TP_Q6: This query displays all the account info with the community they belong to only for the accounts that use content scheduling. From a managerial aspect, the query is important because it captures the pattern of the groups who use content scheduling. This helps by telling us which groups/accounts do not use it and with that information, we can find out why they don't and what we can do to encourage them to use the feature. 
