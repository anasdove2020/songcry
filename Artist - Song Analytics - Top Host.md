# Song Analytic

## Page: Top Host

### Task 1: Header Section

**User Story:**  
As an artist or content manager, I want to see a clear page header with navigation controls  
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

### Task 2: Search and Filter Section

**User Story:**  
As an artist or content manager, I want to search for specific hosts and filter the ranking by different metrics  
so that I can quickly find relevant hosts and view rankings based on my preferred criteria.

**Acceptance Criteria:**

* AC 1: Search bar is prominently displayed below the header section
* AC 2: Search bar accepts text input for host usernames with placeholder text
* AC 3: Search filters the ranking list in real-time as user types
* AC 4: Search is case-insensitive and supports partial matches
* AC 5: Clear search button (X) resets search and shows full list
* AC 6: "Total Plays" dropdown button is displayed next to search bar
* AC 7: Dropdown opens bottom sheet overlay with filter options
* AC 8: Bottom sheet contains "Total Fans" and "Total Plays" radio button options
* AC 9: Only one filter option can be selected at a time
* AC 10: "Apply" button applies selected filter and closes bottom sheet
* AC 11: "Cancel" button closes bottom sheet without applying changes
* AC 12: Current selected filter is indicated on the dropdown button

### Task 3: Host Ranking List

**User Story:**  
As an artist or content manager, I want to view a scrollable ranking list of hosts with status indicators  
so that I can see performance rankings and track changes in host performance over time.

**Acceptance Criteria:**

* AC 1: All hosts are displayed in descending order by selected metric
* AC 2: Each host entry shows rank number (#1, #2, #3, etc.)
* AC 3: Green up arrow (↑) displays for hosts with improved ranking
* AC 4: Red down arrow (↓) displays for hosts with declined ranking
* AC 5: "NEW" badge displays for newly entered hosts
* AC 6: Status indicators are clearly visible and color-coded appropriately
* AC 7: List supports smooth vertical scrolling
* AC 8: Minimum 10 host entries are visible for comprehensive ranking view
* AC 9: Horizontal scroll bar appears during vertical scrolling
* AC 10: Scroll bar accurately represents current position in the list
* AC 11: Scroll bar fades out after scrolling stops
* AC 12: Ties in metrics maintain consistent ranking order
* AC 13: Real-time updates reflect current performance data every 30 seconds
* AC 14: Smooth scrolling performance with no lag
* AC 15: Empty state display when no hosts match search criteria

### Task 4: Host Detail Data

**User Story:**  
As an artist or content manager, I want to see detailed information for each host in the ranking list  
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
