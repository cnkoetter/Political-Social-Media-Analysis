# Political-Social-Media-Analysis

This dataset, from Crowdflower's Data For Everyone Library, provides text of 5000 messages from politicians' social media accounts, along with human judgments about the purpose, partisanship, and audience of the messages.

How was it collected?
Contributors looked at thousands of social media messages from US Senators and other American politicians to classify their content. Messages were broken down into audience (national or the tweeter’s constituency), bias (neutral/bipartisan, or biased/partisan), and finally tagged as the actual substance of the message itself (options ranged from informational, announcement of a media appearance, an attack on another candidate, etc.)

Acknowledgments
Data was provided by the Data For Everyone Library on Crowdflower.

Our Data for Everyone library is a collection of our favorite open data jobs that have come through our platform. They're available free of charge for the community, forever.

Inspiration
Here are a couple of questions you can explore with this dataset:

what words predict partisan v. neutral messages?
what words predict support messages v. attack messages?
do politicians use Twitter and Facebook for different purposes? (e.g., Twitter for attack messages, Facebook for policy messages)?
The Data
The dataset contains one file, with the following fields:

unitid: a unique id for the message
_golden: always FALSE; (presumably whether the message was in Crowdflower's gold standard)
unitstate: always "finalized"
trustedjudgments: the number of trusted human judgments that were entered for this message; an integer between 1 and 3
lastjudgment_at: when the final judgment was collected
audience: one of national or constituency
audience:confidence: a measure of confidence in the audience judgment; a float between 0.5 and 1
bias: one of neutral or partisan
bias:confidence: a measure of confidence in the bias judgment; a float between 0.5 and 1
message: the aim of the message. one of:
-- attack: the message attacks another politician
-- constituency: the message discusses the politician's constituency
-- information: an informational message about news in government or the wider U.S.
-- media: a message about interaction with the media
-- mobilization: a message intended to mobilize supporters
-- other: a catch-all category for messages that don't fit into the other
-- personal: a personal message, usually expressing sympathy, support or condolences, or other personal opinions
-- policy: a message about political policy
-- support: a message of political support
message:confidence: a measure of confidence in the message judgment; a float between 0.5 and 1
orig__golden: always empty; presumably whether some portion of the message was in the gold standard
audience_gold: always empty; presumably whether the audience response was in the gold standard
bias_gold: always empty; presumably whether the bias response was in the gold standard
bioid: a unique id for the politician
embed: HTML code to embed this message
id: unique id for the message WITHIN whichever social media site it was pulled from
label: a string of the form "From: firstname lastname (position from state)"
message_gold: always blank; presumably whether the message response was in the gold standard
source: where the message was posted; one of "facebook" or "twitter"
text: the text of the message
