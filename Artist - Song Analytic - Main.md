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

### Task 10: City Performance Analytics

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS an artist,  
I want to see detailed analytics about my song's performance across different cities  
so that I can understand geographic distribution of my audience and identify top-performing locations.

**Acceptance Criteria:**

* AC 1: City Performance section displays below the Plays vs Skip section within the Overview tab

* AC 2: Section header shows "City Performance" with navigational chevron (>) on the right

* AC 3: Clicking the "City Performance" header title navigates to the dedicated City Performance page

* AC 4: Header chevron (>) provides visual indication of navigation capability

* AC 5: Top-right corner displays dropdown filter with default selection "Total Plays"

* AC 6: Dropdown filter shows downward arrow (▼) indicating expandable options

* AC 7: Clicking dropdown filter opens bottom sheet modal with filter options:

  * "Select data filter" header with close (X) button in top-right

  * "Total Fans" option with radio button (unselected by default)

  * "Total Plays" option with radio button (selected by default, pink/magenta)

  * "Apply" button at bottom for confirming selection

* AC 8: Bottom sheet modal uses dark theme with white text for consistency

* AC 9: Radio button selection allows only one option to be active at a time

* AC 10: Clicking "Apply" button closes bottom sheet and updates city performance data

* AC 11: Clicking close (X) button dismisses bottom sheet without applying changes

