# DHIS version 2.36 Release Note

This document highlights the key features of the initial release of DHIS2 version 2.36. This version is fully compatible with the DHIS2 [Android Capture App](https://www.dhis2.org/android-2-4) version 2.4.


## ANALYTICS FEATURES

**Scatter plots:** The data visualizer app now features scatter plots. This enables users to chart organisational units as points against two variables for a single period with scatter plots.

  - *Zoom in* by clicking and dragging the cursor over an area you would like to zoom in on. This is often necessary to see more detail in areas where many organisation units are clustered together.
  - *Outlier detection* can be done using either a standard z-score, modified z-score, or an interquartile range via the options menu. An extreme vertical (y-axis) and horizontal (x-axis) threshold line can also be applied. Endorsed by the WHO, this is a very clear and powerful way to identify outliers that often represent data quality issues. You can identify the outliers that are most likely to throw off national statistics by using the outlier detection in combination with the extreme X and Y threshold lines.

[Screenshot 1](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+scatter+plot+1.png) | [Screenshot 2](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+scatter+plot+2.png) | [Docs]()

**Full screen dashboard item presentation mode:** Expand any dashboard item (chart, map, or pivot table) to the size of the entire screen. This is great  for presenting data in virtual or in-person meetings directly from the dashboard.

[Screenshot](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+full+screen.JPG) | [Docs]()

**Bar and column chart legends:** Change the color of a bar or column based upon a predefined legend. This makes it easy to highlight under and over-performance with bar and column charts.

[Screenshot 1](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+chart+legend.png) | [Screenshot 2](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+chart+legend+2.JPG) | [Docs]()

**Mobile-friendly dashboard app:** The DHIS 2 dashboard web app is now more mobile-friendly and is more usable on mobile devices. This allows you to use the power of dashboards from your mobile device. Now you can take your dashboards with you, check them any time, and share data with anyone you need from the convenience of your phone. The app has adopted several of the principles of _Progressive Web Apps_ (PWA). Offline support to dashboards will come a in future release.

[Screenshot 1](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+PWA+1.jpg) | [Screenshot 2](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+PWA+2.jpg) | [Screenshot 3](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+PWA+3.jpg) | [Docs]()

**Population maps from Google Earth Engine:** Many DHIS2 instances suffer from not having adequate or accurate population values. This feature allows you to build maps with all data available in Google Earth Engine including the latest World Pop population estimates. You can apply a boundary layer to visualize the population totals, density by hectare, and average by hectare for organizational units. You can also apply a buffer around a facility or health post to see the population that falls within that buffer. Population dataset are available for age and sex disaggregation as well. These features allow you to quickly get the latest World Pop population estimates directly from the maps application. This is very useful feature for example in areas where census data is unreliable, for planning outreach or mass campaigns, and estimating risk for areas for high disease transmission.

[Screenshot 1](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+population+map+2.png) | [Screenshot 2](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+population+map+3.png) | [Screenshot 3](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+population+map+4.png) | [Docs]()

**Universal data item search:** The data visualizer app now supports search for data items across all types, making it much easier to find the data items you want across indicators, data elements, data sets, program data elements and program indicators. All you need to do is search for the data item and all matches will be displayed irrespective of data item type.

[Screenshot 1](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+universal+search+1.JPG) | [Screenshot 2](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+universal+search+2.JPG)| [Docs]()

**Dashboard filter settings:** Dashboard owners can now define which filters to make available for each dashboard. Often, a large number of data dimensions exist, and not all of them apply to the data in dashboard. This makes it cumbersome to find and select relevant data dimension. By defining exactly which data dimensions are relevant and become available for a dashboard, the user experience is simplified and made more engaging. Go to _Edit_ > _Filter settings_ to select filters.

[Screenshot](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+dashboard+filter+settings.png) | [Docs]()

**Visualization type constraints for dashboard items:** Countries and projects work hard to craft dashboards that tell a specific story. In these countries the visualization types (maps, charts, or tables) are carefully selected and optimized. In previous versions of DHIS2 a user can quickly change the visualization type of each dashboard item between a table, map, or bar chart, but sometimes this may undermine the carefully crafted story the dashboard owner is trying to communicate. Now system administrators can control the availability of the option to change visualization types of the dashboard item, the interpretations panel, the option to open the analytics in the relevant app, and the option for view full-screen. This is a system wide setting by the administrator through the system settings app and applies to all dashboards.

[Screenshot](https://s3-eu-west-1.amazonaws.com/content.dhis2.org/releases/screenshots/36/236+vis+type+constraints.png) | [Docs]()


## TRACKER AND EVENT FEATURES

**Performance improvements:** A huge number of performance improvements got included in 2.36 and there are broad improvements to tracker performance, in particular around database query optimizations. The improvements are leading to lower response times, faster database queries and less memory consumption. Most of these updates have been applied to versions 2.34.4, 2.35.2 and 2.36.0. Large scale DHIS2 implementations are advised to upgrade.

[Jira]()

**Tracker functionality in Capture app:** The capture app now has more support for tracker programs than before. Users will now be able to list and interact with tracked entity instances much in the same way as events, and will have access to searching and registering/enrolling tracked entity instances in the Capture app itself. Further interaction with enrollments and events in enrollments will in 2.36 still take place in the Tracker Capture app, but navigation between the apps will happen seamlessly. This will allow data entry user to access tracker and event data in the same place, and have a more integrated workflow.

[Screenshot 1](https://github.com/dhis2/dhis2-releases/blob/master/releases/2.36/images/capture_list_tei.png) [2](https://github.com/dhis2/dhis2-releases/blob/master/releases/2.36/images/capture_list_tei_filter.png) [3](https://github.com/dhis2/dhis2-releases/blob/master/releases/2.36/images/capture_search_tei.png) [4](https://github.com/dhis2/dhis2-releases/blob/master/releases/2.36/images/capture_register_tei_and_enroll.png) | [Docs]() | [Jira]()

**New endpoint for importing tracker data:** A new API for tracker data is now released side by side with the existing API. The new API is redesigned and reimplemented from the bottom up with a new architecture. The new implementation is more maintainable and yields a bigger potential for performance enhancements than it was possible to achieve in the old code base. The new API will run a full program rule execution, and allows server side field assignment and payload validation in addition to the existing functionality for sending messages. The new API is going to take the place of the existing one in later versions of DHIS2, but is released side by side at this time to allow app developers to start integration processes. 

[Docs]() | [Jira](https://jira.dhis2.org/browse/DHIS2-5068)

**New endpoint for retreiving tracker data:** A new API for retreiving tracker data is now released with the new endpoint for importing tracker data. This new API allows downloading tracker data on the same format as the new endpoint for importing data uses, making it easier to integrate with this new set of services.

[Docs]() | [Jira](https://jira.dhis2.org/browse/DHIS2-10093)


**New program indicator functionality:** It is now possible to build program indicator expressions and filters based on the event status, using the `V{event_status}` variable.
[Docs](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-master/configuring-the-system/programs.html#program_indicator_functions_variables_operators) | [Jira](https://jira.dhis2.org/browse/DHIS2-10294)

**Full name shown in notes** In tracker capture, the full name is now shown for the user that entered a note/comment. Previously only the username was shown. The full name is useful in cases where the username is not readable.

[Screenshot]() | [Jira](https://jira.dhis2.org/browse/DHIS2-9574)

**Keyboard-only data entry:** In tracker capture, data can now be entered without the use of a mouse. It is now possible to search and select options in option sets and boolean fields using the keyboard.

[Jira](https://jira.dhis2.org/browse/DHIS2-5902)

## PLATFORM FEATURES

**Outlier detection:** A new and improved outlier detection is available in the data quality app. Outlier values are now ranked and the most significant outlier are returned first, making it lot easier to find and correct the outlier values which greatly affects your data analysis. Previously, outliers were returned without an order. Outliers are ranked by *absolute distance from mean*. The *z-score* of the value, as well as mean, std dev, min and max are available in the response.

[Screenshot]() | [User docs]() |[API docs]() 

**OpenID Connect:** The OpenID Connect (OIDC) support is greatly improved. A generic solution is now available which will work with most OIDC providers.  Specific providers for Azure and WSO2 are also added. Providers which have been tested and verified to work are Google, Microsoft/Azure, Okta, Keykloak and WSO2. OIDC allows for Single Sign-On across multiple systems while managing identities in a central location.

[Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/data-validation.html#outlier-detection)

**Translations:** Dynamic metadata translations have been extended to cover many more entities and properties and allows you to translate most of the DHIS 2 application in any number of languages. This is helpful for multi-language DHIS2 instances.

[Docs]() | [Jira 1](https://jira.dhis2.org/browse/DHIS2-10562) | [2](https://jira.dhis2.org/browse/DHIS2-10556) | [3](https://jira.dhis2.org/browse/DHIS2-10487) | [4](https://jira.dhis2.org/browse/DHIS2-8669) | [5](https://jira.dhis2.org/browse/DHIS2-8297) | [6](https://jira.dhis2.org/browse/DHIS2-5587)

**User account expiration:** User accounts can now be set to expire on a particular date. This is useful for creating temporary accounts, e.g. when inviting partners through guest accounts.

[Docs]() | [Jira](https://jira.dhis2.org/browse/DHIS2-8089)

**Disable inactive users:** A new system job is available for automatically disable users which have been inactive (not logged in) for a given number of months. This is useful from a security perspective to prevent inactive user accounts from being compromised.

[Docs]()

**Data read sharing for SQL views:** Data read sharing is now required to read the output of an SQL view. This allows implementers to grant users access to read the output of SQL views without giving access to add or edit the views.

[Docs]()

**Data integrity checks performance:** The performance of the data integrity checks (in the data administration app) has been improved and completes a lot faster.

[Docs]()

**Disable program rule execution:** A new configuration property is available in `dhis.conf` for disabling/enabling server-side program rule execution.

[Docs]()

**Core application modernization:** The majority of core applications bundled with the 2.36.0 DHIS2 release have been upgraded to leverage the latest DHIS2 application suite of tools.  This ensures that modernized apps have identical headerbars, improved translation coverage, and more standardized user interface elements.

[Jira](https://jira.dhis2.org/browse/DHIS2-10026)

## API FEATURES

**Cluster leader node:** In a cluster setup, the ID of the leader node is available in the new `/api/cluster/leader` endpoint. This is useful to sysadmins to understand which node in the cluster is acting as the leader and is running scheduled jobs.

[Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/maintenance.html#cluster-info) | [Jira](https://jira.dhis2.org/browse/DHIS2-102579)

**Data value follow-up:** A new endpoint is available for marking data values for follow-up.

[Docs](https://docs.dhis2.org/master/en/dhis2_developer_manual/web-api.html#follow-up) | [Jira](https://jira.dhis2.org/browse/DHIS2-10344)

**Server timezone:** The server timezone information is added to the `/api/system/info` endpoint.

[Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/maintenance.html#webapi_system_resource_view_system_information) | [Jira](https://jira.dhis2.org/browse/DHIS2-9970)

**Delete validation results:** A new endpoint is available for deleting validation results.

 [Docs](https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/data-validation.html#webapi_validation_results) | [Jira](https://jira.dhis2.org/browse/DHIS2-74399)

## RELEASE INFO


|Release Information|Link|
| --- | --- |
|Download release and sample database|https://www.dhis2.org/downloads|
|Documentation|[https://www.dhis2.org/documentation](https://docs.dhis2.org/)|
|Upgrade notes|[Upgrade notes on GitHub](https://github.com/dhis2/dhis2-releases/blob/master/releases/2.36/README.md)|
|Details about each feature on JIRA|https://jira.dhis2.org/issues/?filter=XXXXX|
|Overview of bugs fixed on JIRA|https://jira.dhis2.org/issues/?filter=XXXXX|
|Source code on Github|https://github.com/dhis2|
|Demo instance|https://play.dhis2.org/2.36/|
|Docker|`docker pull dhis2/core:2.36.0`<br>_for more docker image variants see [dockerhub](https://hub.docker.com/repository/docker/dhis2/core)_|
|DHIS 2 community|https://community.dhis2.org/|
