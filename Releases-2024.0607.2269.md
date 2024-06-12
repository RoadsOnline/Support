# 2024.0607.2269 (7th June 2024)
## General ##

- fix: dont run the emailer except at configured times.
- fix: changed the dashboard with the upldated roadmap and logos. 

## TTRO Module ##

- fix: Show the date that the Social Media post will be sent in GMT() timezone 
- refactor: Change the way we get tags via a filter for email logs, to speed up performance. 
- fix: Ensure we through back a TTRORequestForList when searching via the TTRO search functionality. 

## Drivers Module ##

- fix: change license check reminder to be sent once per week by 
- feature: Change the drivers request to be more readable to a user. 
- feature: Add class code for driver permit assessment requests. 

## Winter Module ##

- fix: Fix issues with ARA Nightly function not sending emails. 
- feature: Allow the town to be associated with a depot.
