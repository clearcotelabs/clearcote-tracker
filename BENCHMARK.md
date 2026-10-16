# Benchmark: 91 websites, 2 loads each, strict rules

**16 October 2026 · Clearcote hosted cloud browsers · every browser headless · two full runs on the same day**

A one-day measurement of how often a Clearcote hosted cloud browser gets the real page of 91 popular websites, under deliberately strict rules: every page loaded twice, logged out, in a fresh browser, with **30 seconds** to show the real page and **no clicks, no typing and no automatic help of any kind**. It is a snapshot of one day, not a promise about any website: sites change their pages often.

## Result

| Run | Real page served | Loads | 95% range | Leaving out loads our proxy could not connect |
| --- | :---: | :---: | :---: | :---: |
| Run 1 | **86.3%** | 157/182 | 81 to 91 | 92.4% (157/170, 87 to 95) |
| Run 2 | **85.2%** | 155/182 | 79 to 90 | 91.2% (155/170, 86 to 95) |

The range is the 95% Wilson interval. Every control page (five plain, unprotected websites) loaded in every run.

**Our own proxy.** Some of the misses are not the website turning the browser away. For six addresses (an airline home page and five sign-in pages) the default proxy pool behind the cloud browsers refuses to open the connection at all, so the browser shows its own "can't be reached" page and the site never receives the request. They count as misses above, the same as any other page that did not load. With your own proxy ([docs](https://www.clearcotelabs.com/docs/hosted-browsers)) those addresses go through a different network.

## By kind of website

| Kind | Websites | Run 1 | Run 2 |
| --- | :---: | :---: | :---: |
| Shopping | 22 | 41/44 | 41/44 |
| Travel & hotels | 15 | 28/30 | 26/30 |
| Tickets & events | 3 | 6/6 | 5/6 |
| Real estate & cars | 10 | 18/20 | 20/20 |
| News, finance & business | 10 | 19/20 | 19/20 |
| Jobs | 3 | 6/6 | 6/6 |
| Food delivery & Q&A | 3 | 6/6 | 6/6 |
| Log-in & sign-up pages (opened only) | 20 | 23/40 | 22/40 |
| Controls | 5 | 10/10 | 10/10 |

## Every website

Each cell is how many of that run's two loads got the real page.

### Shopping

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| academy.com | 2/2 ✅ | 2/2 ✅ |
| advanceautoparts.com | 2/2 ✅ | 2/2 ✅ |
| albertsons.com | 2/2 ✅ | 2/2 ✅ |
| autozone.com | 2/2 ✅ | 2/2 ✅ |
| bhphotovideo.com | 2/2 ✅ | 2/2 ✅ |
| costco.com | 2/2 ✅ | 2/2 ✅ |
| etsy.com | 2/2 ✅ | 2/2 ✅ |
| gap.com | 2/2 ✅ | 2/2 ✅ |
| harborfreight.com ² | 1/2 | 1/2 |
| homedepot.com | 2/2 ✅ | 2/2 ✅ |
| joann.com | 2/2 ✅ | 2/2 ✅ |
| kohls.com ² | 2/2 ✅ | 1/2 |
| macys.com | 2/2 ✅ | 2/2 ✅ |
| michaels.com | 2/2 ✅ | 2/2 ✅ |
| nike.com | 2/2 ✅ | 2/2 ✅ |
| petco.com | 2/2 ✅ | 2/2 ✅ |
| rei.com | 2/2 ✅ | 2/2 ✅ |
| sephora.com | 2/2 ✅ | 2/2 ✅ |
| staples.com | 2/2 ✅ | 2/2 ✅ |
| target.com | 2/2 ✅ | 2/2 ✅ |
| uniqlo.com ² | 0/2 | 1/2 |
| walmart.com | 2/2 ✅ | 2/2 ✅ |

### Travel & hotels

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| aa.com ¹ | 0/2 | 0/2 |
| booking.com | 2/2 ✅ | 2/2 ✅ |
| easyjet.com | 2/2 ✅ | 2/2 ✅ |
| enterprise.com | 2/2 ✅ | 2/2 ✅ |
| expedia.com | 2/2 ✅ | 2/2 ✅ |
| hertz.com | 2/2 ✅ | 2/2 ✅ |
| hotels.com | 2/2 ✅ | 2/2 ✅ |
| hyatt.com | 2/2 ✅ | 2/2 ✅ |
| kayak.com | 2/2 ✅ | 2/2 ✅ |
| lufthansa.com | 2/2 ✅ | 2/2 ✅ |
| marriott.com ² | 2/2 ✅ | 0/2 |
| norwegian.com | 2/2 ✅ | 2/2 ✅ |
| priceline.com | 2/2 ✅ | 2/2 ✅ |
| skyscanner.com | 2/2 ✅ | 2/2 ✅ |
| tripadvisor.com | 2/2 ✅ | 2/2 ✅ |

### Tickets & events

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| seatgeek.com ² | 2/2 ✅ | 1/2 |
| stubhub.com | 2/2 ✅ | 2/2 ✅ |
| viagogo.com | 2/2 ✅ | 2/2 ✅ |

### Real estate & cars

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| apartments.com | 2/2 ✅ | 2/2 ✅ |
| cars.com | 2/2 ✅ | 2/2 ✅ |
| copart.com | 2/2 ✅ | 2/2 ✅ |
| iaai.com | 2/2 ✅ | 2/2 ✅ |
| immobilienscout24.de ² | 0/2 | 2/2 ✅ |
| leboncoin.fr | 2/2 ✅ | 2/2 ✅ |
| redfin.com | 2/2 ✅ | 2/2 ✅ |
| truecar.com | 2/2 ✅ | 2/2 ✅ |
| zillow.com | 2/2 ✅ | 2/2 ✅ |
| zoopla.co.uk | 2/2 ✅ | 2/2 ✅ |

### News, finance & business

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| bloomberg.com ² | 1/2 | 1/2 |
| coinbase.com | 2/2 ✅ | 2/2 ✅ |
| economist.com | 2/2 ✅ | 2/2 ✅ |
| g2.com | 2/2 ✅ | 2/2 ✅ |
| nytimes.com | 2/2 ✅ | 2/2 ✅ |
| reuters.com | 2/2 ✅ | 2/2 ✅ |
| similarweb.com | 2/2 ✅ | 2/2 ✅ |
| t-mobile.com | 2/2 ✅ | 2/2 ✅ |
| vercel.com | 2/2 ✅ | 2/2 ✅ |
| wsj.com | 2/2 ✅ | 2/2 ✅ |

### Jobs

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| indeed.com | 2/2 ✅ | 2/2 ✅ |
| monster.com | 2/2 ✅ | 2/2 ✅ |
| ziprecruiter.com | 2/2 ✅ | 2/2 ✅ |

### Food delivery & Q&A

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| doordash.com | 2/2 ✅ | 2/2 ✅ |
| quora.com | 2/2 ✅ | 2/2 ✅ |
| ubereats.com | 2/2 ✅ | 2/2 ✅ |

### Log-in & sign-up pages (opened only)

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| Adobe sign-in ¹ | 0/2 | 0/2 |
| Bank of America sign-in ¹ | 0/2 | 0/2 |
| Battle.net log-in | 2/2 ✅ | 2/2 ✅ |
| Dropbox sign-up | 2/2 ✅ | 2/2 ✅ |
| EA log-in | 2/2 ✅ | 2/2 ✅ |
| Expedia log-in ² | 2/2 ✅ | 1/2 |
| GitHub sign-up ² | 0/2 | 0/2 |
| Hotels.com log-in | 2/2 ✅ | 2/2 ✅ |
| LinkedIn log-in | 2/2 ✅ | 2/2 ✅ |
| Microsoft account sign-up ¹ | 0/2 | 0/2 |
| OpenAI log-in | 2/2 ✅ | 2/2 ✅ |
| PayPal log-in ¹ | 0/2 | 0/2 |
| Roblox log-in | 2/2 ✅ | 2/2 ✅ |
| Snapchat sign-up | 2/2 ✅ | 2/2 ✅ |
| Sony sign-in ³ | 0/2 | 0/2 |
| Tinder | 2/2 ✅ | 2/2 ✅ |
| Twitch log-in | 2/2 ✅ | 2/2 ✅ |
| Uber Eats log-in ¹ | 0/2 | 0/2 |
| X sign-up ³ | 1/2 | 1/2 |
| Zillow log-in ² | 0/2 | 0/2 |

### Controls

| Website | Run 1 | Run 2 |
| --- | :---: | :---: |
| developer.mozilla.org | 2/2 ✅ | 2/2 ✅ |
| example.com | 2/2 ✅ | 2/2 ✅ |
| httpbin.org/html | 2/2 ✅ | 2/2 ✅ |
| iana.org/domains/reserved | 2/2 ✅ | 2/2 ✅ |
| wikipedia.org | 2/2 ✅ | 2/2 ✅ |

¹ Our default proxy could not connect to this address (the site never received the request).  
² The site showed a check or access page instead.  
³ The page stayed empty or showed the site's own error within 30 s.

## How it was run

- **One fresh cloud browser per load.** Every website was loaded twice per run, each time in a new hosted browser that was closed afterwards. Both runs used the same 91 addresses, in a different shuffled order, at most two browsers on one website at a time.
- **Default settings, every browser headless.** The hosted defaults, a US exit from the default proxy pool, no saved profile, no cookies carried over.
- **Load, then wait at most 30 seconds.** After opening the address the page was checked every 2 seconds until it showed real text and no check or access page, or until 30 seconds had passed since the navigation started.
- **No help.** No clicks, no typing, no press-and-hold. The cloud browser's automatic handling of on-page checks (checkbox, slider and press-and-hold) was switched **off** for every load, and the paid [challenge service](https://www.clearcotelabs.com/docs/cloud/challenges) was not used. The session logs confirm that no such action ran in any load.
- **Log-in and sign-up pages are only opened**, never filled in or submitted. Checks that some websites run only when a form is sent are therefore not part of this test.
- **One rule decides every load.** A load counts as served when the website's own page is showing, with real text and no check, access or error page in the way. The verdict comes from one set of rules applied to the saved page, title and status, and the screenshots were reviewed by hand; a check page in another language that the rules first missed was added as a rule before the final numbers.

These rules are stricter than the main list in the [README](README.md), which allows longer waits and the cloud browser's normal settings, so a website can be ✅ there and miss here.

---

<sub>Measured 16 October 2026. Only public pages were loaded: no accounts, no logins, no purchases, and no content from the websites is stored or published here. Not affiliated with any website listed. All trademarks belong to their owners. To have a website removed, see [Remove a website](README.md#remove-a-website).</sub>
