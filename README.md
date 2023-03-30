# GroupProject1

CREATE PROCEDURE TP_06()
SELECT accounts.accountID, accHandle, accountType, accPrivacy, numPosts, numHighlights, numFollowers, numFollowing, accPass, communityName
FROM accounts
JOIN accounts_has_communities ON accounts_has_communities.accountID = accounts.accountID
JOIN communities ON accounts_has_communities.communityID = communities.communityID
WHERE EXISTS (SELECT scheduleID FROM `content schedule` WHERE scheduleFreq > 0);

CALL TP_06();



CREATE PROCEDURE TP_03()
SELECT communityName, COUNT(messageID)
FROM messages
JOIN accounts ON accounts.accountID = messages.accFrom
JOIN accounts_has_communities ON accounts_has_communities.accountID = accounts.accountID
JOIN communities ON accounts_has_communities.communityID = communities.communityID
WHERE TIME(timeSent) BETWEEN '11:59:59' AND '18:00:00'
GROUP BY communityName;

CALL TP_03();
