# google-sheet-gantt
Render a Google Charts gantt diagram from a Google sheet

Follow instructions below to generate Client ID / API Key:

https://developers.google.com/sheets/api/quickstart/js

Copy config.sample.json to config.json

The visit index.html?sheetId=[Sheet Id]&range=[Data range]
Data range should exclude any header rows.

## Parameters

* sheetId - The ID of the google sheet
* range - The range inside the sheet
* height - The hight in pixels of the chart
* start - The start date

The columns of the range should be:

* Task Id
* Task Name
* Resource
* Start (Either: Blank, Date or + Days from start, i.e. +5 for five days after start date)
* End
* Duration (Days)
* Percent Complete
* Dependencies

See full details here:

https://developers.google.com/chart/interactive/docs/gallery/ganttchart
