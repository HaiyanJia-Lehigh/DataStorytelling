## Online Data Collection 1: Data Scraping

- **Getting Started with ParseHub**
  -   Please download ParseHub and create an account on their website: https://www.parsehub.com/.
  -   If you'd like, check out the [ParseHub tutorials](https://help.parsehub.com/hc/en-us/categories/202638628-Using-ParseHub). You might want to start with "Example: Create your first ParseHub project."
  
  
- **Using ParseHub to scrape online data**
  1.   Open ParseHub software, log in with account information, and create a new project.
  2.   We will use Teachers Salary Project as an example. Enter URL for Teacher salary data feed: http://teachersalaryproject.org/state-data/
  3.   Click on Alaska as selection 
       *  Change selection name to “State” 
       *  Scroll down and click yellow check mark next to Arkansas 
       *  All States on the page should be recognized as such now
  4.   Click the + next to select State
       *  Choose relative select
       *  First Click on Alaska
       *  Then drag the arrow down and click on the per pupil spending figure for Alaska
       *  Now click on Arkansas
       *  Then drag the arrow down and click on the per pupil spending figure for Alaska
       *  You should now have pupil figures for all states on the page
       *  Rename that selection to “Pupil”
  5.   Repeat Step IV for inmate spending and name it “Inmate”
  6.   Repeat Step IV for salary change and name it “Salary”
       *  Note that only 19 of 20 states on page find that subselection 
       *  You can manually add the missing one if you can find it 
       *  OR wait and clean it up in final output
  7.   Click the + next to "select page"
       *  Click on select
       *  Click on “next” at bottom of page
       *  Change selection name to “Next”
  8.   Click the + next to "Next" selection (*NOTE THIS MAY NOT WORK; MORE EXPLANATION AND OPTIONS BELOW*)
       *  Select “Click” from menu
       *  Answer “Yes” that “Next” is a next page button
       *  Click on advanced and increase 5 second wait to 30 seconds
       *  Click on “Repeat Current Template” button
  9.   Click on “get data” button
       * Click “Run”
       * Wait for scraping to finish running
       * Click on CSV/Excel to download data
  10.   Review data and clean up as needed

- **What to do if "Next Page" selection does NOT work?"**
  -   Note that newly created projects will not page to next page following directions above. To fix, you could either request adding an "Ignore Disable Element" checkbox from the website by chatting to the customer service, or
  -   Pagination Fix:
      1. Enter your project and click on the blue menu icon and choose export project
      2. Save as phj file
      3. Open that file in a text editor like notepad
      4. Change "ignoreDisabledElements\":true TO "ignoreDisabledElements\":false
      5. Save file
      5. Import edited project into project list
      6. Use imported project


- **Assignment**
  -   Scrape the ACLUs list of cases, press releases, blogs, podcasts, and other publications on Racial Profiling found here
https://www.aclu.org/search/%20?f[0]=field_issues:245
  -   Create a quick view table of all of these items including title, URL, date, and type (as shown below)
  -   Please write a short description of your data
*Note: you do not have to scrape all 600+ items, but see if you can at least scrape beyond the first page of 10 results.

![ParseHub Assignment](https://github.com/HaiyanJia-Lehigh/DataStorytelling/blob/master/ParseHub%20Assignment%20SP21.png?raw=true)

  -   **ALTERNATIVELY:** Scrape data from any other web site of your choice. Try to find an example that has formatted consistent data, but not already in tabular form and without a direct data download available. In your description, please also explain your rationale for choosing this data.
