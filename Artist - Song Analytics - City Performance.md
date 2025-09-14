# Artist - Song Analytics - City Performance

*Note: This page shows city-based performance rankings where cities are ranked by their engagement and performance metrics for the artist's songs.*

## Overview
The City Performance page displays analytics showing how the artist's songs perform across different cities, including rankings, play counts, and engagement metrics by geographic location.

---

### Task 1: Header Section

**User Story:**  
As an artist,  
I want to see a clear header section on the City Performance page  
so that I can understand what analytics I'm viewing and navigate back if needed.

**Acceptance Criteria:**

* AC 1: Display "City Performance" as the main page title

* AC 2: Include a back arrow button on the top left for navigation

* AC 3: Header should have a dark background consistent with the app theme

* AC 4: Title should be centered and clearly visible

* AC 5: Status bar should show current time, signal strength, and battery level

* AC 6: Header height should be appropriate for mobile viewing

---

### Task 2: Search Section

**User Story:**  
As an artist,  
I want to search for specific cities  
so that I can quickly find performance data for particular locations.

**Acceptance Criteria:**

* AC 1: Display a search bar below the header

* AC 2: Search bar should have a magnifying glass icon on the left

* AC 3: Placeholder text should read "Search"

* AC 4: Search bar should have rounded corners and dark background

* AC 5: Search functionality should filter cities in real-time as user types

* AC 6: Search bar should be responsive and easy to tap on mobile

* AC 7: Clear search option should be available when text is entered

---

### Task 3: Filter Section

**User Story:**  
As an artist,  
I want to filter city performance data by different metrics  
so that I can analyze the data from various perspectives.

**Acceptance Criteria:**

* AC 1: Display a filter dropdown on the right side above the city list

* AC 2: Default filter should show "Total Plays" with a dropdown arrow

* AC 3: Filter button should be aligned to the right margin

* AC 4: When clicked, show a bottom sheet with filter options

* AC 5: Filter options should include:
   - Total Fans
   - Total Plays

* AC 6: Each filter option should be displayed as a radio button

* AC 7: Include "Apply" button at the bottom of the filter sheet

* AC 8: Selected filter should update the city ranking accordingly

* AC 9: Filter dropdown should show the currently selected filter option

* AC 10: Bottom sheet should slide up smoothly when opened

* AC 11: Bottom sheet should have a semi-transparent overlay behind it

* AC 12: Tapping outside the bottom sheet should close it



---

### Task 4: City Ranking List

**User Story:**  
As an artist,  
I want to see a ranked list of cities based on performance metrics  
so that I can understand which locations have the highest engagement with my music.

**Acceptance Criteria:**

* AC 1: Display cities in a vertical scrollable list

* AC 2: List should be scrollable to accommodate many cities

* AC 3: Each city entry should have consistent spacing and alignment

* AC 4: City entries should have subtle separators or spacing between them

* AC 5: List should maintain proper ordering based on selected filter metric

* AC 6: Implement smooth scrolling performance for the list

* AC 7: List should update dynamically when filter is changed

* AC 8: Display vertical scroll bar when content exceeds screen height

---

### Task 5: City Detail Data

*Note: City refers to geographic locations where the artist's songs are being played and engaged with by fans.*

**User Story:**  
As an artist,  
I want to see detailed information for each city in the ranking list  
so that I can understand the specific performance metrics for different locations.

**Acceptance Criteria:**

* AC 1: Each city entry should display the city's ranking position

* AC 2: Show city image or representative icon

* AC 3: Display the full city name clearly

* AC 4: Include subtitle showing "Your Rank • #[position]"

* AC 5: Show the main performance metric (plays, fans, etc.) on the right

* AC 6: Display metric with appropriate formatting (e.g., 4.2K for 4,200)

* AC 7: Include visual indicator (arrow) showing trend direction

* AC 8: Use green color for positive metrics

* AC 9: Ensure consistent spacing and alignment across all entries

* AC 10: Make city entries visually distinct but cohesive

* AC 11: Optimize display for mobile screen sizes

* AC 12: Ensure text is readable with appropriate contrast
