# ScamShield

Paste a suspicious text message, email or link and ScamShield explains, in plain words, which red flags it found and what to do next. Examples are built around scams common in the Philippines: fake bank and e-wallet alerts, parcel-fee texts, raffle prizes and fake job offers.

## How it works
A transparent rule-based scorer (no black box):
- **Message rules**: asking for OTP/PIN, deadline pressure, account-locked threats, surprise prizes, parcel fees, unrealistic pay, generic greetings, guaranteed returns
- **Link rules**: look-alike brand domains (for example `gcash-verify.xyz`), shortened links, raw IP addresses, throwaway endings, `http` instead of `https`
- Each rule adds a weight; the total is a 0 to 100 risk score with the matched text highlighted

## Test the detector
The second tab scores 20 made-up, hand-labeled messages (10 scams, 10 legitimate) and shows precision, recall, F1 and the confusion matrix. A slider changes the threshold so you can see the trade-off between missed scams and false alarms.

## Run
Open `index.html`. Nothing is sent anywhere.

## Limits and next steps
- Rules are easy to explain but can be evaded. A thesis version would train a classifier (Naive Bayes, logistic regression) on a larger collected dataset and compare it with this rule baseline.
- Package it as a browser extension or SMS-filter app and test with real users.
