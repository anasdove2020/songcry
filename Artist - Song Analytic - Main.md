# Song Analytic

## Page: Song Analytic Main

### Task 1: Header Section

**User Story:**

As a user,  
I want to see a comprehensive header section  
so that I can navigate, select songs, and control playback.

**Acceptance Criteria:**

* AC 1: Header displays back button for navigation to previous page

* AC 2: Header background shows selected song cover image as background

* AC 3: Header contains dropdown selector for choosing different songs

* AC 4: Dropdown click opens bottom sheet with song list for selection

* AC 5: Bottom sheet displays comprehensive song selection interface with:

  * Search functionality to find specific songs

  * List of artist's songs with album artwork thumbnails

  * Song titles and artist names clearly displayed

  * Radio button selection for single song choice

  * "In Feed" status indicator for songs currently in feed

  * Apply button to confirm song selection

* AC 6: Song selection process allows artists to:

  * Browse through their complete song catalog

  * Search for specific songs using the search bar

  * Select one song at a time using radio buttons

  * View which songs are currently "In Feed"

  * Apply selection to update analytics display

* AC 7: Selected song updates all analytics data including:

  * Map visualization and performance metrics

  * Statistics dashboard numbers

  * City rankings and performance breakdowns

  * Total cities counter and breakdown categories

* AC 8: Header includes play button for music playback functionality

* AC 9: Play button navigates to feed page and starts playing selected song

### Task 2: Time Period Filter Dropdown

**User Story:**

As a user,  
I want to filter map data by time period  
so that I can analyze performance for specific timeframes.

**Acceptance Criteria:**

* AC 1: Dropdown displays current selected time period (default: "All-time")

* AC 2: Clicking dropdown opens bottom sheet with time period options

* AC 3: Bottom sheet includes comprehensive time period options:

  * Latest 24 hours

  * Last 7 days

  * Last 14 days

  * Last 30 days

  * Last 60 days

  * Last 90 days

  * Last 6 months

  * Last 12 months

  * All-time

* AC 4: "All-time" is selected by default

* AC 5: Selecting option updates dropdown display and closes bottom sheet

* AC 6: Apply button confirms selection and updates map data

* AC 7: Map dots and statistics update based on selected time period

### Task 3: Interactive Map Section

**User Story:**

As a user,  
I want to view an interactive map of the United States  
so that I can see geographical performance data of my song.

**Acceptance Criteria:**

* AC 1: Interactive map of United States displays with clear geographical boundaries

* AC 2: Map shows color-coded data points representing performance metrics with specific color coding:

  * Blue: Low Area (low performance regions)

  * Orange: Medium Area (medium performance regions)

  * Red: High Area (high performance regions)

* AC 3: Map supports zoom and pan functionality for detailed exploration

* AC 4: Clicking on map regions shows detailed performance data

* AC 5: Map legend explains color coding and data representation

* AC 6: Interactive slider below map allows adjusting starting point and end point

* AC 7: Slider supports drag functionality for both start and end handles

* AC 8: Moving slider dynamically updates map dots based on selected range

* AC 9: Slider provides visual feedback during interaction and range selection with time period-based functionality:

  * Start and end range are determined based on the selected time period (example: "Last 12 months")

  * If "Last 12 months" is selected: slider start = 12 months ago, slider end = now

  * User can move the starting point for dynamic filtering within the 12-month range

  * Total range remains 12 months, but can be shifted within that period

  * Map dots update in real-time according to the range selected on the slider

  * Total cities counter updates dynamically based on slider range selection

  * Breakdown area content (Blue, Orange, Red categories) updates automatically when slider changes

  * All statistics and performance metrics below the map refresh according to slider range

  * Enables comprehensive data filtering with complete UI synchronization within the same time period

* AC 10: Total cities counter displays number of cities with data for selected song (e.g., "32.245 Total cities") and updates dynamically when different songs are selected from dropdown

* AC 11: Breakdown area below "Total cities" title displays category statistics with color-coded performance metrics:

  * Blue (758): Number of cities with Low Area performance

  * Orange (987): Number of cities with Medium Area performance

  * Red (24K): Number of cities with High Area performance

* AC 12: Color coding in breakdown area correlates directly with map dots colors for visual consistency

* AC 13: Numbers represent exact count of cities for each performance category

* AC 14: Sum of all breakdown categories equals the total cities counter (e.g., 758 + 987 + 24K = 32.245)

* AC 15: Breakdown area updates dynamically when different songs are selected from dropdown

### Task 4: Tab Navigation System

**User Story:**

As a user,  
I want to navigate between different analytics views using tabs  
so that I can access Overview, Discovery, Audience, and Feed Insights data with Overview being the default view.

**Acceptance Criteria:**

* AC 1: Tab navigation bar displays four main tabs: Overview, Discovery, Audience, and Feed Insights

* AC 2: Overview tab is selected and active by default when the page loads

* AC 3: Active tab displays with distinct visual styling (highlighted/underlined) to indicate current selection

* AC 4: Clicking on any tab switches the view to display corresponding analytics data

