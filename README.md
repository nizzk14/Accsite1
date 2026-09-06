Amity Coding Club (ACC) Website
This is the website we made for the Amity Coding Club. It's just one HTML file that has everything in it — the design, the styling, and the functionality. It shows our club's info, events, team members, photo gallery, and contact details, and it also has a light/dark mode and a small intro animation that plays when the page loads. DDT
Project Overview
We built this as a one-page website for our club. Instead of having separate pages for each section, everything (Home, About, Events, Gallery, Team, Achievements, Podcasts, Join, Contact) is on the same file, and we just show or hide the section the user clicks on. So it feels like an app where nothing reloads.
Some of the things we added:
A short intro animation with little doodles (like a dinosaur, chips, gears, etc.) that shows up for a second before the actual website appears.
A button to switch between light mode and dark mode.
A menu button (hamburger icon) that opens a slide-in menu to move between sections.
A photo gallery where you can click a photo and it opens bigger, and you can swipe between photos.
The whole website adjusts itself properly whether you open it on a phone, a tablet, or a laptop/computer.
A contact form, and buttons linking to our WhatsApp, Discord, Instagram, and LinkedIn.
What We Used
HTML – for all the content and structure of the page.
CSS – for all the styling (colors, spacing, animations, layout). We wrote it in a way where we could just flip one setting to change between light and dark mode instead of changing colors everywhere.
JavaScript – for the things that need to respond to clicks, like switching sections, opening the menu, changing the theme, and opening photos in the gallery.
Google Fonts – we used two fonts from Google Fonts (Fredoka and JetBrains Mono) to make the text look nicer.
All the icons are drawn directly as simple graphics inside the code (instead of using icon packs), and the photos are also stored directly inside the file, so we didn't need to keep separate image files.
We didn't use any extra tools, frameworks, or libraries — just plain HTML, CSS, and JavaScript in one file. There's no backend or database either, since it's just a website to show information.
How to Open/Install It
There's nothing to install. You just need the acc-site.html file.
Download the file (or clone the project if it's on GitHub).
That's it, there's no setup needed.
bash
git clone <your-repo-link>
cd <folder-name>
How to Run It
Since it's a single file, you can just open it like a normal file:
Double-click acc-site.html and it'll open in your browser.
Or, if you want to view it the way it would look on a real website, you can run it through a simple local server (not required, but sometimes better for testing):
bash
# If you have Python installed
python3 -m http.server 8000
# then go to http://localhost:8000/acc-site.html in your browser

# Or if you have Node.js installed
npx serve .
There's no build step, no installing packages, and nothing to compile — you just open the file and it works.
How We Designed It
We designed it first for mobile phones (since that's how most people would open it), and then added extra styling so it also looks good on bigger screens like tablets and laptops.
We kept all the colors in one place, so changing the theme (light/dark) is just a matter of switching one setting instead of changing every color individually.
We reused the same "card" style (the white/dark boxes with rounded corners) for different sections like team members, stats, and events, so everything looks consistent.
Instead of making separate HTML pages for each section, we just hide and show different parts of the same page using JavaScript. This makes it feel faster since nothing has to reload.
We kept the animations short and simple (like the intro doodles and the little blinking dot for live notices) so it feels lively but not distracting.
We avoided using outside images or icon packs as much as possible, so the website loads fast and doesn't depend on too many outside things.
Things This Website Needs to Work
It needs an internet connection just to load two fonts from Google Fonts (Fredoka and JetBrains Mono). That's the only outside thing it depends on. If someone needs it to fully work without internet, the fonts would need to be downloaded and added locally instead.
Apart from that, it doesn't need any other library, tool, or package to work.
Extra Notes / Things to Keep in Mind
Everything (HTML, CSS, JavaScript) is in the same file, so if you want to edit something, just search for the part you need inside acc-site.html instead of looking for separate files.
The gallery photos and event photos are currently placeholders. To add real photos, you'll need to add them into the image section of the code (look for data-gallery-key in the file).
All the text content (event names, team member names, notices, etc.) is written directly in the HTML, so to change any text, just find that part and edit it directly.
If you want to change the colors of the website, look for the color settings near the top of the style section — there are two sets, one for dark mode and one for light mode.
The responsive design (how it looks different on phone vs tablet vs laptop) is handled in a few specific sections near the end of the style code — it's better to add any new sizing changes there instead of spreading them around the file.
This website works best on newer browsers (like recent versions of Chrome, Edge, Firefox, or Safari)