* AC 12: City ranking list displays top 5 performing cities with following format:

  * Ranking number (#1, #2, #3, #4, #5) in white text

  * City thumbnail image (circular format)

  * City name as primary text (e.g., "New York, NY", "Utah", "Bali", "Los Angeles", "Boston")

  * Subtitle showing "Your Rank • #21" in gray text

  * Ranking status indicators with performance metrics:

    * Green upward arrow (↑): Indicates city moved up in ranking from previous period

    * Red downward arrow (↓): Indicates city moved down in ranking from previous period

    * "NEW" badge: Indicates city is newly entered into top 5 leaderboard

  * Performance metric (e.g., "4.2K") displayed with corresponding status indicator color

* AC 13: Each city list item maintains consistent spacing and alignment

* AC 14: City thumbnails display representative images for each location

* AC 15: Performance metrics (4.2K) reflect the selected filter data (Total Plays or Total Fans)

* AC 16: Green upward arrows indicate positive performance trends

* AC 17: "Your Rank • #21" subtitle provides artist's ranking context within each city

* AC 18: List items support hover states for better user interaction feedback

* AC 19: City performance data updates dynamically when different songs are selected from header dropdown

* AC 20: Filter selection persists during song switching until manually changed

* AC 21: All city data reflects accurate geographic performance metrics

* AC 22: Section maintains consistent styling with other Overview tab components

* AC 23: City Performance section remains accessible and functional only within the Overview tab context

* AC 24: Header section includes info icon in the top left area for additional information access

* AC 25: Clicking info icon displays tooltip with contextual information (TBD)

### Task 11: Song Data Analytics Dashboard

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS an artist,  
I want to see interactive song data analytics with multiple metric buttons  
so that I can analyze different performance aspects by switching between various data visualizations.

**Acceptance Criteria:**

* AC 1: Song Data Analytics section displays below the City Performance section within the Overview tab

* AC 2: Section header shows "Song Data" with clear visual hierarchy

* AC 3: Horizontal scrollable button container displays 5 clickable metric buttons:

  * "Plays" button (default selected with white background)

  * "Hosts" button (unselected with dark background)

  * "Followers" button (unselected with dark background)

  * "Returning Listeners" button (unselected with dark background)

  * "Total Fans Listened" button (unselected with dark background)

* AC 4: Button container shows only 3 buttons visible by default in the viewport

* AC 5: Horizontal scrolling functionality allows users to swipe/scroll right to reveal additional buttons

* AC 6: Smooth horizontal scroll animation when swiping between button sets

* AC 7: Each button displays metric name with clear, readable typography

* AC 8: Active button shows distinct visual styling (white background) while inactive buttons show darker styling

* AC 9: Clicking any button switches the active state and updates the corresponding graph below

* AC 10: Button selection maintains single-select behavior (only one button active at a time)

* AC 11: Below buttons, comprehensive analytics graph displays with:

  * Top metrics bar showing current values for selected metric (e.g., "230K" for Plays)

  * Percentage change indicators with color-coded arrows (green ↑ for positive, red ↓ for negative)

  * Time-based line chart with monthly progression (Jan, Feb, Mar, Apr, May)

  * Y-axis scale appropriate for selected metric (0-500 range)

  * Interactive data point highlighting with tooltip functionality

* AC 12: Graph tooltip displays detailed information on hover:

  * Specific metric value (e.g., "280 Plays")

  * Time period reference (e.g., "March 2025")

  * Smooth tooltip animation and positioning

* AC 13: Each metric button switches graph data to show corresponding analytics:

  * Plays: Shows play count trends and statistics

  * Hosts: Shows hosting activity and engagement metrics

  * Followers: Shows follower growth and retention data

  * Returning Listeners: Shows repeat listener behavior patterns

  * Total Fans Listened: Shows total fan engagement metrics

* AC 14: Graph maintains consistent visual styling across all metric types

* AC 15: Line chart uses consistent color coding (pink/magenta) for data visualization

* AC 16: Grid lines and axis labels provide clear data reference points

* AC 17: All metric data updates dynamically when different songs are selected from header dropdown

* AC 18: Button scrolling supports both touch/swipe gestures and mouse wheel interactions

* AC 19: Responsive design ensures proper button and graph display across different screen sizes

* AC 20: Section maintains consistent styling with other Overview tab components

* AC 21: All analytics calculations reflect accurate real-time performance data

* AC 22: Graph transitions smoothly when switching between different metrics

* AC 23: Section remains accessible and functional only within the Overview tab context

* AC 24: Header section includes info icon in the top left area for additional information access

* AC 25: Clicking info icon displays tooltip with contextual information (TBD)

### Task 12: Top Hosts Analytics

**User Story:**

GIVEN that I am viewing the Overview tab,  
AS an artist,  
I want to see detailed analytics about my top hosts and their fan engagement  
so that I can understand which fans are actively hosting my songs and driving community engagement.

**Acceptance Criteria:**

* AC 1: Top Hosts section displays below the Song Data Analytics section within the Overview tab

* AC 2: Section header shows "Top Hosts" with navigational chevron (>) on the right

* AC 3: Clicking the "Top Hosts" header title navigates to the dedicated Top Hosts page containing detailed artist's song host fans data

* AC 4: Header chevron (>) provides visual indication of navigation capability to Top Hosts page

* AC 5: Top-right corner displays dropdown filter with default selection "Total Plays"

* AC 6: Dropdown filter shows downward arrow (▼) indicating expandable options

* AC 7: Clicking dropdown filter opens bottom sheet modal with comprehensive filter options:

  * "Select data filter" header with close (X) button in top-right

  * "Total Plays" option with radio button (selected by default, pink/magenta)

  * "Total Plays Generated" option with radio button (unselected by default)

  * "Total Hosts Generated" option with radio button (unselected by default)

  * "Total Followers Generated" option with radio button (unselected by default)

  * "Apply" button at bottom for confirming selection

* AC 8: Bottom sheet modal uses dark theme with white text for consistency with application styling

* AC 9: Radio button selection allows only one filter option to be active at a time

* AC 10: Clicking "Apply" button closes bottom sheet and updates top hosts performance data based on selected filter

* AC 11: Clicking close (X) button dismisses bottom sheet without applying changes

* AC 12: Top hosts ranking list displays exactly 5 fan/host entries with following comprehensive format:

  * Ranking number (#1, #2, #3, #4, #5) in white text with consistent positioning

  * Circular profile image/avatar for each fan/host user

  * Username display with @ symbol format (e.g., "@aliflkpd") as primary identifier

  * Subtitle showing "Fan Rank • #21" in gray text indicating fan's ranking position

  * Ranking status indicators with performance metrics:

    * Green upward arrow (↑): Indicates host moved up in ranking from previous period

    * Red downward arrow (↓): Indicates host moved down in ranking from previous period

    * "NEW" badge: Indicates host is newly entered into top 5 leaderboard

  * Performance metric display (e.g., "4K") with corresponding color coding based on ranking status

* AC 13: Each fan/host list item (grid row) is fully clickable and navigates to individual fan profile page

* AC 14: Fan profile navigation provides detailed view of specific fan's hosting activity and engagement data

* AC 15: Profile images display high-quality circular avatars representing each fan/host

* AC 16: Username formatting maintains consistent @ symbol prefix for all entries

* AC 17: Fan Rank subtitle provides context about each fan's position within the artist's fan community

* AC 18: Performance metrics (4K) reflect the selected filter data (Total Plays, Total Plays Generated, etc.)

* AC 19: Ranking status indicators consistently reflect hosting performance trends and position changes

* AC 20: List items support hover states for better user interaction feedback and clickability indication

* AC 21: Each grid row maintains consistent spacing, alignment, and visual hierarchy

* AC 22: Top hosts data updates dynamically when different songs are selected from header dropdown

* AC 23: Filter selection persists during song switching until manually changed by user

* AC 24: All fan/host data reflects accurate hosting activity and engagement metrics

* AC 25: Section maintains consistent styling with other Overview tab components

* AC 26: Top Hosts section remains accessible and functional only within the Overview tab context

* AC 27: Header section includes info icon in the top left area for additional information access

* AC 28: Clicking info icon displays tooltip with contextual information (TBD)

### Task 13: Discovery Tab - Unique vs Returning Listeners Analytics

**User Story:**

GIVEN that I am viewing the Discovery tab,  
AS an artist,  
I want to see detailed analytics comparing unique versus returning listeners over time  
so that I can understand my audience retention patterns and discover insights about listener behavior trends.

**Acceptance Criteria:**

* AC 1: Discovery tab displays "Unique vs Returning Listeners" analytics section as the primary content area

* AC 2: Section header shows "Unique vs Returning Listeners" with clear visual hierarchy and professional typography

* AC 3: Header section includes info icon in the top left area for additional information access

* AC 4: Clicking info icon displays tooltip with contextual information (TBD)

* AC 5: Analytics chart displays comprehensive line graph with dual-line visualization:

  * Y-axis scale ranges from 0 to 10,000 with appropriate interval markings (0, 2,000, 4,000, 6,000, 8,000, 10,000)

  * X-axis shows monthly progression with clear labels (Jan, Feb, Mar, Apr, May)

  * Grid lines provide precise data reference points for accurate reading

* AC 6: Two distinct colored trend lines represent different listener categories:

  * Pink/magenta line represents "Return Listener" data with smooth curve progression

  * Purple line represents "Unique Listener" data with independent trend visualization

* AC 7: Interactive tooltip functionality displays detailed information on data point hover:

  * Shows specific listener count (e.g., "3,325 Return Listener")

  * Displays corresponding time period (e.g., "April 2025")

  * Tooltip appears with smooth animation and optimal positioning

  * White background with rounded corners for clear readability

* AC 8: Chart legend positioned at bottom of graph clearly identifies line colors:

  * Pink/magenta circle indicator with "Return Listener" label

  * Purple circle indicator with "Unique Listener" label

  * Legend maintains consistent styling with chart theme

* AC 9: Data visualization accurately reflects listener behavior patterns over the specified time period

* AC 10: Chart supports interactive hover states for enhanced user engagement and data exploration

* AC 11: Line chart maintains smooth curve rendering for professional data presentation

* AC 12: All chart elements (axes, grid, lines, labels) use consistent color scheme matching application design

* AC 13: Chart responsive design ensures proper display across different screen sizes and orientations

* AC 14: Data updates dynamically when different songs are selected from header dropdown

* AC 15: Chart loading states display appropriate indicators while data is being fetched

* AC 16: Error handling provides user-friendly messages if data cannot be loaded

* AC 17: Chart maintains accessibility standards with proper contrast ratios and screen reader support

* AC 18: Discovery tab remains accessible and functional only when explicitly selected by the artist

* AC 19: Section maintains consistent styling with other application components and tabs

* AC 20: All listener analytics calculations reflect accurate real-time audience engagement data

### Task 14: Discovery Tab - Audience Retention Analytics

**User Story:**

GIVEN that I am viewing the Discovery tab,  
AS an artist,  
I want to see detailed audience retention analytics with an interactive slider for my songs  
so that I can understand at what specific moments listeners drop off and optimize my content accordingly.

**Acceptance Criteria:**

* AC 1: Audience Retention section displays below the Unique vs Returning Listeners section within the Discovery tab

* AC 2: Section header shows "Audience Retention" with clear visual hierarchy and professional typography

* AC 3: Header section includes info icon (ⓘ) in the top left area for additional information access

* AC 4: Clicking info icon displays tooltip with contextual information (TBD)

* AC 5: Song cover image displays prominently in the upper section with high-quality resolution and proper aspect ratio

* AC 6: Interactive timeline slider positioned below the song cover with comprehensive functionality:

  * Horizontal slider bar spanning full width of the retention chart

  * Draggable handle/thumb positioned at current playback time (e.g., 2:02)

  * Time markers at start (0:00), current position (2:02), and end (2:46) of song duration

  * Pink/magenta colored handle for visual consistency with application theme

  * Smooth dragging interaction allowing precise time selection

* AC 7: Artist can drag slider handle to any specific time position (seconds/minutes) within song duration

* AC 8: Slider interaction immediately updates retention chart data to show audience behavior at selected time point

* AC 9: Subtitle "Average play duration over time" provides clear context for the retention analytics

* AC 10: Retention chart displays comprehensive audience retention visualization:

  * Y-axis shows percentage scale from 0% to 100% with clear interval markings (0%, 33%, 66%, 100%)

  * X-axis displays song duration timeline from 0:00 to 2:46 with appropriate time intervals

  * Horizontal dashed grid lines provide precise percentage reference points

  * Chart area uses dark background for optimal data visibility

* AC 11: Interactive tooltip displays detailed retention information:

  * Shows specific retention percentage (e.g., "66% of your audience")

  * Displays corresponding time duration (e.g., "stayed until 2:46")

  * Pink/magenta circular indicator for visual consistency

  * White background with rounded corners and proper positioning

  * Tooltip appears dynamically based on slider position

* AC 12: Dual-line chart visualization compares retention performance:

  * Pink/magenta line represents current song "La La Lost You" retention data

  * Gray line represents "Other songs average" as comparative baseline

  * Both lines display smooth curve progression with accurate data points

* AC 13: Chart legend positioned at bottom clearly identifies line meanings:

  * Pink/magenta circle indicator with "La La Lost You" label

  * Gray circle indicator with "Other songs average" label

  * Legend maintains consistent styling with chart theme

* AC 14: Real-time data synchronization ensures slider position matches tooltip information and chart highlighting

* AC 15: Slider supports both mouse drag and touch interactions for cross-device compatibility

* AC 16: Chart maintains smooth animation transitions when slider position changes

* AC 17: Retention data updates dynamically when different songs are selected from header dropdown

* AC 18: Slider range automatically adjusts to match selected song's actual duration

* AC 19: Chart responsive design ensures proper display across different screen sizes and orientations

* AC 20: All retention calculations reflect accurate listener behavior and drop-off patterns

* AC 21: Section maintains consistent styling with other Discovery tab components

* AC 22: Audience Retention section remains accessible and functional only within the Discovery tab context

* AC 23: Chart loading states display appropriate indicators while retention data is being fetched

* AC 24: Error handling provides user-friendly messages if retention data cannot be loaded

* AC 25: Chart maintains accessibility standards with proper contrast ratios and keyboard navigation support

### Task 15: Discovery Tab - Song Comparison

**User Story:**

GIVEN that I am viewing the Discovery tab,  
AS an artist,  
I want to see comprehensive song performance data with comparison metrics and interactive analytics  
so that I can analyze my song's performance against other tracks and understand detailed engagement patterns.

**Acceptance Criteria:**

* AC 1: Song Comparison section displays below the Audience Retention section within the Discovery tab

* AC 2: Section header shows "Song Comparison" with clear visual hierarchy and professional typography

* AC 3: Header section includes info icon (ⓘ) in the top left area for additional information access

* AC 4: Clicking info icon displays tooltip with contextual information (TBD)

* AC 5: Three metric cards display horizontally across the top section with comprehensive performance data:

  * Plays card shows dynamic value (e.g., "230K") with variable trend indicator (green upward/red downward arrow) and dynamic percentage change (e.g., "2%")
  
  * Hosts card shows dynamic value (e.g., "230K") with variable trend indicator (green upward/red downward arrow) and dynamic percentage change (e.g., "2%")
  
  * Followers card shows dynamic value (e.g., "230K") with variable trend indicator (green upward/red downward arrow) and dynamic percentage change (e.g., "2%")

* AC 6: Each metric card maintains consistent styling with white background, rounded corners, and proper spacing

* AC 7: Performance indicators use color-coded arrows for immediate visual understanding:

  * Green upward arrow (↗) indicates positive performance increase
  
  * Red downward arrow (↘) indicates performance decrease
  
  * Percentage values display with matching color (green for positive, red for negative)

* AC 8: Status indicator section displays below metric cards with comprehensive information:

  * Large number "805" prominently displayed with professional typography
  
  * Green checkmark (✓) icon indicating positive status
  
  * Descriptive text "About the same as usual" providing context for the metric
  
  * Gray text styling for subtle but readable information presentation

* AC 9: Interactive line chart displays comprehensive song performance analytics:

  * Y-axis scale ranges from 0 to 500 with clear interval markings (0, 100, 200, 300, 400, 500)
  
  * X-axis shows monthly progression with clear labels (Jan, Feb, Mar, Apr, May)
  
  * Horizontal dashed grid lines provide precise data reference points
  
  * Chart area uses dark background for optimal data visualization

* AC 10: Dual-line chart visualization compares performance data:

  * Pink/magenta line represents current song "La La Lost You" performance data
  
  * Gray line represents "Other songs average" as comparative baseline
  
  * Both lines display smooth curve progression with accurate data points

* AC 11: Interactive tooltip functionality displays detailed information on data point hover:

  * Shows specific play count (e.g., "Total Plays : 257")
  
  * Displays corresponding time period (e.g., "March 2025")
  
  * Pink/magenta circular indicator for visual consistency
  
  * White background with rounded corners and proper positioning
  
  * Tooltip appears with smooth animation and optimal placement

* AC 12: Chart legend positioned at bottom clearly identifies line meanings:

  * Pink/magenta circle indicator with "La La Lost You" label
  
  * Gray circle indicator with "Other songs average" label
  
  * Legend maintains consistent styling with chart theme and application design

* AC 13: Chart supports interactive hover states for enhanced user engagement and data exploration

* AC 14: All chart elements (axes, grid, lines, labels) use consistent color scheme matching Discovery tab design

* AC 15: Data visualization accurately reflects song performance patterns over the specified time period

* AC 16: Chart responsive design ensures proper display across different screen sizes and orientations

* AC 17: Song performance data updates dynamically when different songs are selected from header dropdown

* AC 18: Metric cards automatically refresh to show selected song's current performance statistics

* AC 19: Status indicator updates to reflect selected song's performance relative to historical averages

* AC 20: Chart loading states display appropriate indicators while performance data is being fetched

* AC 21: Error handling provides user-friendly messages if song data cannot be loaded

* AC 22: All performance calculations reflect accurate real-time song engagement and streaming data

* AC 23: Section maintains consistent styling with other Discovery tab components

* AC 24: Song Comparison section remains accessible and functional only within the Discovery tab context

* AC 25: Chart maintains accessibility standards with proper contrast ratios and screen reader support

***

