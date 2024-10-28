I chose to create a website dedicated to sports news because sports play an important role in many people's lives, and I am personally passionate about various sports disciplines. On this website, users can access up-to-date information on the latest sports events, match results, upcoming championships, and follow their favorite teams. It’s a platform designed to help fans stay informed about everything happening in their favorite sports—from football to basketball and tennis. I wanted to create a convenient and dynamic website that offers users intuitive features and saves their preferences for an easy and personalized experience.

Functional features of the website:

   - User Authentication:  
     One of the key elements of the website is the user authentication system. I implemented a feature where users can register on the site by entering their name. This name is saved, and even after logging out or refreshing the page, the user’s name is remembered in the browser. So, upon their next visit, they don’t have to re-enter their details. This feature enhances user convenience by retaining personal data and making the experience more seamless.
   
   - Theme Switcher:  
     I added a theme switcher that allows users to toggle between light and dark modes. This isn’t just a visual change, but also a way to personalize the interface according to users’ preferences. Some may prefer a light background, while others may like a dark one. Furthermore, once a theme is selected, it’s saved, so even if the user closes the browser or reloads the page, their preference remains unchanged thanks to the use of `localStorage`.

   - News Filter:  
     Another important feature is the news filter. Users can choose which categories of news they want to see, such as only “RPL” (Russian Premier League), “World Cup,” or “EuroLeague.” Once a filter is selected, only news matching the chosen category is displayed. Additionally, the selected filter is saved, so even after refreshing the page or coming back to the site later, the user will still see the filtered news they selected earlier. This makes the site more personalized for each user.

Using `localStorage` to save data:

   To implement all these features, I utilized the browser's `localStorage`, which allows data to be saved on the user's side and persists even after the browser is closed or the page is refreshed. Here’s how it works:

   - Saving the user’s name:  
     When a user registers, their name is saved in `localStorage`. This allows the site to load the user’s name during future visits so they don’t have to re-enter it each time. I used `localStorage.setItem()` to store the data and `localStorage.getItem()` to retrieve it when needed.

   - Theme switcher:  
     When the user switches the theme to either dark or light, the selected color scheme is also saved in `localStorage`. This means that after refreshing the page, the website automatically applies the last selected theme by loading the value from the storage.

   - News filtering:  
     When a user selects a filter to display only certain categories of news, that filter is saved in `localStorage`. This way, on their next visit, the filter is automatically applied, and the user doesn't have to adjust the display preferences again.

Thus, by using `localStorage`, I am able to save personal settings for users—their name, website theme, and news filters—and restore them when they revisit the site. This significantly improves the user experience by making the website more personalized and user-friendly.
