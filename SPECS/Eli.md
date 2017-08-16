# Ideas for how to process data
0. Curl/get http://santamonicacityca.iqm2.com/Citizens/calendar.aspx
1. Find div id="ContentPlaceholder1_pnlMeetings"
2. For Each Meeting Row -> RowTop -> RowLink -> a tag
    a. Get href value parse for Meeting ID
    b. Follow href
        * Get Meeting Group and type and date from spans with ids: having prefix "ContentPlaceholder1_lbl" and suffixes "MeetingGroup", "MeetingType", "MeetingDate" 
        * Search for Special Agenda Items:
            1. 