* AC 5: Tab switching maintains smooth transitions without page reload

* AC 6: Each tab shows relevant content specific to its analytics category:

  * Overview: General performance metrics and map visualization

  * Discovery: Song discovery and reach analytics

  * Audience: Demographic and audience behavior data

  * Feed Insights: Social media and feed performance metrics

* AC 7: Tab state persists during user session until manually changed

* AC 8: All tabs remain accessible and functional across different screen sizes

* AC 9: Tab navigation provides clear visual feedback on hover and click interactions

* AC 10: Default Overview tab loads all associated content including map, statistics, and performance data

### Task 5: Song Performance Card Display

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS a user,  
I want to see a detailed song performance card  
so that I can quickly view key metrics and performance indicators for the selected song.

**Acceptance Criteria:**

* AC 1: Song performance card displays prominently in the Overview tab interface

* AC 2: Card shows song cover image/artwork as visual identifier on the left side

* AC 3: Song title "La La Lost You" is displayed clearly as the main heading

* AC 4: Location-based ranking shows current position with city/state (e.g., "#12 New York, NY")

* AC 5: Total plays counter displays formatted number with appropriate suffix (e.g., "14.7K" for thousands)

* AC 6: National ranking displays current position with "National Rank • #1" format

* AC 7: Peak position shows highest achieved ranking with "Peak Position • #1" format

* AC 8: Performance indicators use green up arrows (↗) to show positive performance trends

