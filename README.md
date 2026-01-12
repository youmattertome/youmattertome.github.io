[[____________________________________]]
[[ Most Recent Patch Notes: 1/11/2026 ]]
[[____________________________________]]

[[ Executive Summary (TL;DR) ]]

- [TO DO]

(( Please note that this is the long-awaited part two of a two-part update. Closure for all of part one's Outstanding Issues can be found below. For more on the future of the You Matter to Me project, please see "On The Future" at the end of these patch notes! ))

___________________________________________________________________________________
The Flagship Features of This Update
___________________________________________________________________________________

[[ Refreshed Copy & Content Modernization — Overview ]]
- [Update on an Outstanding Issue from the last patch notes]: You Matter to Me was first released in 2021, and its resources have long been overdue for some fact-checking and a refresh...until now! All sorts of changes have transpired since the departure of the site's original researcher (a third team member who worked with Emma and Cassie). Fortunately, Miss Professional Writing Major Cassie *also* knows a thing or two about researching and writing copy. As of the past few months, she's been on the road to recovery, allowing her to finally shoulder this task...and, as of 01/12/2026, complete it! 
- [Outstanding issue, cont.]: Cassie tackled this mission from the ground up, so it ended up being less of a fact-checking and more of a total relift for *all* of the resources in the Find Support and Learn sections. This section of the patch notes will cover the changes to how this site approaches copy. Changes to the resources themselves (hotlines closing, org renames, added considerations, etc.) can be found in the "Resource/Hotline Updates" section of "Other Changes in This Version" below. 

[[ Refreshed Copy & Content Modernization — Copy Layout ]]
- The scalability of the site has been improved. The mobile version feels a little less claustrophobic, and the desktop version won't get quite so sprawling and expansive as it could in the past.
- Removed the horizontal lines around section and subsection titles for a cleaner, more modern look.
- The buttons to expand and collapse resources have been moved from the righthand side of their section elements to the lefthand side, right next to their resource titles. This ensures the buttons remain fixed in place and directly adjacent to their corresponding resource titles on all screen sizes.
- The buttons to expand and collapse resources have been changed from plus signs ("+") to carats ("^")...or, technically, lowercase letter "v's." Each button rotates up 180 degrees when its resource is expanded and down 180 degrees when its resource is collapsed, providing a recognizable visual indicator of whether that resource is currently expanded or collapsed.
- Enlarged the "hitbox" of the buttons to expand and collapse resources to make them easier to click on mobile.
- Implemented the Clearfix hack to keep resource titles and subtitles neatly aligned to the right of their respective buttons regardless of screen size.

[[ Refreshed Copy & Content Modernization — Copy Approach & Standardization ]]
- Speaking of resource subtitles, this once-uncommon element is now ubiquitous across all resources in Find Support and Learn.
- [TO FINISH]

[[ Restored Legacy Content ]]
- [TO DO]

note: it's now 1am, i've been working on this site all day now and i need to sleep. log on again to finish this task right when i get up tomorrow morning...hope no one happens to check it in the eight hours it'll be sitting here half-done.
- c

v ISSUES FROM PART ONE UPDATE THAT STILL NEED CLOSURE WRITEUPS v
- Currently, most of the references to time have been translated to United States Pacific Time, the local time zone for this webpage, for consistency's sake. Going forward, we hope to have a feature that will standardize *all* references to time and give the user control over which time zone the website displays.

___________________________________________________________________________________
Other Changes in This Version
___________________________________________________________________________________

[[ Page Layout & Section Framework Changes ]]
- The "Learn About Mental Health" section has been renamed to "Learn & Grow" to reflect that the content there covers other facets of health and wellness in addition to mental health. For the sake of clarity, it will be referred to as the "Learn" section for the remainder of these patch notes.

[[ Navigation Bar ]]
- [Update on an Outstanding Issue from the last patch notes]: The fidelity of the navigation bar is finally fixed, and the sticky navbar no longer hides the heading of the section to which the user navigates. This comes after no small amount of effort on my part. Evidently, this is a whole 'thing' with Bootstrap; Bootstrap is aware of it and claiming it's an intentional effect of the interplay between sticky navbars, navlinks, and scrollspy. Why anyone would want these components to be incompatible with one another is beyond me. After more than 32 hours of research, trial, and error, I found only one option that was effective: the Double Backanchor hack, aka using duplicate IDs in quick succession. Duplicating IDs is a big no-no in HTML, but extensive testing indicated no negative effect on the site. As such, I pushed this fix. Maybe that's sloppy of me, but I'm done dying on this ridiculous hill.
- [Update on an Outstanding Issue from the last patch notes]: The issue of scrollspy not updating correctly when the user navigates via the navbar dropdown has been fixed! It was deeply interconnected with the navbar issue described above, and it was ultimately rectified somewhere along the way. I fixed it a few different ways, but none of them were compatible with the Double Backanchor hack. Fortunately, fixing the root problem behind the low-fidelity navbar auto-resolved this issue. (That "root problem" had something to do with scrollspy not counting the sticky navbar's height when measuring section length, if I recall.)
- Navbar links no longer get larger when the user hovers over them. This feature was a casualty of the battle against the scrollspy and its bad counting; trying to fix the scrollspy when elements were also changing heights on the fly was a bridge too far for someone of my ability.
- Most navbar elements have been reverted back to center alignment. I implemented left alignment last patch because I didn't like how the dropdown items looked center-aligned. However, I eventually realized that I could just have the dropdown items align left and everything else align center, so that's what I did! Center alignment works much better for visual balance when in desktop mode~
- Chadsworth the Hippo is now better aligned with and more responsive to the other items in the navbar.

[[ Dark Mode/Light Mode & Toggle Button ]]
- Fixed a strange error whereby first-time visitors to the site (or those who had just cleared their browser history) whose web browsers are set to force light mode would end up in a weird hybrid state; some elements would load in light mode, some would load in dark mode, and the site would stay half-and-half until the user both used the toggle button and refreshed the page. As a LibreWolf user, I was pretty embarrassed that I didn't catch this one sooner. On the bright side (pun intended), this forced me to revisit the code for dark mode and light mode, which was pretty awful. That code (CSS and JavaScript) has now been greatly simplified and streamlined.
- The color palettes of both dark mode and light mode have been simplified; they now feature fewer colors and more consistent color-coding.
- The light mode color palette has also been rebalanced to make links show up better against the light background. Feedback on this new balance is always welcome!

[[ Header & Title Plate ]]
- Restored Jason's legacy -webkit gradient background.
- Replaced the <h5> elements serving as subtitles with previously-unutilized <h3> elements to free up the <h5> elements for in-body titles.
- Created specific font size and color variables for the new <h3> subtitles.
- Slightly rebalanced the font size and color of the subtitles to increase legibility.

[[ Censor ]]
- The upsetting content censor has been reworked from the ground up. While I was proud of my former implementation of it, it didn't really add much as a feature. If anything, all the asterisks only drew *more* attention to the words it was supposed to be "hiding."
- As such, all asterisk censoring has been removed from the site. Common words that are firmly embedded in the subject matter of this website, like "abuse" and "violence," are now permanently uncensored.
- Many of the more potent former censor words, such as ||"suicide," "rape," and "sexual assault"|| have been addressed at the root: their presence on this website in the first place. In most cases, it was easy to write around them or use less loaded language, preempting much of the need for censoring.
- A new censor has been implemented to cover cases where the more potent former censor words *are* necessary to invoke. This censor works smarter rather than harder; organizations with potent words in their names are now listed by their acronym, with their full name appearing in parenthesis. When applied, the censor takes advantage of this inversion to hide the entire parenthetical.
- Instead of hiding all instances of a certain word with no regard for context, the censor now targets only specially-marked words and passages and removing them seamlessly (i.e., leaving no sign that there had ever been additional content at all). Most of these cases involve organizations providing laundry lists of upsetting things that they can help with when an umbrella term or two would offer a negligible semantic trade-off. Likewise, potent words repeated over and over again, sentence after sentence, will see the first mention left visible but any repetitions hidden and subverted.
- I've taken care to ensure that the new censor doesn't substantively alter the meaning of text it modifies, so this system should offer a good balance of semantic fidelity and frictionless protection from some of the website's more evocative words.
- As before, the censor can be turned on and off as many times as the user desires.
- I still call this feature "the censor" for the sake of clarity and consistency, but the *word* "censor" has been removed from all user-facing copy, including the censor button itself. I made this change in light of the current, tempestuous climate surrounding free speech and censorship the world over. Conflating content advisories and trigger warnings with censorship is misleading and liable to deflate the potency of the word "censorship" itself. This concern might be a touch granular, especially given the context, but I've never been one for apathy or *laissez-faire* communication.

[[ Welcome Section (aka Hey There Section) ]]
- Restored Jason's legacy -webkit gradient border to its rightful place around this subsection.
- Updated, consolidated, edited, and otherwise improved the original copy of this section.
- Added an example of a blue link (aka "resource link") in-line. The example link isn't clickable, and it doesn't actually link to anything.
- Added new copy explaining how privacy-minded folks can easily flush their phones' DNS cache.
- Added new copy featuring warnings, disclaimers, and a reminder that nothing on this website or its peripheral media constitutes "advice" of any kind.
- Increased the visibility of the "If your life is in immediate danger" warning by setting it off from the copy and adding an <h5> element as a mini-title.

[[ The Find Support Section & The Learn Section — New Resources/Hotlines ]]
- Added Vet Centers Readjustment Counseling under the Veterans subsection.

[[ The Find Support Section & The Learn Section — Moved Resources/Hotlines ]]
- 211.org has been moved from the Learn section to the General subsection to reflect that it is a hotline, not just a set of resources.
- MindWise Innovations has been moved from the Veterans subsection due to a rebrand. I couldn't find their old screeners for Veterans, and their focus has clearly broadened into more of a resource library. This makes them ideal for placement in the "Learn" section.
- Various resources have been rearranged within their subsections.
  
[[ The Find Support Section & The Learn Section — Resource/Hotline Updates ]]
- Updated the list of hotlines offered by Vibrant Emotional Health in the General subsection to reflect their current options.
- Updated Crisis Text Line in the General subsection to reflect its ability to operate in Puerto Rico and changes to the word to start a conversation (Text "Home" -> Text "CONNECT"/"SHOUT") in Canada & the U.K. 
- Updated Befrienders Worldwide to reflect its unique support options for seafarers in international waters (or anywhere in the world, really).
- "Mental Health Hotlines in Every Country" in the General subsection has been renamed to "Mental Health Hotlines Around the World" to reflect the fact that this resource doesn't list hotlines for "*every* country."
- "Substance Abuse and Mental Health Services Administration (SAMHSA) Helpline" in the Substance Abuse subsection has had "Helpline" removed from its name to reflect the fact that it has substantially more offerings also available.
- Added a note to Substance Abuse and Mental Health Services Administration (SAMHSA) to disclose that it's a branch of the U.S. federal government's Department of Health & Human Services, currently headed by Secretary Robert F. Kennedy, Jr.
- Updated Contra Costa Health in the Substance Abuse subsection to clarify that it only serves Contra Costa County in California, U.S.A.
- The National Association of Anorexia Nervosa and Associated Disorders in the Eating Disorders subsection is now listed as "ANAD," with its full name in parenthesis beside it.
- The Rape, Abuse, & Incest National Network in the Domestic & Sexual Violence subsection is now listed as "RAINN," with its full name in parenthesis beside it.
- Updated Pathways to Safety International in the Domestic & Sexual Violence subsection to reflect that its international hotline is temporarily closed due to a loss of funding from the U.S. federal government.
- Nullified the Pathways to Safety International Phone link to avoid any confusion. The number itself is still present, just as white text rather than a blue link.
- "National Runaway Safeline" in the Child Abuse & Trafficking subsection has had "(1800 Runaway)" added on to the end of its name to reflect the ongoing, prevalent usage of that nickname.
- Added a note to National Runaway Safeline (1800 Runaway) to disclose that its forums aren't moderated in real time and shouldn't be used in emergencies.
- Added a note to ChildHelp National Child Abuse Hotline in the Child Abuse & Trafficking subsection to clarify that it's for crisis counseling, not for reporting cases of child abuse.
- "Rethink.org" in the Learn section has been renamed to "Rethink Mental Illness (Rethink.org)" to reflect its full name.
- Updated Rethink Mental Illness (Rethink.org) to clarify that it operates in England.
- "MindWise Innovations" in the Learn section has been renamed to "MindWise Library: The Behavioral Health Beat" to reflect its rebrand.

[[ The Find a Therapist Section ]]
- Improved the scalability of the Find a Therapist options, allowing them to better utilize the space.
- Simplified the color scheme of the Find a Therapist options.

- All modes of communication, including Email, Live Chat, & WhatsApp, as well as one forum and one custom mobile app, are now consistently listed together with the Phone and Text options. Every contact option has a blue link or instructions.
- If hotlines that offer help in Spanish have different instructions or a different number to call for Spanish-language support, that information now has instructions and its own blue link.
  
[[ The About Emma Section ]]
- Biographical information about Emma has been revised to reflect new developments since the last site update was deployed.
- Removed the listing of Emma's usual Twitch streaming hours to reflect the fact that Emma isn't currently streaming on a regular schedule.
- Removed all social media icons and links except for one link due to privacy concerns on Cassie's end. The remaining link is small and strategically placed, ensuring that people who sincerely do wish to follow Emma's advocacy have a chance to do so.
- Much of the style framework that once supported the social media icons has been left intact in the code; I preserved as much of it as I could amidst the other changes.

[[ Footer ]]
- Updated the "copyright" information to include "2026."
- Now that Cassie has researched and compiled all information in this site by her own hand, the sites credits have been adjusted to indicate that Emma and Cassie are the site's only two creators and "owners."
- Added Jason's name to the credits...for the first time!? This one's Cassie's fault. My apologies to Jason for the long-term oversight.
- Adjusted the link to this repository page so that it will open in a new tab rather than in the user's current tab.
- Adjusted the Email us! link to reflect that Cassie's "cassaleatory" email address has switched from "@gmail.com" to "@proton.me."
- Added some requests for bug reports alongside the request for [users to report] out-of-date information.
- [Update on an Outstanding Issue from the last patch notes]: The legibility problem affecting visited links in the footer was auto-resolved when :visited styles for *all* links were deprecated in this update.

___________________________________________________________________________________
On The Future
___________________________________________________________________________________

[[ Outstanding Issues ]]
- No outstanding issues have been identified yet! This section will be updated if any issues are found or reported.

[[ Privacy ]]
- [Update on an Outstanding Issue from the last patch notes]: Last time, Cassie was "planning to look into cookies," albeit in a very limited and qualified sense. She said, quite wisely, that "protecting user privacy is both an ethical obligation and an imperative step in ensuring that information on an array of sensitive mental health concerns can be safely accessed by everyone who needs it." A statement like this begs the question, "why bother with cookies in the first place?" Cassie had no satisfactory answer to that question.
- [Outstanding issue, cont.]: In addition to not contributing to privacy, cookies tend to actively compromise it. And what benefit would they provide to a website like this one in return? The only thing included on this site that might make sense to track across sessions is the user's dark mode/light mode preference, but that can just as easily be obtained by checking the user's system preference—no local data storage required. For the sake of accomplishing her stretch goal, Cassie *did* manage to make a persistent cookie to store this preference. She tested it out and it worked! Her stretch goal was complete, and she was very proud of herself~
- [Outstanding issue, cont.]: Are you beginning to see what's going on here? The goal of exploring was never *really* about improving the website; it was about improving Cassie's skills as a web developer. There's not anything wrong with adding that extra layer of challenge, but at the end of the day, the site needs to reflect the needs of its users above all else. So, Cassie commented out the cookie and left it [inoperable but] otherwise intact in the JavaScript, where it remains to this day.
- [Outstanding issue, cont.]: Maybe, in another time, it would've been fun to keep experimenting with cookies and see if I could design something that *would* serve this site's users. But I lack the knowledge and experience to do that, and with today's digital privacy landscape looking so bleak, the project no longer holds any appeal. Therefore, that lone, deactivated cookie will be both the first and last of its kind on this website.
- I'll end this section with a reiteration of an old promise: this website hasn't explored tracking cookies, personal data collection, advertisements, or monetization, nor will it ever. You Matter to Me exists for but one purpose: to help everyone who needs it as best as it can. It doesn't need any of that other stuff to complete its mission.

[[ AI ]]
- This website was researched, designed, coded, and...*everything else*... without the use of large language models or other generative AI.
- There have been some heartrending stories about the use and misuse of AI in the mental health world, so in case anyone's concerned, I promise that this website will always be built and maintained by humans alone, and that it won't be offering any AI features or "services" to users, either.
- I don't make these promises to assign an implicit moral judgment to the existence or use of these AI tools—in fact, I hope they continue to grow in their ability to help people. However, mental health isn't a "game," or a "challenge," or a "use case." The unofficial Silicon Valley ethos of "move fast and break things" is not acceptable when the "things" that stand to be broken are vulnerable human beings. Some things need a softer touch, and mental health is one of them. That's why I'm so adamant on keeping You Matter to Me "for humans by humans."

[[ So, What's Next? ]]
- It's time to rest for a while. Cassie's been hard on work on a great many things for a long time now, so she's in no rush to subvert opportunities for closure. That's a fancy way of saying that no new updates or features are on the horizon for now.
- Now that all of the erstwhile Outstanding Issues have been cleared, Cassie will try her best to be on top of any new ones that might pop up. She intends to address them as they're reported rather than letting a new heap of them pile up. So, you might notice small, targeted patches every now and again.
- Should the day ever come when Emma or Cassie have new big ideas for You Matter to Me, expect this section to be updated with some hints about what's to come well ahead of any major update.
- Until then, we look forward to keeping You Matter to Me up and running for a long time to come. <3

___________________________________________________________________________________
Thanks for reading~ If the You Matter to Me website, its Github repository, or these patch notes have given you $5 worth of value today, please consider taking that $5 and spending it on yourself; self-love ain't selfish!

If you happen to catch any other errors in either the website or its information, or if you have other suggestions for improvement, please reach out to Cassie at cassaleatory@proton.me
___________________________________________________________________________________

Patch notes written by Cass Aleatory.
