# 🚧 UNDER CONSTRUCTION 🚧

# DHIS version 2.37 Release Note


## ANALYTICS FEATURES

**DEVELOPMENT**

**Dashboard default layout** will automatically configure a dashboard as users add more items. [jira](https://jira.dhis2.org/browse/DHIS2-3600)

**Drill-down in charts for period and org unit dimensions** is not possible as long as those demensions are not in the filter. [jira](https://jira.dhis2.org/browse/DHIS2-11061)

**Freeze for and column headers in pivot tables** will allow users to scroll through large pivot tables while not loosing reference to the data labels. [jira](https://jira.dhis2.org/browse/DHIS2-11057)

**Axis labels for multi-axis charts** [jira](https://jira.dhis2.org/browse/DHIS2-6672)

**Continuous analytics for event and enrollment data** will make it possible to see new tracker and event data added to your dashboard in real-time. [jira](https://jira.dhis2.org/browse/DHIS2-11188)

**DESIGN AND REQUIRMENTS GATHERING**

**Design of the new event reports/line listing application:** we are working on the next generation of the event reports and linelisting application. The development of this application is expected to extend through the 2.37 release and we expect the first version to be released in 2.38. [jira](https://jira.dhis2.org/browse/DHIS2-3442)

**New series management in the data visualizer application:** There is an ever expanding fuctionality in the data visualizer application, and this means that we periodically have to update your menues and user experience to keep the application easy to use. Now we are working to design a new series management menue so that we can continue to expand the fuctionality specifially around custom series colors. [jira](https://jira.dhis2.org/browse/DHIS2-11132)

## TRACKER AND EVENT FEATURES

**DEVELOPMENT**

**Performance improvements:** Improvements to Tracker database lock issues (concurrency); Improved routines and pipelines for performance testing; updates to new Tracker importer

**Deduplication:** Strengthening the search/warning on registration of new TEI; Improved services for returning potential duplicates

**Tracker features in Capture App:** new tool for generating and interacting with managements for TEIs; expand capture app to allow users to work with enrollments and events in tracker programs; user acceptance testing

**DESIGN AND REQUIREMENTS GATHERING**

**Deduplication:** design for merging of identified duplicates

**Tracker features in Capture App:** requirements for editing multiple TEIs in a line-listed format

**Sync**: requirements gathering and design for improved sync between instances / servers

## PLATFORM FEATURES


## API FEATURES

