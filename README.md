- 👋 Hi, I’m @mbsmith9
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mbsmith9/mbsmith9 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.

I found this code from Jefferson at https://support.mozilla.org/en-US/questions/1351530but don't know how to put in in firefox so I'm looking for help here.

/*
  Multi-column Bookmarks Menu for Fx92
  Ref. https://www.reddit.com/r/FirefoxCSS/comments/m2iu4z/firefox_multicolumn_bookmarks/
  TODO: horizontal scroll for too many columns? [2021-09-23]
*/

/* USER PARAMETERS */

#bookmarksMenuPopup, #BMB_bookmarksPopup {
  --user-top-bottom-padding: 2px; /* spacing tightness; default is 8px */
  --user-items-per-column: 45; /* reduce if the menu doesn't fit */
}

/* RULES */

/* Modify bookmark spacing only in bookmark menus */
menupopup:not(.in-menulist) > menuitem, 
menupopup:not(.in-menulist) > menu {
  padding-block: var(--user-top-bottom-padding, inherit) !important;
  min-height: unset !important;
}

/* Keep width to a reasonable total */
#bookmarksMenuPopup, #BMB_bookmarksPopup {
  max-width: 80vw !important;
  overflow-x: scroll !important; /* DOESN'T WORK */
}

/* Apply grid layout */
.menupopup-arrowscrollbox * {
  display: grid;
  grid-auto-flow: column;
  grid-template-rows: repeat(var(--user-items-per-column, 40), auto);
  grid-auto-columns: minmax(200px, 380px);
}
--->