* AC 9: All ranking numbers (#12, #1, #1) are prominently displayed with consistent styling

* AC 10: Card layout maintains clean, organized structure with proper spacing and typography

* AC 11: Performance metrics update dynamically when different songs are selected from header dropdown

* AC 12: Card design follows consistent visual styling with the overall application theme

* AC 13: All text elements are clearly readable with appropriate contrast and font sizing

* AC 14: Card remains visible and accessible only within the Overview tab context

* AC 15: Performance indicators (arrows and numbers) reflect real-time data accuracy

### Task 6: Song Journey by States

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS an artist,  
I want to track my song's journey from initial upload through different US states  
so that I can understand how my music spreads geographically across state boundaries from the moment it was first uploaded.

**Acceptance Criteria:**

* AC 1: Song journey section displays below the song performance card within the Overview tab

* AC 2: Section header shows "\[Song Title] Journey" where the song title dynamically changes based on the artist's selected song (e.g., "La La Lost You Journey" when "La La Lost You" is selected), indicating the song's state-by-state progression

* AC 3: Two clickable tabs are available: "Song Journey" and "State Reach Over Time"

* AC 4: Song Journey tab is selected and active by default when Overview tab loads

* AC 5: Active tab displays with distinct visual styling (white background) while inactive tab shows darker styling

* AC 6: Clicking on either tab switches the view to display corresponding state-based analytics data

* AC 7: Song Journey tab displays state progression visualization with:

  * Circular state images/icons showing geographical progression (California, New York, Ohio)

  * Fan count numbers for each state showing new listeners gained (e.g., "132 New Fans")

  * Upload timeline showing when song first reached each state (e.g., "11/2/2025", "12/1/2025", "2/13/2025")

  * Arrow indicators (>>) showing chronological progression flow between states

  * Visual representation of song's state-by-state journey from initial upload

* AC 8: State Reach Over Time tab displays line chart visualization with:

  * Y-axis showing numerical scale from 0 to 500+ for state count metrics

  * X-axis showing time progression from upload date (Jan, Feb, Mar, Apr, May)

  * Purple/magenta colored line graph showing state expansion trajectory

  * Data point highlighting showing "232 New States (March 2025)" with milestone tooltip

  * Grid lines for easy tracking of state penetration over time

* AC 9: Tab switching maintains smooth transitions without affecting other Overview tab content

* AC 10: Both visualizations update dynamically when different songs are selected from header dropdown

* AC 11: Song Journey visualization shows chronological state penetration from upload date onwards

* AC 12: State Reach Over Time chart demonstrates geographic expansion patterns across US states

* AC 13: All data points reflect accurate state-based performance metrics from upload timeline

* AC 14: Visual elements (state icons, charts, numbers) maintain consistent styling with overall application theme

* AC 15: State journey tracking remains accessible and functional only within the Overview tab context

* AC 16: Header section includes info icon in the top left area for additional information access

* AC 17: Clicking info icon displays tooltip with contextual information (TBD)

### Task 7: Play Sources Analytics

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS an artist,  
I want to see detailed analytics about where my song is being played from different sources  
so that I can understand which platforms and sources are driving the most engagement.

**Acceptance Criteria:**

* AC 1: Play Sources section displays below the Song Journey section within the Overview tab

* AC 2: Section header shows "Play Sources" with clear visual hierarchy

* AC 3: Four main source categories are displayed with progress bars:

  * Feed: Shows percentage and visual progress bar (e.g., "45%")

  * Hosts: Shows percentage and visual progress bar (e.g., "45%")

  * Profile: Shows percentage and visual progress bar (e.g., "45%")

  * Shares: Shows percentage and visual progress bar (e.g., "45%")

* AC 4: Progress bars use consistent color coding (magenta/pink) for visual consistency

* AC 5: Each progress bar accurately reflects the percentage of plays from that source

* AC 6: Percentages are calculated based on total plays across all sources

* AC 7: Progress bars are visually proportional to their respective percentages

* AC 8: Source names are clearly labeled and easily readable

* AC 9: Section maintains consistent styling with other Overview tab components

* AC 10: Play Sources data updates dynamically when different songs are selected from header dropdown

* AC 11: All percentage calculations reflect real-time data accuracy

* AC 12: Progress bars provide smooth visual transitions when data updates

* AC 13: Section remains accessible and functional only within the Overview tab context

* AC 14: Header section includes info icon in the top left area for additional information access

* AC 15: Clicking info icon displays tooltip with contextual information (TBD)

### Task 8: Amount of Time Played Analytics

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS an artist,  
I want to see detailed analytics about the total amount of time my song has been played  
so that I can understand listening duration patterns and compare performance against other songs.

**Acceptance Criteria:**

* AC 1: Amount of Time Played section displays below the Play Sources section within the Overview tab

* AC 2: Section header shows "Amount of Time Played" with subtitle "Play Time (Hours)"

* AC 3: Main metric displays total hours in large format (e.g., "3.7 H") with prominent styling

* AC 4: Contextual description shows comparison status with three possible conditions:

  * "About the same as usual" with green checkmark icon (✓)

  * "Higher than usual" with green upward arrow icon (↑)

  * "Lower than usual" with red downward arrow icon (↓)

* AC 5: Interactive data point displays tooltip on hover showing detailed information:

  * Total playtime with specific duration (e.g., "Total playtime: 3.7 Hours")

  * Time period reference (e.g., "March 2025")

  * Tooltip appears with smooth animation and clear visual styling

* AC 6: Line chart visualization displays time-based analytics with:

  * Y-axis showing hours scale from 1.3 to 4.0 hours with appropriate intervals

  * X-axis showing monthly progression (Jan, Feb, Mar, Apr, May)

  * Pink/magenta colored line representing selected song performance ("La La Lost You")

  * Gray colored line showing "Other songs average" for comparison

  * Grid lines for easy data reading and trend analysis

* AC 7: Chart includes interactive data point highlighting for March 2025 milestone

* AC 8: Legend clearly identifies line colors and what they represent:

  * Pink dot: "La La Lost You" (selected song)

  * Gray dot: "Other songs average" (benchmark comparison)

* AC 9: Chart supports hover interactions for detailed data point information

* AC 10: All time-based data updates dynamically when different songs are selected from header dropdown

* AC 11: Chart maintains responsive design across different screen sizes

* AC 12: Visual styling remains consistent with other Overview tab analytics components

* AC 13: Time calculations reflect accurate listening duration data

* AC 14: Comparison metrics provide meaningful benchmark against artist's other songs

* AC 15: Section remains accessible and functional only within the Overview tab context

* AC 16: Header section includes info icon in the top left area for additional information access

* AC 17: Clicking info icon displays tooltip with contextual information (TBD)

### Task 9: Plays vs Skip Analytics

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS an artist,  
I want to see detailed analytics about plays versus skips for my song  
so that I can understand listener engagement patterns and identify whether my song retains audience attention or gets skipped frequently.

**Acceptance Criteria:**

* AC 1: Plays vs Skip section displays below the Amount of Time Played section within the Overview tab

* AC 2: Section header shows "Plays vs Skip" with clear visual hierarchy

* AC 3: Horizontal progress bar displays two distinct segments:

  * Left segment (pink/magenta): Shows "55% Played" with corresponding visual fill

  * Right segment (dark purple): Shows "45% Skip/Swiped Away" with corresponding visual fill

* AC 4: Progress bar segments are visually proportional to their respective percentages

* AC 5: Color coding uses consistent theme colors:

  * Pink/magenta for played content (positive engagement)

  * Dark purple for skipped content (negative engagement)

* AC 6: Percentage labels are clearly displayed within or adjacent to their respective segments

* AC 7: Below progress bar, two descriptive labels are shown:

  * Left label: "Played" (aligned with pink segment)

  * Right label: "Skip/Swiped Away" (aligned with purple segment)

* AC 8: Labels use appropriate typography and spacing for clear readability

* AC 9: Progress bar maintains smooth visual transitions when data updates

* AC 10: Percentages are calculated based on total listener interactions (plays + skips = 100%)

* AC 11: All engagement data updates dynamically when different songs are selected from header dropdown

* AC 12: Visual representation provides immediate understanding of listener retention vs abandonment

* AC 13: Progress bar design follows consistent styling with other Overview tab components

* AC 14: Section remains accessible and functional only within the Overview tab context

* AC 15: Data accuracy reflects real-time listener behavior patterns

* AC 16: Header section includes info icon in the top left area for additional information access

* AC 17: Clicking info icon displays tooltip with contextual information (TBD)

***

