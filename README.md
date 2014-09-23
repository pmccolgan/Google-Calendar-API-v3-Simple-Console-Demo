#Google Calendar API v3 Simple Console Demo

Simple console application to use the Google Calender API v3 to read a calendar's events; I didn't find Google's .Net documentation/samples to be that helpful, this just acts as a starting point, something that works that can be built on.  Set up the credentials and it will read all the events in the calendar for the next year, printing out the date they occur and the summary.

To use set up application credentials for an installed application (this will produce a Client ID and Client Secret): https://developers.google.com/google-apps/calendar/instantiate

Ensure the calendar you want to read from is visible to the account you set up credentials for, get the calendar id: http://googleappstroubleshootinghelp.blogspot.co.uk/2012/09/how-to-find-calendar-id-of-google.html

Get the API packages to build: https://www.nuget.org/packages/Google.Apis.Calendar.v3/

Replace the three keys in the app.config:
```
        <add key="ClientId" value="YOUR_CLIENT_ID" />
        <add key="ClientSecret" value="YOUR_CLIENT_SECRET" />
        <add key="CalendarId" value="YOUR_CALENDAR_ID" />
```

When first run you may be prompted to grant calendar access to the application (this appears in a browser), approve this and the calendar should be readable.