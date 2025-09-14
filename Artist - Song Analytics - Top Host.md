# Song Analytic

## Page: Top Host

### General Information
The Top Host page displays a comprehensive ranking system for hosts based on their performance metrics. This page provides detailed analytics for host rankings with real-time data updates, allowing users to track performance changes over time. Users can filter data by different metrics (Total Fans, Total Plays), search for specific hosts, and monitor ranking movements with clear visual indicators for improved, declined, or new entries in the leaderboard.

### Task 1: Top Host Ranking Dashboard

#### User Story
As an artist or content manager, I want to view a comprehensive ranking of top hosts for my songs so that I can:
- Track which hosts are performing best with my content
- Monitor ranking changes over time (up, down, new entries)
- Search for specific hosts quickly
- Filter rankings by different metrics (Total Fans vs Total Plays)
- Navigate easily back to the main song analytics page
- Understand my current position in the ranking system through visual scroll indicators

#### UI Components

**Header Section:**
- Back button (arrow left icon) for navigation to Song Analytics Main page
- Page title "Top Hosts" centered
- Status bar with time, signal, and battery indicators

**Search and Filter Section:**
- Search bar with magnifying glass icon and "Search" placeholder text
- "Total Plays" dropdown button with down arrow icon
- When dropdown is clicked, opens bottom sheet with filter options:
  - "Total Fans" option with radio button
  - "Total Plays" option with radio button (default selected)
  - "Apply" button at bottom

**Ranking List Section:**
- Scrollable vertical list of host entries
- Each entry contains:
  - Ranking number (#1, #2, etc.) on the left
  - Status indicator (green up arrow, red down arrow, or "NEW" badge)
  - Host profile picture (circular)
  - Host username (@aliflkpd format)
  - Fan rank information ("Fan Rank • #21")
  - Performance metric on the right ("4K" with green color)

**Navigation Section:**
- Bottom navigation bar with Home, Inbox, Plus, Analytics, and Profile tabs
- Analytics tab highlighted as active
- Notification badges on Inbox and Analytics tabs

**Scroll Indicator:**
- Horizontal scroll bar at bottom when scrolling to show current position
- Visual feedback for user orientation within the list

#### Acceptance Criteria

1. **Navigation Functionality**
   - Back button successfully navigates to Song Analytics Main page
   - Page transition is smooth and maintains app state
   - Bottom navigation remains functional and highlights Analytics tab

2. **Search Functionality**
   - Search bar accepts text input for host usernames
   - Search results filter the ranking list in real-time
   - Search is case-insensitive and supports partial matches
   - Clear search functionality resets to full list

3. **Filter Dropdown Functionality**
   - "Total Plays" dropdown opens bottom sheet overlay
   - Bottom sheet contains "Total Fans" and "Total Plays" radio options
   - Only one option can be selected at a time
   - "Apply" button applies the selected filter and closes bottom sheet
   - Filter changes re-sort the entire ranking list accordingly

4. **Ranking List Display**
   - All hosts are displayed in descending order by selected metric
   - Each entry shows complete information: rank, status, profile, username, fan rank, metric value
   - List supports smooth vertical scrolling
   - Minimum 10 host entries visible for comprehensive ranking view

5. **Status Indicator System**
   - Green up arrow (↑) displays for hosts with improved ranking
   - Red down arrow (↓) displays for hosts with declined ranking
   - "NEW" badge displays for hosts newly entered in leaderboard
   - Status indicators are clearly visible and color-coded appropriately

6. **Ranking Logic**
   - Hosts are sorted by highest performance metric first
   - Ranking numbers are sequential (#1, #2, #3, etc.)
   - Ties in metrics maintain consistent ranking order
   - Real-time updates reflect current performance data

7. **Scroll Position Indicator**
   - Horizontal scroll bar appears during vertical scrolling
   - Scroll bar accurately represents current position in the list
   - Scroll bar fades out after scrolling stops
   - Visual feedback helps users understand list length and current position

8. **Performance and Data**
   - Page loads within 2 seconds with cached data
   - Real-time updates occur every 30 seconds
   - Smooth scrolling performance with no lag
   - Accurate metric calculations and ranking updates

9. **Visual Design**
   - Dark theme consistency with app design
   - Proper spacing and alignment for all elements
   - Clear typography hierarchy for readability
   - Appropriate color coding for status indicators

10. **Responsive Behavior**
    - Layout adapts to different screen orientations
    - Touch targets meet minimum size requirements (44px)
    - Smooth animations for state changes
    - Proper handling of long usernames with ellipsis

11. **Error Handling**
    - Graceful handling of network connectivity issues
    - Loading states during data fetch operations
    - Empty state display when no hosts match search criteria
    - Error messages for failed filter applications

12. **Accessibility**
    - Screen reader support for all interactive elements
    - Proper contrast ratios for text and background
    - Keyboard navigation support where applicable
    - Voice-over descriptions for status indicators
