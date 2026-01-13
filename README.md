<hr>
<h1>Most Recent Patch Notes: 1/11/2026</h1>
<hr>
<p>The You Matter to Me website is now live at: <a href="https://youmattertome.github.io/index.html" target="_blank">https://youmattertome.github.io/index.html</a></p>
<hr>
<h2>Executive Summary (TL;DR</h2>
<hr>
<ul><li> Complete copy relift featuring refreshed copy, up-to-date content, and descriptions that better reflect the hotlines & resources that appear on this website.</li>
<li> Standardized the information provided for each resource and implemented a consistent layout of information sitewide.</li>
<li> Updated and replaced broken links.</li>
<li> Improved scalability across all screen sizes for many components.</li>
<li> All resources now have descriptive subtitles under their titles. Subtitles are always visible, allowing users to get a better feel for what a resource has to offer before they decide whether or not to tap the expand/collapse button.</li>
<li> Resource contact information now collapses with the resource description, making the site easier to browse.</li>
<li> Fixed the long-standing bugs with the scrollspy misidentifying the user's position on the page and the sticky navbar overlapping section tiles when using navlinks to jump around the site.</li>
<li> Fixed an unusual bug in which the site would load half in light mode and half in dark mode under certain circumstances.</li>
<li> The censor (content warning system) has been reimagined from the ground-up and is now significantly more useful.</li>
<li> All :visited styles for links have been removed.</li>
<li> All legacy content provided by Jason, including the gradient backgrounds and borders, has been restored.</li>
<li> Added one new resource in the Veterans subsection of the Find Support section.</li>
<li> Updated the site to Bootstrap 5.1.3 and linked in jQuery 3.7.1 for new JavaScript features.</li>
<li> Cleaned up the code and improved its commenting and legibility.</li>
<li> Fixed questionable syntax, several semantics errors, and various typos across the site.</li>
</ul>
<p>Please note that this is the long-awaited part two of a two-part update. Closure for all of part one's Outstanding Issues can be found below. For more on the future of the You Matter to Me project, please see "On The Future" at the end of these patch notes!</p>
<hr>
<h2>The Flagship Features of This Update</h2>
<hr>
<h3>Refreshed Copy & Content Modernization — Overview</h3>
<ul><li> [Update on an Outstanding Issue from the last patch notes]: You Matter to Me was first released in 2021, and its resources have long been overdue for some fact-checking and a refresh...until now! All sorts of changes have transpired since the departure of the site's original researcher (a third team member who worked with Emma and Cassie). Fortunately, Miss Professional Writing Major Cassie <i>also</i> knows a thing or two about researching and writing copy. As of the past few months, she's been on the road to recovery, allowing her to finally shoulder this task...and, as of 01/12/2026, complete it!</li>
<li> [Outstanding issue, cont.]: Cassie tackled this mission from the ground up, so it ended up being less of a fact-checking and more of a total relift for <i>all</i> of the resources in the Find Support and Learn sections. This section of the patch notes will cover the changes to how this site approaches copy. Changes to the resources themselves (hotlines closing, org renames, added considerations, etc.) can be found in the "Resource/Hotline Updates" section of "Other Changes in This Version" below.</li>
</ul>
<h3>Refreshed Copy & Content Modernization — Fact-Checking & Modernization</h3>
<ul><li> For the sake of security, the last few http:// links have been phased out and replaced with modern https:// options. In a few cases, this changed the landing page, but it was always a significant improvement.</li>
<li> In one odd case (that of NAMI in the General subsection), the link now takes the user to the homepage <i>instead of</i> a helpline specific page, because the old link (and everything else I tried) resulted in the user being sent to NAMI's <i>sitemap</i> instead. Fortunately, the helpline-specific information <i>is</i> present on NAMI's homepage, one just needs to scroll down a little ways.</li>
<li> I've tested all the non-blue links on the site, including those for the list of emergency response numbers by country, resource/organization websites, peripheral links in resource descriptions, title links <i>and</i> "Visit!" buttons in the Find a Therapist section, the links to Emma's Twitch, SC Live, and Rise Above the Disorder (RAD) in the About Emma section, and the links to Github Pages, this site's Github repository, and Cassie's email in the footer. All issues identified along the way were successfully eliminated.</li>
<li> I've confirmed that all hotlines and other contact information provided (blue links) remain listed on the respective organizations' website. That said, I didn't test any of these blue links (for obvious reasons—these hotlines do important work, and dealing with curious web developers isn't in their job descriptions).</li>
</ul>
<h3>Refreshed Copy & Content Modernization — Copy Layout</h3>
<ul><li> Resources and hotlines now better utilize the available space in their sections across all screen sizes.</li>
<li> Removed the horizontal lines around section and subsection titles for a cleaner, more modern look.</li>
<li> The buttons to expand and collapse resources have been moved from the righthand side of their section elements to the lefthand side, right next to their resource titles. This ensures the buttons remain fixed in place and directly adjacent to their corresponding resource titles on all screen sizes.</li>
<li> The buttons to expand and collapse resources have been changed from plus signs ("+") to carats ("^")...or, technically, lowercase letter "v's." Each button rotates up 180 degrees when its resource is expanded and down 180 degrees when its resource is collapsed, providing a recognizable visual indicator of whether that resource is currently expanded or collapsed.</li>
<li> Added &lth5&gt subheadings to the contact information for the 988 Lifeline in the General subsection in particular, on account of its wide array of English and Spanish support options.</li>
<li> Contact information for resources now collapses with the descriptions and blockquotes rather than remaining permanently visible with the resource title (and subtitle, for the few resources that had one). This should better match typical user behavior, as folks are unlikely to choose resources to contact from the title alone.</li>
<li> Contact information is offset from the descriptions and blockquotes by way of an additional horizontal line (&lthr&gt element).</li>
</ul>
<h3>Refreshed Copy & Content Modernization — A Consistent Approach to Copy</h3>
<ul><li> All resources in Find Support and Learn now have subtitles. This allows users to get an idea for what each resource offers without having to hit the expand button and read through the entire blockquote. As such, it should now be a little easier for users to quickly locate resources that match their needs.</li>
<li> In accordance with a sitewide norm, all links that took the user to organizations' homepages rather than the helpline landing page have been upgraded to take the user directly to the helpline landing page.</li>
<li> All contact information for each resource is now grouped together at the top of that resource's expanded description, rather than scattered throughout the description.</li>
<li> All contact options for each resource now have blue links to allow for one-tap access. All Phone and Text options had this already, and most Email and TTY did, too. However, this greatly enhances the visibility of other options, including Live Chat and several more unique options for select references, including one WhatsApp, one CyberTipline, one forum, and one custom mobile app.</li>
<li> If hotlines that offer help in Spanish that requires users to call/text a different number or press additional buttons (e.g., "for Spanish, press '2'"), those instructions now have their own entries in the contact information, complete with blue links.</li>
<li> When hotlines require users to press additional buttons (e.g., "for Spanish, press '2'"), the names of those buttons now always appear in quotation marks (e.g., "2").</li>
<li> When hotlines require users to text a specific word or phrase to start a conversation, that word or phrase now always appears in all capitals and quotation marks (e.g., "HELP").</li>
<li> When hotlines offer a TTY option, it's now listed as "TTY" instead of "Deaf & Hard of Hearing TTY." Users who are deaf and hard of hearing are likely to be well aware of what TTY is and whom it's for—there's no need to insult their intelligence. Nevertheless, for the sake of others, the connection is still spelled out in the upcoming description section.</li>
</ul>
<h3>Refreshed Copy & Content Modernization — Standardization of Resource/Hotline Descriptions</h3>
<ul><li> The first paragraph of each resource's description section now follows a standardized layout that prioritizes the three most important pieces of information: availability (when known), country of operation (always), and language options (if different from "only English").</li>
<li> All hotlines that operate 24/7 now use the standard phrase, "available 24/7."</li>
<li> Hours for all hotlines with limited availability now follow a standard format.</li>
<li> [Update on an Outstanding Issue from the last patch notes]: All hotlines with limited availability now list their hours in U.S. Pacific Time, with hours in U.S. Eastern Time following in parenthesis. While I'd once hoped to display hotline hours in the user's timezone (via device time), the issues with this approach quickly became apparent. Most notably, there's no easy way to control for daylight savings time use (or lack thereof) among the resource organizations themselves. Ultimately, this idea was simply beyond my capabilities and would've required more human micromanagement of this website going forward than I was prepared to provide. The overwhelming majority of Emma's viewer base lives in the U.S. and Canada, and most of <i>those</i> users are on the west coast. As such, I'm confident that listing hours in west coasst time with an east coast translation readily available should meet the needs of as many users within the site's target demographic as is currently feasible.</li>
<li> All hotlines now use the standard phrase, "operates in..." when identifying their country/ies of operation.</li>
<li> All hotlines that offer support in English and Spanish now use the standard phrase, "offers support in English y en Español."</li>
<li> All hotlines that support TTY now have the addendum and explanatory comma, "as well as Deaf<li> & Hard of Hearing-accessible resources (TTY)."</li>
<li> All hotlines that offer support in additional languages or language interpretation services now list that information in a standard format that includes the number of languages served (listing them all wouldn't be feasible, as it's never fewer than 44).</li>
<li> Additional information, qualifiers, and advisories, have been implemented in subsequent description paragraphs on an as-needed basis.</li>
</ul>
<h3>Refreshed Copy & Content Modernization — Blockquotes</h3>
<ul><li> Blockquotes have received an overhaul! They've all been cross-referenced with the current copy of their respective organizations and updated accordingly, with a more intentional and consistent approach driving the information selection process.</li>
<li> Most all of the new blockquote copy is sourced from the website or resources of its respective organization.</li>
<li> Many of the blockquotes have been replaced or supplemented by new copy from the websites of their respective organizations that better captures those organizations' stated philosophy and priorities.</li>
<li> Where there wasn't much room for improvement in the blockquote copy, it was checked against the organization's website and modernized accordingly.</li>
<li> In a few cases where the original blockquote copy was both adequate and unchanged, it was retained unaltered.</li>
<li> In one or two edge cases where the original blockquote copy no longer appeared on its organization's website, but I couldn't find anything that better described the organization, the original copy was retained and touched up by me.
<li> In one or two edge cases where no copy on an organization's website adequately articulated that organization's philosophy and/or priorities, I added some novel phrasing of my own.</li>
<li> Blockquote attribution is now listed in the same font size as the rest of the blockquote text.</li>
<li> Quotation marks (" ") no longer appear in blockquotes. This freed me up to paraphrase rather than just quoting verbatim; in some cases, I blended direct quotations from across a given resource's website to better capture the breadth and scope of its approach.</li>
</ul>
<h3>Refreshed Copy & Content Modernization — Usability & Accessibility</h3>
<ul><li> The scalability of the site has been improved. The mobile version feels a little less claustrophobic, and the desktop version won't get quite as sprawling and expansive as it did in the past.</li>
<li> Enlarged the "hitbox" of the buttons to expand and collapse hotlines and resources to make them easier to click on mobile.</li>
<li> Implemented the Clearfix hack to keep resource titles and subtitles neatly aligned to the right of their respective buttons regardless of screen size.</li>
<li> Added more space between each contact information link to make it easier for users on mobile to click the one they intend to.</li>
<li> Added more padding to blockquotes, so they feel a little less cramped.</li>
<li> Improved tooltips and alt text for all &ltimg&gt elements, including the ones that didn't have tooltips in the past.</li>
</ul>
<h3>Enhanced User Safety</h3>
<ul><li> Deprecated and fully removed all :visited styles for all links on the website. For anyone without the rare luxury of a completely private device, a visual indicator of exactly which resources one has been exploring constitutes a privacy and safety risk—especially in the context of a website that features hotlines for domestic abuse, human trafficking, eating disorders, runaway children, and LGBTQ+ folks.</li>
</ul>
<h3>Restored All Legacy Content from Jason</h3>
<p>This last part is a little embarrassing, but I can't sidestep it any longer. A few years ago, Jason Docton was kind enough to help out with this project, instituting improvements across the website but most notably in the stylesheet. This was an invaluable service, introducing some industry tricks and best practices to a project otherwise coded by a web development amateur (me). Unfortunately, for an update from <i>years ago now</i>, Miss Web Development Amateur forgot to pull the code down from this repo; she just started editing the files saved on her computer. As a result, most of Jason's improvements were inadvertently reverted when the update went live. I then went on to fail to realize what I'd done until <i>spring of 2025</i>. <b><i>Whoops</i></b>.</p>
<blockquote><p>"When working on a collaborative project, always download the Github files for the current release before you start working."</p></blockquote>
<p>&nbsp&nbsp&nbsp&nbsp&nbsp– Almost every software developer ever, but apparently not Cassie</p>
<p>Oh, well...you live and you learn, I guess~</p>
<p>If there's a bright side to my little oversight, it's that I got to take on a challenge that really pushed me to grow as a developer: re-implementing all of the features Jason had added in code that had since changed again and again in their absence. I'm proud to announce that, in this update, I succeeded in restoring <i>every</i> feature that <b><i>I myself</i></b> had messed up!</p>
<h4>These features from Jason include:</h4>
<ul><li> Fluid type scales (clamping font-size) that greatly enhance the legibility of text by allowing for more dynamic responsiveness to screen size.</li>
<li> Many units given in rems rather than pixels. In fact, I ended up implementing rems even more broadly across the site.</li>
<li> Animated, seamless linear-gradient background for the header and footer.</li>
<li> Matching animated, seamless linear-gradient border for the Welcome section (aka, the "Hey!" section).</li>
<li> Implementation of overscroll lock.</li>
<li> Implementation of inheritable border-box.</li>
<li> A fix for the title overflow that occasionally cropped up on certain screen shapes and sizes.</li>
<li> A fix that stops images from overflowing their containers (something that used to happen in the Find a Therapist section).</li>
<li> A fix to prevent the new bottom bar added to Safari in iOS 15 from overlapping or clipping the website.</li>
<li> Better spacing on the stylesheet to improve code legibility on Github.</li>
</ul>
<p>Thank you again to Jason for providing the original code for these features! The website's looking better than ever now that they're all up and running again~</p>
<hr>
<h2>Other Changes in This Version</h2>
<hr>
<h3>Page Layout & Section Framework Changes</h3>
<ul><li> The "Learn About Mental Health" section has been renamed to "Learn & Grow" to reflect that the content there covers other facets of health and wellness in addition to mental health. For the sake of clarity, it will be referred to as the "Learn" section for the remainder of these patch notes.</li>
<li> Slightly reduced the amount of blank space after each resource/hotline, offering a more compact (yet still highly legible) readout.</li>
</ul>
<h3>Navigation Bar</h3>
<ul><li> [Update on an Outstanding Issue from the last patch notes]: The fidelity of the navigation bar is finally fixed, and the sticky navbar no longer hides the heading of the section to which the user navigates. This comes after no small amount of effort on my part. Evidently, this is a whole 'thing' with Bootstrap; Bootstrap is aware of it and claiming it's an intentional effect of the interplay between sticky navbars, navlinks, and scrollspy. Why anyone would want these components to be incompatible with one another is beyond me. After more than 32 hours of research, trial, and error, I found only one option that was effective: the Double Backanchor hack, aka using duplicate IDs in quick succession. Duplicating IDs is a big no-no in HTML, but extensive testing indicated no negative effect on the site. As such, I pushed this fix. Maybe that's sloppy of me, but I'm done dying on this ridiculous hill.</li>
<li> [Update on an Outstanding Issue from the last patch notes]: The issue of scrollspy not updating correctly when the user navigates via the navbar dropdown has been fixed! It was deeply interconnected with the navbar issue described above, and it was ultimately rectified somewhere along the way. I fixed it a few different ways, but none of them were compatible with the Double Backanchor hack. Fortunately, fixing the root problem behind the low-fidelity navbar auto-resolved this issue. (That "root problem" had something to do with scrollspy not counting the sticky navbar's height when measuring section length, if I recall.)</li>
<li> Navbar links no longer get larger when the user hovers over them. This feature was a casualty of the battle against the scrollspy and its bad counting; trying to fix the scrollspy when elements were also changing heights on the fly was a bridge too far for a developer of my caliber.</li>
<li> Most navbar elements have been reverted back to center alignment. I implemented left alignment last patch because I didn't like how the dropdown items looked center-aligned. However, I eventually realized that I could just have the dropdown items align left and everything else align center, so that's what I did! Center alignment works much better for visual balance when in desktop mode~</li>
<li> Chadsworth the Hippo is now better aligned with and more responsive to the other items in the navbar.</li>
</ul>
<h3>Dark Mode/Light Mode & Toggle Button</h3>
<ul><li> Fixed a strange error whereby first-time visitors to the site (or those who had just cleared their browser history) whose web browsers are set to force light mode would end up in a weird hybrid state; some elements would load in light mode, some would load in dark mode, and the site would stay half-and-half until the user both used the toggle button and refreshed the page. As a LibreWolf user, I was pretty embarrassed that I didn't catch this one sooner. On the bright side (pun intended), this forced me to revisit the code for dark mode and light mode, which was pretty awful. That code (CSS and JavaScript) has now been greatly simplified and streamlined.</li>
<li> The color palettes of both dark mode and light mode have been simplified; they now feature fewer colors and more consistent color-coding.</li>
<li> The light mode color palette has also been rebalanced to make links show up better against the light background. Feedback on this new balance is always welcome!</li>
</ul>
<h3>Header & Title Plate</h3>
<ul><li> Restored Jason's legacy -webkit gradient background.</li>
<li> Replaced the &lth5&gt elements serving as subtitles with previously-unutilized &lth3&gt elements to free up the &lth5&gt elements for in-body titles.</li>
<li> Created specific font size and color variables for the new &lth3&gt subtitles.</li>
<li> Slightly rebalanced the font size and color of the subtitles to increase legibility.</li>
</ul>
<h3>Censor</h3>
<ul><li> The upsetting content censor has been reworked from the ground up. While I was proud of my former implementation of it, it didn't really add much as a feature. If anything, all the asterisks only drew <i>more</i> attention to the words it was supposed to be "hiding."</li>
<li> As such, all asterisk censoring has been removed from the site. Common words that are firmly embedded in the subject matter of this website, like "abuse" and "violence," are now permanently uncensored.</li>
<li> Many of the more potent former censor words, such as ||"suicide," "rape," and "sexual assault"|| have been addressed at the root: their presence on this website in the first place. In most cases, it was easy to write around them or use less loaded language, preempting much of the need for censoring.</li>
<li> A new censor has been implemented to cover cases where the more potent former censor words <i>are</i> necessary to invoke. This censor works smarter rather than harder; organizations with potent words in their names are now listed by their acronym, with their full name appearing in parenthesis. When applied, the censor takes advantage of this inversion to hide the entire parenthetical.</li>
<li> Instead of hiding all instances of a certain word with no regard for context, the censor now targets only specially-marked words and passages and removing them seamlessly (i.e., leaving no sign that there had ever been additional content at all). Most of these cases involve organizations providing laundry lists of upsetting things that they can help with when an umbrella term or two would offer a negligible semantic trade-off. Likewise, potent words repeated over and over again, sentence after sentence, will see the first mention left visible but any repetitions hidden and subverted.</li>
<li> I've taken care to ensure that the new censor doesn't substantively alter the meaning of text it modifies, so this system should offer a good balance of semantic fidelity and frictionless protection from some of the website's more evocative words.</li>
<li> As before, the censor can be turned on and off as many times as the user desires.</li>
<li> I still call this feature "the censor" for the sake of clarity and consistency, but the <i>word</i> "censor" has been removed from all user-facing copy, including the censor button itself. I made this change in light of the current, tempestuous climate surrounding free speech and censorship the world over. Conflating content advisories and trigger warnings with censorship is misleading and liable to deflate the potency of the word "censorship" itself. This concern might be a touch granular, especially given the context, but I've never been one for apathy or <i>laissez-faire</i> communication.</li>
</ul>
<h3>Welcome Section (aka Hey There Section)</h3>
<ul><li> Restored Jason's legacy -webkit gradient border to its rightful place around this subsection.</li>
<li> Updated, consolidated, edited, and otherwise improved the original copy of this section.</li>
<li> Added an example of a blue link (aka "resource link") in-line. The example link isn't clickable, and it doesn't actually link to anything.</li>
<li> Added new copy explaining how privacy-minded folks can easily flush their phones' DNS cache.</li>
<li> Added new copy featuring warnings, disclaimers, and a reminder that nothing on this website or its peripheral media constitutes "advice" of any kind.</li>
<li> Increased the visibility of the "If your life is in immediate danger" warning by setting it off from the copy and adding an &lth5&gt element as a mini-title.</li>
</ul>
<h3>The Find Support Section & The Learn Section — New Resources/Hotlines</h3>
<ul><li> Added Vet Centers Readjustment Counseling under the Veterans subsection.</li>
</ul>
<h3>The Find Support Section & The Learn Section — Moved Resources/Hotlines</h3>
<ul><li> 211.org has been moved from the Learn section to the General subsection to reflect that it is a hotline, not just a set of resources.</li>
<li> MindWise Innovations has been moved from the Veterans subsection due to a rebrand. I couldn't find their old screeners for Veterans, and their focus has clearly broadened into more of a resource library. This makes them ideal for placement in the "Learn" section.</li>
<li> Various resources have been rearranged within their subsections.</li>
</ul>
<h3>The Find Support Section & The Learn Section — Resource/Hotline Updates</h3>
<ul><li> Updated the list of hotlines offered by Vibrant Emotional Health in the General subsection to reflect their current options.</li>
<li> Updated Crisis Text Line in the General subsection to reflect its ability to operate in Puerto Rico, as well as some changes to the keywords used to start a conversation (Text "Home" -> Text "CONNECT"/"SHOUT") in Canada & the U.K. respectively.</li>
<li> Updated Befrienders Worldwide to reflect its unique support options for seafarers in international waters (or anywhere in the world, really).</li>
<li> "Mental Health Hotlines in Every Country" in the General subsection has been renamed to "Mental Health Hotlines Around the World" to reflect the fact that this resource doesn't list hotlines for "<i>every</i> country."</li>
<li> "Substance Abuse and Mental Health Services Administration (SAMHSA) Helpline" in the Substance Abuse subsection has had "Helpline" removed from its name to reflect the fact that it has substantially more offerings also available.</li>
<li> Added a note to Substance Abuse and Mental Health Services Administration (SAMHSA) to disclose that it's a branch of the U.S. federal government's Department of Health & Human Services, currently headed by Secretary Robert F.</li> Kennedy, Jr.</li>
<li> Updated Contra Costa Health in the Substance Abuse subsection to clarify that it only serves Contra Costa County in California, U.S.A.</li>
<li> The National Association of Anorexia Nervosa and Associated Disorders in the Eating Disorders subsection is now listed as "ANAD," with its full name in parenthesis beside it. This seems to be in line with that organization's current approach to branding.</li>
<li> "National Eating Disorders Association" in the Eating Disorders subsection has had "(NEDA)" added on to the end of its name to reflect the ongoing, prevalent usage of that nickname. This seems to be in line with that organization's current approach to branding, too.</li>
<li> The Rape, Abuse, & Incest National Network in the Domestic & Sexual Violence subsection is now listed as "RAINN," with its full name in parenthesis beside it. This seems to be in line with that organization's current approach to branding.</li>
<li> Updated Pathways to Safety International in the Domestic & Sexual Violence subsection to reflect that its international hotline is temporarily closed due to a loss of funding from the U.S. federal government.</li>
<li> Nullified the Pathways to Safety International Phone link to avoid any confusion. The number itself is still present, just as white text rather than a blue link.</li>
<li> "National Runaway Safeline" in the Child Abuse & Trafficking subsection has had "(1800 Runaway)" added on to the end of its name to reflect the ongoing, prevalent usage of that nickname. This seems to be in line with that organization's current approach to branding, too.</li>
<li> Added a note to National Runaway Safeline (1800 Runaway) to disclose that its forums aren't moderated in real time and shouldn't be used in emergencies.</li>
<li> Added a note to ChildHelp National Child Abuse Hotline in the Child Abuse & Trafficking subsection to clarify that it's for crisis counseling pertaining to child abuse, not for <i>reporting</i> child abuse.</li>
<li> "Rethink.org" in the Learn section has been renamed to "Rethink Mental Illness (Rethink.org)" to reflect its full name.</li>
<li> Updated Rethink Mental Illness (Rethink.org) to clarify that it operates in England.</li>
<li> "MindWise Innovations" in the Learn section has been renamed to "MindWise Library: The Behavioral Health Beat" to reflect its rebrand.</li>
</ul>
<h3>The Find a Therapist Section</h3>
<ul><li> Improved the scalability of the Find a Therapist options, allowing them to better utilize the space.</li>
<li> Simplified the color scheme of the Find a Therapist options.</li>
<li> Made the "Visit!" buttons on the Find a Therapist options a little larger to make them easier to press on mobile.</li>
<li> "Rise Above the Disorder" has had "(RAD)" added on to the end of its name to reflect the ongoing, prevalent usage of that nickname. This seems to be in line with that organization's current approach to branding.</li>
<li> "American Psychological Association" has been renamed to "The American Psychological Association (APA)" in the interest of completeness.</li>
</ul>
<h3>The About Emma Section</h3>
<ul><li> Biographical information about Emma has been revised to reflect new developments since the last site update was deployed.</li>
<li> Removed the listing of Emma's usual Twitch streaming hours to reflect the fact that Emma isn't currently streaming on a regular schedule.</li>
<li> Removed all social media icons and links except for one link due to privacy concerns on Cassie's end. The remaining link is small and strategically placed, ensuring that people who sincerely do wish to follow Emma's advocacy have a chance to do so.</li>
<li> Much of the style framework that once supported the social media icons has been left intact in the code; I preserved as much of it as I could amidst the other changes.</li>
</ul>
<h3>Footer</h3>
<ul><li> Updated the "copyright" information to include "2026."</li>
<li> Now that Cassie has researched and compiled all information in this site by her own hand, the sites credits have been adjusted to indicate that Emma and Cassie are the site's only two creators and "owners."</li>
<li> Added Jason's name to the credits...for the first time!? This one's Cassie's fault. My apologies to Jason for the long-term oversight.</li>
<li> Adjusted the link to this repository page so that it will open in a new tab rather than in the user's current tab.</li>
<li> Adjusted the Email us! link to reflect that Cassie's "cassaleatory" email address has switched from "@gmail.com" to "@proton.me."</li>
<li> Added some requests for bug reports alongside the request for [users to report] out-of-date information.</li>
<li> [Update on an Outstanding Issue from the last patch notes]: The legibility problem affecting visited links in the footer was auto-resolved when :visited styles for <i>all</i> links were deprecated in this update.</li>
</ul>
<h3>Copy</h3>
<ul><li> Fixed a handful of typos in resource links or their text. While this issue was small in scale, it's of considerably greater severity—I apologize for not catching these sooner.</li>
<li> Replaced vague identifiers like "the nation" or "the country" with the name of the specific nation or country in question (usually the United States).</li>
<li> Fixed questionable syntax, several semantics errors, and various typos (encompassing both words and grammar) across the site.</li>
</ul>
<h3>Code</h3>
<ul><li> Updated the site to Bootstrap 5.1.3 CSS & Javascript.</li>
<li> Linked in jQuery 3.7.1 for a few new JavaScript features.</li>
<li> Simplified and greatly improved some unnecessary-complex and accident-prone code in both CSS & Javascript pertaining to dark mode/light mode and the censor.</li>
<li> Improved the code's commenting, especially in the JavaScript section.</li>
<li> Improved the code's overall legibility.</li>
<li> Implemented a more intuitive organization and grouping system in the site's custom CSS stylesheet.</li>
<li> Cleaned up the code by clearing out some leftover components for old, long-deprecated features.</li>
<li> Fixed a sprawling assortment of miscellaneous bugs, formatting errors, and other oversights.</li>
</ul>
<hr>
<h2>On The Future</h2>
<hr>
<h3>Outstanding Issues</h3>
<ul><li> No outstanding issues have been identified yet! This section will be updated if any issues are found or reported.</li>
</ul>
<h3>Privacy</h3>
<ul><li> [Update on an Outstanding Issue from the last patch notes]: Last time, Cassie was "planning to look into cookies," albeit in a very limited and qualified sense. She said, quite wisely, that "protecting user privacy is both an ethical obligation and an imperative step in ensuring that information on an array of sensitive mental health concerns can be safely accessed by everyone who needs it." A statement like this begs the question, "why bother with cookies in the first place?" Cassie had no satisfactory answer to that question.</li>
<li> [Outstanding issue, cont.]: In addition to not contributing to privacy, cookies tend to actively compromise it. And what benefit would they provide to a website like this one in return? The only thing included on this site that might make sense to track across sessions is the user's dark mode/light mode preference, but that can just as easily be obtained by checking the user's system preference—no local data storage required. For the sake of accomplishing her stretch goal, Cassie <i>did</i> manage to make a persistent cookie to store this preference. She tested it out and it worked! Her stretch goal was complete, and she was very proud of herself~</li>
<li> [Outstanding issue, cont.]: Are you beginning to see what's going on here? The goal of exploring was never <i>really</i> about improving the website; it was about improving Cassie's skills as a web developer. There's not anything wrong with adding that extra layer of challenge, but at the end of the day, the site needs to reflect the needs of its users above all else. So, Cassie commented out the cookie and left it [inoperable but] otherwise intact in the JavaScript, where it remains to this day.</li>
<li> [Outstanding issue, cont.]: Maybe, in another time, it would've been fun to keep experimenting with cookies and see if I could design something that <i>would</i> serve this site's users. But I lack the knowledge and experience to do that, and with today's digital privacy landscape looking so bleak, the project no longer holds any appeal. Therefore, that lone, deactivated cookie will be both the first and last of its kind on this website.</li>
<li> I'll end this section with a reiteration of an old promise: this website hasn't explored tracking cookies, personal data collection, advertisements, or monetization, nor will it ever. You Matter to Me exists for but one purpose: to help everyone who needs it as best as it can. It doesn't need any of that other stuff to complete its mission.</li>
</ul>
<h3>AI</h3>
<ul><li> This website was researched, designed, coded, and...<i>everything else</i>... without the use of large language models or other generative AI.</li>
<li> There have been some heartrending stories about the use and misuse of AI in the mental health world, so in case anyone's concerned, I promise that this website will always be built and maintained by humans alone, and that it won't be offering any AI features or "services" to users, either.</li>
<li> I don't make these promises to assign an implicit moral judgment to the existence or use of these AI tools—in fact, I hope they continue to grow in their ability to help people. However, mental health isn't a "game," or a "challenge," or a "use case." The unofficial Silicon Valley ethos of "move fast and break things" is not acceptable when the "things" that stand to be broken are vulnerable human beings. Some things need a softer touch, and mental health is one of them. That's why I'm so adamant on keeping You Matter to Me "for humans by humans."</li>
</ul>
<h3>So, What's Next?</h3>
<ul><li> It's time to rest for a while. Cassie's been hard at work on a great many things for a long time now, so she's in no rush to subvert opportunities for closure. That's a fancy way of saying that no new updates or features are on the horizon for now.</li>
<li> Now that all of the erstwhile Outstanding Issues have been cleared, Cassie will try her best to be on top of any new ones that might pop up. She intends to address them as they're reported rather than letting a new heap of them pile up. So, you might notice small, targeted patches every now and again.</li>
<li> Should the day ever come when Emma or Cassie have new big ideas for You Matter to Me, expect this section to be updated with some hints about what's to come well ahead of any major update.</li>
<li> Until then, we look forward to keeping You Matter to Me up and running for a long time to come. \<3</li>
</ul>
<hr>
<p>Thanks for reading~ If the You Matter to Me website, its Github repository, or these patch notes have given you $5's worth of value today, please consider taking that $5 and spending it on yourself—self-love ain't selfish!</p>
<p>If you happen to catch any other errors in either the website or its information, or if you have other suggestions for improvement, please reach out to Cassie at <a href="mailto:cassaleatory@proton.me" target="_blank">cassaleatory@proton.me</a>.</p>
<hr>
<p>Patch notes written by Cass Aleatory.</p>
