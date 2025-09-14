# Song Analytic

## Page: Top Host

*Note: Host refers to fans of the artist who host songs on the platform. Hosting a song means fans share, promote, or feature the artist's songs on their social media profiles, playlists, or content, helping to increase the song's reach and engagement.*

### Task 1: Header Section

**User Story:**  
As an artist,  
I want to see a clear page header with navigation controls  
so that I can easily identify the current page and navigate back to the main song analytics page.

**Acceptance Criteria:**

* AC 1: Back button is prominently displayed in the top-left corner of the header
* AC 2: Back button successfully navigates to Song Analytics Main page with smooth page transition
* AC 3: Page title "Top Host" is clearly displayed in the center of the header
* AC 4: Header maintains consistent styling with the app's design system
* AC 5: Bottom navigation remains functional and highlights Analytics tab correctly
* AC 6: Header is fixed at the top during scrolling for consistent navigation access
* AC 7: Touch target for back button meets minimum size requirements (44px)
* AC 8: Header adapts properly to different screen orientations and sizes

### Task 2: Search Section

**User Story:**  
As an artist,  
I want to search for specific hosts  
so that I can quickly find relevant hosts in the ranking list.

**Acceptance Criteria:**

* AC 1: Search bar is prominently displayed below the header section
* AC 2: Search bar accepts text input for host usernames with placeholder text
* AC 3: Search filters the ranking list in real-time as user types
* AC 4: Search is case-insensitive and supports partial matches
* AC 5: Clear search button (X) resets search and shows full list
* AC 6: Search bar spans appropriate width for comfortable text input

### Task 3: Filter Section

**User Story:**  
As an artist,  
I want to access filter options through a bottom sheet when clicking "Total Plays"  
so that I can select different ranking criteria and apply filters to the host list.

**Acceptance Criteria:**

* AC 1: "Total Plays" filter button is positioned at top-right corner below search area
* AC 2: Clicking "Total Plays" button opens a bottom sheet overlay from the bottom
* AC 3: Bottom sheet displays "Select data filter" as the title with close (X) button
* AC 4: Bottom sheet contains "Total Fans" and "Total Plays" as radio button options
* AC 5: Only one filter option can be selected at a time using radio buttons
* AC 6: "Apply" button at bottom applies selected filter and closes bottom sheet
* AC 7: "Cancel" or close (X) button closes bottom sheet without applying changes
* AC 8: Bottom sheet has dark overlay background and smooth slide-up animation

### Task 4: Host Ranking List

**User Story:**  
As an artist,  
I want to view a scrollable ranking list of all hosts  
so that I can see the global performance rankings in an organized format.

**Acceptance Criteria:**

* AC 1: All hosts are displayed in a vertical scrollable list format
* AC 2: Hosts are ordered by the selected ranking metric (Total Plays or Total Fans)
* AC 3: Each host entry shows their position in the ranking
* AC 4: Status indicators (arrows, badges) are visible for ranking changes
* AC 5: List supports smooth vertical scrolling functionality
* AC 6: Scroll bar appears and functions properly during navigation
* AC 7: List displays all available host data in the ranking

### Task 5: Host Detail Data

*Note: Host refers to fans of the artist who host songs on the platform.*

**User Story:**  
As an artist, I want to see detailed information for each host in the ranking list  
so that I can understand their profile, performance metrics, and fan engagement levels.

**Acceptance Criteria:**

* AC 1: Each host entry displays profile picture or avatar
* AC 2: Host username is clearly displayed and readable
* AC 3: Fan rank information is shown for each host
* AC 4: Current metric value (Total Plays or Total Fans) is prominently displayed
* AC 5: Long usernames are handled with ellipsis to prevent layout breaking
* AC 6: Profile pictures load efficiently with placeholder during loading
* AC 7: All text maintains proper contrast ratios for readability
* AC 8: Host information is properly aligned and spaced
* AC 9: Data updates reflect accurate metric calculations
* AC 10: Loading states are shown during data fetch operations
* AC 11: Error handling for missing or failed data loads
* AC 12: Consistent typography hierarchy for all host information
* AC 13: Clicking on any host entry navigates to the Fan Profile page with smooth page transition
