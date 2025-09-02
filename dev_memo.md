I want to redo the website in the following way:

1. Change the style of the site.
   - Change the color scheme of the page to the one I used in gst.crepe.fund
   - Change the font and its sizes to the one I used in gst.crepe.fund
   - Change the layout to the one I used in gst.crepe.fund

2. In the "Navigation"
   - Leave the buttons "About" and "Docs" the same. 
   - Add a button to "Blog" and connect it to "https://medium.com/@CrepeFund".
   - Add a button to "GST" and connect it to "https://gst.crepe.fund".
   - Add another button "Staking", and connect it to "https://app.crepe.fund/staking/"
   - Add another button "under development" and make a pulldown menu with options "Crypto ETF", "Index", and "Lagrangian. Protocol". They must be connected to "under Construction" page to "https://crepe.fund/UnderConstruction". It means the "under Construction" page should be created.


3. In the hero section, change the phrase "Manage All The Assets On Earth" to "Prepare the Coming World of Cryto ETF and Stablecoins". The paragraph and the buttons below should stay the same.

4. As for "Why Crepe" Section, its content  should stay the same. 

5. As for "Status" Section, its content should stay the same.

6. As for "Applications" Section, the content must be deleted. 

7. As for "CREPE Index Board" Section, it should stay the same.

8. As for "Team" Section,
   - Change the size of the images of the team members to the same unique size. 
   - Add the team member "Nick Lee" to the team. With the following information:
     - Name: Nick Lee
     - Position: CTO
     - Image: Nick-Lee.jpg
     - Career: 
     - CEO at Crepe, Inc. 
       Professor at Konkuk University,      
     - LinkedIn: https://www.linkedin.com/in/youngwhan-nick-lee-71a89217/

9. As for "Partners" Section, its content should stay the same.

10. As for "Footer" Section, its content should stay the same.


## Implementation Status (2025-09-03)

- __Style__
  - Updated color scheme, fonts, and hover effects to align with gst.crepe.fund (CSS variables + gradients, modern sans-serif stack).

- __Navigation__
  - Kept: About, Docs
  - Added: Blog → https://medium.com/@CrepeFund, GST → https://gst.crepe.fund, Staking → https://app.crepe.fund/staking/
  - Added dropdown label: "Under Development" with items:
    - Crypto ETF → https://crepe.fund/UnderConstruction
    - Index → https://index.crepe.fund/
    - Lagrangian. Protocol → https://crepe.fund/UnderConstruction
  - Created Under Construction pages for development/production:
    - /UnderConstruction/index.html
    - /UnderConstruction.html
  - Removed the "Launch App" button from the nav.

- __Hero__
  - Updated heading to: "Prepare the Coming World of Cryto ETF and Stablecoins"
  - Paragraph and buttons unchanged.

- __Why CREPE__
  - Unchanged.

- __Status__
  - Unchanged.

- __Applications__
  - Entire section removed. Related popup script/styles removed.

- __CREPE Index Board__
  - Unchanged.

- __Team__
  - Standardized member images to 160x160, circular crop.
  - Added member: Nick Lee (CTO)
    - Image path: images/team/Nick-Lee.jpg (asset needed)
    - Career: CEO at Crepe, Inc.; Professor at Konkuk University
    - LinkedIn: https://www.linkedin.com/in/youngwhan-nick-lee-71a89217/

- __Partners__
  - Unchanged.

- __Footer__
  - Unchanged (styles aligned with new theme).

- __Local Preview__
  - Served via WSL: http://127.0.0.1:8000 (proxy available in IDE).
