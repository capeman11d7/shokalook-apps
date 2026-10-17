# Teamdays: Team Calendar for Confluence

A shared calendar on any Confluence page or blog post: meetings, deadlines, releases and who's out of office. It works on every Confluence plan and needs no Google or Outlook account.

## Add a calendar to a page
1. Edit the page, type `/Teamdays` (or search "calendar"), and choose **Teamdays: Team calendar**.
2. In **Calendar settings**, give the calendar a name (optional) and pick the view it opens in: Month, Week or Agenda. Click **Save**.
3. Publish the page.

To change the name or the view later, edit the page, select the macro and click the pencil icon.

## Add, change and remove events
- **Add:** click a day, or drag across several days (or across hours in the week view). You can also click **+ Add event**.
- **Edit:** click an event, change it and click **Save**.
- **Move:** drag the event to another day or time. Drag its edge to make it longer or shorter.
- **Delete:** click the event, then **Delete**.

Each event has a title, a category, a start and an end (all day, or with times), an optional repeat rule, and notes.

## Categories
Meeting, Deadline, Release, Event, Out of office and Other each have their own color. The legend under the calendar shows them; click a category to hide or show it. That choice is remembered in your browser only.

**Out of office** events show the initials and first name of the person who added them, so add your own time off yourself.

## Repeating events
Set **Repeats** to Weekly, Monthly or Yearly, choose "every 1, 2, 3…" and optionally an **until** date.
- A monthly event on the 31st skips months without a 31st, and a yearly event on February 29 appears in leap years only (the same rule as Outlook and Google Calendar).
- To skip a single occurrence, click it and choose **Skip this date**.
- Editing or deleting a repeating event changes the whole series. Repeating events can't be dragged; edit them instead.

## Time zones
Everyone sees events in their own time zone. The dialog says which time zone it uses ("Times in Europe/London"). A repeating 9:00 meeting stays at 9:00 in its time zone when daylight saving starts or ends.

## Who can see and change the calendar
- Everyone who can **view** the page can see the calendar.
- People who can **edit** the page can add, change and delete events. Everyone else gets a read-only view.
- Each calendar belongs to its page. If you **copy the page**, the copy starts with an empty calendar (events aren't copied), so editors of the copy can never change the original's events. Use **Export .ics** if you need the events elsewhere.
- A page can hold several Teamdays calendars; each macro has its own events.

## Export to Outlook, Google or Apple Calendar
Click **Export .ics** to download every event as an .ics file, then import it into your calendar app. The export is a snapshot: later changes in Confluence don't update it.

## Limits
- Titles up to 200 characters, notes up to 5,000, events up to a year long.
- A calendar shows up to 5,000 events in one view. Busy days show 4 events and a "+N more" link.

## Data and privacy
Events are stored in Atlassian Forge storage for your site. The app has no servers of its own and sends nothing outside Atlassian. See the privacy policy for details.

## Support
Email rendermark.support@gmail.com. We reply within two business days.
