# Subtheme-Sentiment-Analysis
Applied KeyBERT &amp; BERT Model.

**Take the following example:**

“One tyre went missing, so there was a delay to get the two tyres fitted. The way garage dealt
with it was fantastic.”

_In this review there are numerous insights, insights we call “subtheme sentiments”. A Subtheme
sentiment is generally a sentiment towards an aspect or a problem._

If we look at the subtheme sentiments of the above review we will get a clearer sense what these
generally are.
_incorrect tyres sent negative     garage service positive     wait time negative_

The main difference between these subthemes is that Garage Service and Wait Time are aspects
of the service that can be positive or negative while
Incorrect Tyres Sent denotes a problem, something inherently negative.

**Task**
The task is to develop an approach that given a sample will identify the subthemes along with
their respective sentiments.
