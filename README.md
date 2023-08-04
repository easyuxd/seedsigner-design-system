# SeedSigner Design System

### Contents:

* [Overview](#overview)
	- [Design Goals](#design-goals)
	- [Proposed Enhancements](#proposed-enhancements)
* [Key Performance Indicators](#key-performance-indicators)
* [Design System](#design-system)
	- [Measurements](#measurements)
	- [Typography](#typography)
	- [Color Palette](#color-palette)
	- [Layouts](#layouts)
	- [Components](#components)
	- [Icons](#iconography)
	- [Interactions](#interactions)
* [Content Strategy](#content-strategy)
	- [IA Best Practices](#ia-best-practices)


---


## Overview

![Main Menu](images/main-menu.png)

A modern, user-friendly GUI to make the SeedSigner software interface more accessible to non-technical users.

### Design Goals:

* **Visual Design:** Improve aesthetics and provide visual aids using UI treatments and iconography.
* **Interaction Design:** Increase overall efficiency of user inputs and feedback.
* **Information Architecture:** Improve findability by organizing and surfacing common tasks.
* **Content Design:** Simplify language to make abstract concepts more accessible to the average user.

### Proposed Enhancements:

* **Navigation:** Add Navigation Bar for context of location and easier access to global navigation functions
* **IA:** Accessible groupings of features, surface high-traffic actions
* **Content:** Simplify labels for viewport optimization and localization
* **Visual:** Add iconography to reduce cognitive load and aid localization
* **Visual:** Change font to a more legible but space-efficient typeface


---


## Key Performance Indicators

* **Efficiency** - Speed (less time/taps, more efficient paths)
	- Minimize button presses
	- More information with less scrolling
	- Predictable interactions and placement
* **Findability** 
	- Context of location (clear labeling, titles)
	- Menu IA (card sorting, tree testing)
* **Overall Satisfaction** (qualitative)
	- Ease-of-use
* **Project Success Measures**
	- Enclosure and pre-built device sales
	- Social media engagement
	- Increased awareness to targeted features
	- Reduction in support requests / complaints for targeted pain points


---


## Design System

**Prototype (WIP):** [Figma Prototype](#)
- Arrow keys to navigate
- Space to select

**Design File:** [Figma](https://www.figma.com/file/YCvGdWbyhxPrYqxk8gZWuA/SeedSigner)


## Measurements

**Standard Measurements (8px Grid System):**

- 4px
- 8px
- 12px
- 16px
- 24px
- 32px
- 64px

**Notes:**
- 8px margins maintained around layouts (224px usable space).
- 8px minumum padding between UI elements (when possible).
- Buttons/targets should be a minimum of 24px for legibility.



## Typography
 
![Typography](images/typography.png)
  
*All typography uses the Open Sans font family and follows a set of type styles, each with an associated font size (px), line height (px), and font weight.*
  
**Type Styles:**

- **Title:** 18px / 22 lh (Bold)
- **Menu Label:** 16px / 20 lh (Bold)
- **Button Large:** 18px / 22 lh (SemiBold)
- **Button:** 17px / 22 lh (SemiBold)
- **Heading** 17px / 22 lh (SemiBold)
- **Body Strong:** 17px / 22 lh (SemiBold)
- **Body:** 17px / 22 lh (Regular)
- **Body Small:** 16px / 20 lh (SemiBold)
- **Caption:** 14px / 18 lh (SemiBold)


## Color Palette
 
![Color Palette](images/color-palette.png)
  
*The SeedSigner color palette is designed for a 'dark mode' interface.*
  
*Light text/images on a dark background provide adequate contrast, while color should be used sparingly in messaging or iconography when applicable.*
  
![Background](images/colors/swatch-background.svg) **Background:** #0A0A0A

![Container](images/colors/swatch-container.svg) **Container:** #2C2C2C

![Container - Disabled](images/colors/swatch-container.svg) **Container (Disabled):** #2C2C2C, 70%
  
![Primary](images/colors/swatch-primary.svg) **Primary:** #FCFCFC
  
![Secondary](images/colors/swatch-secondary.svg) **Secondary:** #FCFCFC, 70%
  
![Active](images/colors/swatch-active.svg) **Active:** #FF9F0A
  
![Informational](images/colors/swatch-informational.svg) **Informational:** #0084FF
  
![Success](images/colors/swatch-success.svg) **Success:** #30D158
  
![Warning](images/colors/swatch-warning.svg) **Warning:** #FFD60A
  
![Error](images/colors/swatch-error.svg) **Error:** #FF453A



## Layouts
 
![Layouts](images/layouts.png)

### Overview:

- Navbar present on all screens.
- Content area begins directly below Navbar.
 
![Layout Overview](images/layouts/overview.png)
 
 
### Menus:

- Grid Menu
- List Menu
 
![Grid Menu](images/layouts/grid-menu.png)
 
![List Menu](images/layouts/list-menu.png)
 
 
### Dialogs:

Variants:
- 1-button
- 2-button
- 3-button*

![Dialogs](images/layouts/dialog.png)
 
 
### Informational:

Variants:
- Transaction Details
- XPUB Details
 
![Informational](images/layouts/informational.png)
 
 
### Word List:

![Word List](images/layouts/word-list.png)
 
 
### Messaging:

Variants:
- Confirmation
- Warning
- Error
 
![Messaging](images/layouts/messaging.png)
 
 
### Input:

- Word Input
- Keyboard Input (Passphrase, Derivation, etc.)
- Dice Input
 
![Input](images/layouts/input.png)
 

### Capture Photo:
 
![Capture Photo](images/layouts/photo.png)
 
 
### Transcribe QR:

![Transcribe QR](images/layouts/transcribe-qr.png)
 
 
## Components

![Components](images/components.png)
  
*Components are reusable building blocks that are aggregated to compose a screen layout, with each component serving a specific function.*

### Navigation Bar (240x48)

*Usage: Included on every screen, fixed to top of viewport.*

*All elements within the Navigation Bar are conditional. Titles should always be included when possible.*

![Navigation Bar](images/components/navbar.png)
  
Anatomy:
- Back Arrow (Medium Button)
- Title (13 character max)
- Action Button (Medium Button)
- Down Arrow (For pagination, displayed when scroll-up is available)
  
![Navigation Bar - Redlines](images/components/navbar-redlines.png)
  
Variants:
- Standard
- Transparent (no title)


### Grid Item (108x80)

![Grid Item](images/components/grid.png)
  
Anatomy:
- Contains: Icon (40x40)
- Label (10 character max)
  
![Grid Item - Redlines](images/components/grid-redlines.png)
  
States:
- Default
- Active
- Disabled


### List Item (224x32)

![List Item](images/components/list.png)
  
States:
- Default
- Active
- Disabled
- First
- Last
  
![List Item - Redlines](images/components/list-redlines.png)
  
Variants:
- Left Text
- Left Text w/ Chevron
- Left Text w/ Icon
- Left + Right Text
- Left + Right Text w/ Icon


### CTAs

*Usage: Set of buttons allowing for selection from 1-3 options. Fixed to bottom of viewport.*
  
![CTAs](images/components/ctas.png)
  
Variants:
- 1-Button (224x32)
- 2-Button (224x72)
- 3-Button (224x112)
- 2-up (224x32)
  
![CTAs - Redlines](images/components/ctas-redlines.png)


### Buttons

#### Large Button (224x32):

*Usage: Call-to-action*
  
![Large Button](images/components/button-large.png)
  
Sizes:
- Standard (100% width)
- 2-up (50% width)
  
States:
- Default
- Active
- Disabled
- Alert
  
![Large Button - Redlines](images/components/button-large-redlines.png)
  
Variants:
- Text only
- Text w/ Icon


#### Medium Button (32x32)

*Usage: General, Navigation Bar*
  
![Medium Button](images/components/button-medium.png)
  
States:
- Default
- Active
- Disabled
  
![Medium Button - Redlines](images/components/button-medium-redlines.png)


#### Small Button (24x24)

*Usage: Floating Action Buttons (icon), Keyboard Keys*
  
![Small Button](images/components/button-small.png)
  
States:
- Default
- Active
- Disabled
  
![Small Button - Redlines](images/components/button-small-redlines.png)


#### Flyout Button (48x24)

*Usage: Floating Action Buttons (text)*
  
![Flyout Button](images/components/button-flyout.png)
  
States:
- Default
- Active
- Disabled
  
![Flyout Button - Redlines](images/components/button-flyout-redlines.png)


#### Word Input Button (64x24)

*Usage: Word Entry UI*
  
![Word Input](images/components/button-word.png)
  
States:
- Default
- Active
  
![Word Input - Redlines](images/components/button-word-redlines.png)


#### Dice Input Button (64x64)

*Usage: Dice Entry UI*
  
![Dice Input](images/components/button-dice.png)
  
States:
- Default
- Active
  
![Dice Input - Redlines](images/components/button-dice-redlines.png)


### Input Field (64x24)

*Usage: Passphrase Entry, Derivation Entry*
  
![Input Field](images/components/input-field.png)
  
![Input Field - Redlines](images/components/input-field-redlines.png)


### Word List (108x20)

*Usage: View/Review Seed Words*
  
![Word List](images/components/word-list.png)
  
![Word List - Redlines](images/components/word-list-redlines.png)


### Table

*Usage: Informational screens*
  
![Table](images/components/table.png)
  
Variants:
- 1-row (224x40)
- 2-row (224x60)
- 3-row (224x80)
  
![Table - Redlines](images/components/table-redlines.png)


### Messaging

*Usage: Contextual overlays. Does not interrupt experience.*
  
![Messaging](images/components/messaging.png)
  
Messaging Types:
- Default
- Success
- Warning
- Error
  
![Messaging - Redlines](images/components/messaging-redlines.png)
  
Variants:
- No Subtitle (224x48)
- Subtitle (224x60)


## Iconography

***Work-in-progress:** Some iconography uses the [FontAwesome](https://fontawesome.com/) icon library, denoted by an asterisk.*

### Menu:

[Scan](images/icons/01-menu/scan.svg) _(40x40)_  
<img src="images/icons/01-menu/scan.svg" alt="icon-scan" width="40" height="40"/>  
  
[Seeds](images/icons/01-menu/seeds.svg) _(40x40)_  
<img src="images/icons/01-menu/seeds.svg" alt="icon-seeds" width="40" height="40"/>  
  
[Settings](images/icons/01-menu/settings.svg) _(40x40)_  
<img src="images/icons/01-menu/settings.svg" alt="icon-settings" width="40" height="40"/> 

[Tools](images/icons/01-menu/tools.svg) _(40x40)_  
<img src="images/icons/01-menu/tools.svg" alt="icon-tools" width="40" height="40"/> 

### Utility:

[Back](images/icons/02-utility/back.svg) _(24x24)_  
<img src="images/icons/02-utility/back.svg" alt="icon-back" width="24" height="24"/>  
  
[Chevron Down](images/icons/02-utility/chevron-down.svg) _(24x24)_  
<img src="images/icons/02-utility/chevron-down.svg" alt="icon-chevron-down" width="24" height="24"/>  
  
[Chevron Left](images/icons/02-utility/chevron-left.svg) _(24x24)_  
<img src="images/icons/02-utility/chevron-left.svg" alt="icon-chevron-left" width="24" height="24"/>  
  
[Chevron Right](images/icons/02-utility/chevron-right.svg) _(24x24)_  
<img src="images/icons/02-utility/chevron-right.svg" alt="icon-chevron-right" width="24" height="24"/>  
  
[Chevron Up](images/icons/02-utility/chevron-up.svg) _(24x24)_  
<img src="images/icons/02-utility/chevron-up.svg" alt="icon-chevron-up" width="24" height="24"/>  
  
[Close](images/icons/02-utility/close.svg) _(24x24)_  
<img src="images/icons/02-utility/close.svg" alt="icon-close" width="24" height="24"/>  

[Page Down](images/icons/02-utility/page-down.svg) _(16x8)_  
<img src="images/icons/02-utility/page-down.svg" alt="icon-page-down" width="16" height="8"/>  
  
[Page Up](images/icons/02-utility/page-up.svg) _(16x8)_  
<img src="images/icons/02-utility/page-up.svg" alt="icon-page-up" width="16" height="8"/>  
  
[Plus](images/icons/02-utility/plus.svg) _(24x24)_  
<img src="images/icons/02-utility/plus.svg" alt="icon-plus" width="24" height="24"/>  
  
[Power](images/icons/02-utility/power.svg) _(24x24)_  
<img src="images/icons/02-utility/power.svg" alt="icon-power" width="24" height="24"/>  

### Messaging:

[Error](images/icons/03-messaging/error.svg) _(40x40)_  
<img src="images/icons/03-messaging/error.svg" alt="icon-error" width="40" height="40"/>
  
[Success](images/icons/03-messaging/success.svg) _(40x40)_  
<img src="images/icons/03-messaging/success.svg" alt="icon-success" width="40" height="40"/>  
  
[Warning](images/icons/03-messaging/warning.svg) _(40x40)_  
<img src="images/icons/03-messaging/warning.svg" alt="icon-warning" width="40" height="40"/>    

### Informational:

[Address](images/icons/04-info/address.svg) _(24x24)_  
<img src="images/icons/04-info/address.svg" alt="icon-address" width="24" height="24"/>  
  
[Change](images/icons/04-info/change.svg) _(24x24)_  
<img src="images/icons/04-info/change.svg" alt="icon-change" width="24" height="24"/>  
  
[Derivation](images/icons/04-info/derivation.svg) _(24x24)_  
<img src="images/icons/04-info/derivation.svg" alt="icon-derivation" width="24" height="24"/>  
  
[Fee](images/icons/04-info/fee.svg) _(24x24)_  
<img src="images/icons/04-info/fee.svg" alt="icon-fee" width="24" height="24"/>  
  
[Fingerprint](images/icons/04-info/fingerprint.svg) _(24x24)_  
<img src="images/icons/04-info/fingerprint.svg" alt="icon-fingerprint" width="24" height="24"/>  
  
[Passphrase](images/icons/04-info/passphrase.svg) _(24x24)_  
<img src="images/icons/04-info/passphrase.svg" alt="icon-passphrase" width="24" height="24"/>  
  
### Misc:

[Bitcoin](images/icons/05-misc/bitcoin.svg) _(24x24)_  
<img src="images/icons/05-misc/bitcoin.svg" alt="icon-bitcoin" width="24" height="24"/>  
  
[Bitcoin Alt](images/icons/05-misc/bitcoin-alt.svg) _(24x24)_  
<img src="images/icons/05-misc/bitcoin-alt.svg" alt="icon-bitcoin-alt" width="24" height="24"/> 
  
[Brightness](images/icons/05-misc/brightness.svg) _(24x24)_  
<img src="images/icons/05-misc/brightness.svg" alt="icon-brightness" width="24" height="24"/> 
  
[MicroSD](images/icons/05-misc/microsd.svg) _(24x24)_  
<img src="images/icons/05-misc/microsd.svg" alt="icon-microsd" width="24" height="24"/> 
  
[QR Code](images/icons/05-misc/qrcode.svg) _(24x24)_  
<img src="images/icons/05-misc/qrcode.svg" alt="icon-qrcode" width="24" height="24"/> 

### Outstanding Icons:

Single-Sig  
Multi-Sig  
Private Key 
XPUB 
Generate XPUB  
Generate Last Word  
Keyboard  
Dice  
Coinflip  
Wallet  
Network  
QR Code  
I/O Test  
Info  
Donate  
Save  
Available  
Unavailable  
More  
Scan QR Code  
Scan Image  
Loading Spinner  


## Interactions

#### Navigation:

- Next - Continue to next step
- Done - End of flow, return to entry point (non-destructive)
- OK/Close - Exit current screen (non-destructive)
- Cancel - End task and return to entry point (destructive)


---


## Content Strategy


### IA Best Practices:


### Clear and concise labeling

_Categories and labels should be clear and meaningful to users._
  
**Navigational labels should:**
- Make sense to all users, not just to advanced Bitcoin users
- Be concise -- maximum of 2 words if possible
- Only lead with an action verb when it's necessary for clarity
- Use "&"" instead of "and" for readability and space efficiency
- Meet users' expectations of what they'll find at a destination


### Intuitive groupings

_Like items should be clustered for enhanced discoverability._
  
**Navigational groupings should:**
- Meet user expectations (mental model)
- Consist of like items
- Adhere to cognitive load best practices
- Not have too many (or too few) items in a category


### Expected hierarchy

_The order of items should make sense and meet user expectations._
  
**Menu item hierarchy should:**
- Derive from user expectations
- Prioritize frequently-used and urgent tasks
- Leverage a common heirarchy of left-to-right or top-to-bottom based on frequency, urgency, and promoting awareness
- Utilize last position in a list (e.g. users expect Help/Contact near the bottom)


### Cognitive load control

_Decrease clutter that may confuse or distract users._
  
**To reduce cognitive load:**
- Limit the number of menus, categories, and items
- Avoid using a general category as a catch-all for orphan items
- Avoid visual clutter that may confuse or distract users


### Complementary contextual navigation

_When used, should align with the larger navigation ecosystem._
  
**Contextual navigation should:**
- Meet users' mental model for finding information and performing tasks
- Be easily visible and actionable
- Enhance but not duplicate the global navigation
- Create awareness of additional services/features


---


## Version History

**v0.1** __(2021-07-16)__
- Overview, design goals, proposed enhancements, preliminary design system
  
**v0.2** __(2021-09-14)__
- Table of contents, IA best practices, key performance indicators
  
**v0.3** __(2021-10-31)__
- Added layouts, added info tile and messaging components, updated color palette image, minor copy edits
  
**v0.4** __(2021-11-20)__
- Added typography, color palette, components

**v0.5** __(2022-02-11)__
- Added iconography (WIP)

**v0.6** __(2023-08-04)__
- Updated iconography
- Added Figma design file
- Updated usage for messaging overlay