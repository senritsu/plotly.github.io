---
layout: connectors-tutorial-single_layout
title: Connect Your Charts and Dashboards to Parquet files with Apache Drill
subtitle: Graph data from your Parquet files using Apache Drill database with Plotly 2.0 and the Plotly Database Connector.
permalink: /database-connectors/apache-drill/
imageurl:  /static/images/database-connectors/logos/apache-drill.png
state: active
tags: other
section: Basics
meta_description: Follow these steps to connect to your Parquet files using Apache Drill
popularity: featured
actioncall-url: https://github.com/plotly/electron-sql-connector/releases

steps:
 - title: Download and Install the Plotly Database Connector App
   sub-steps:
    - copy: "If you haven't downloaded and installed the application yet, please follow the instructions for either [personal setup](/database-connectors/personal-login) or [company on-premise](/database-connectors/on-prem-login)."
 - title: Launch and Connect
   sub-steps:
    - copy: "Having launched the app, select *Postgres* by clicking on its icon."
      img: "![](/static/images/database-connectors/select-dialect/drill.png)"
    - copy: "Enter your username, password, database server name (*host*) and its port number."
    - copy: "Finally, click on the *connect* button!"
    - copy: "Once connection is established, your connection credentials will be saved and greyed out to avoid unintentional changes. If you wish to modify your connection, click on *edit credentials*."
      img: "![](/static/images/database-connectors/connected/drill.png)"
 - title: Preview Your Files
   sub-steps:
    - copy: "Two lists will appear. The values are the Plugins and Files available for querying."
      img: "![](/static/images/database-connectors/preview/drill.png)"
 - title: Send a Query to Your Database
   sub-steps:
    - copy: "Once you have successfully certified your database credentials and you have an [automatically generated an SSL](https://help.plot.ly/database-connectors/personal-login/#step-6-automatic-ssl), you are setup to begin querying data in Plotly. It is important to note that the automatically generated SSL can sometimes take up to *several minutes*, but don't worry, this authorization only needs to be completed once. Once you can see that is has been generated, click the 'Click to Open Query Editor' link under the 'Final Step. Query Data on Plotly' section. This will open the Plotly workspace in your default browser."
      img: "![Query data on Plotly](/static/images/database-connectors/v2/query-data-on-plotly.png)"
    - copy: "Now, the SQL import modal will appear. Simply, clik 'Next'"
      img: "![Import SQL modal](/static/images/database-connectors/v2/import-sql-modal.png)"
    - copy: "Verify that both 'https' is selected and your unique address is in the text box. Then click **Connect**"
      img: "![Verify and Connect](/static/images/database-connectors/v2/verify-and-connect.png)"
    - copy: "The modal will close and a new panel will be added to your Plotly Chart Creator."
      img: "![](/static/images/database-connectors/one-time-query/drill-editor.png)"
    - copy: "On the right, your available connections from the Plotly Database Connector will be displayed. If you have more than one, make sure you select the database connection that you want to use when writing the query."
      img: "![](/static/images/database-connectors/one-time-query/drill-connections.png)"
    - copy: "In this use case, we want to query parquet files, we wrote a SQL-like query as supported by Apache Drill to obtain data from our *sample-data* file as shown. Visit Apache Drill [documentation](https://drill.apache.org/docs/sql-reference/) for SQL-like queries to have a better understanding of its functionality."
      img: "![](/static/images/database-connectors/one-time-query/drill-query.png)"
    - copy: "Once your query is finalized, click *Run Query*. If you wish to set your query on a schedule to keep your grid's data updated to the latest entries of your database, visit our [schedule a query tutorial](http://help.plot.ly/database-connectors/schedule-query)."
      img: "![](/static/images/database-connectors/one-time-query/drill-data.png)"
 - title: Making a plot!
   sub-steps:
    - copy: "Let's visualize the complaints types from our dataset. Click on *Graph* on the left side of the window and choose *Histogram* as *Chart Type*. Select *Complaint Type* as the labels for the chart."
      img: "![](/static/images/database-connectors/make-graph/drill-graph.png)"
    - copy: "The graph will have been updated as per our data selection and we can notice that *Heating* was by far the highest complaint."
    - copy: "Finally let's not forget to save and share our graph. You can press Control + S to save or click on the *Save* button on the left of the window."
      img: "![](/static/images/database-connectors/make-graph/drill-share.png)"
    - copy: "You will be prompted to choose your privacy settings for this graph and data. There is nothing here to classify, let's simply set both *plot* and *data* to *public*. Click *SAVE*."
      img: "![](/static/images/database-connectors/make-graph/graph-save-modal.png)"
    - copy: "Let's share this interactive plot with a friend or a coworker (or both)! Click on the *SHARE* tab on the left."
    - copy: "The fastest way is to send the *Shareable Link*, copy and paste it into your favorite e-mail or other communication service. Try out our Twitter, Facebook and Google+ links as well or embed it into your website by obtaining the iframe link in the *Embed* tab. If you set the settings to *public* previously, your friend or coworker will be able to view it even without an account and give you feedback."
      img: "![](/static/images/database-connectors/make-graph/graph-share-modal.png)"

---
