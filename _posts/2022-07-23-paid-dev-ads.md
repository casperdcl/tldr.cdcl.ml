---
title: Marketing to developers
src: https://www.developermarkepear.com/blog/paid-advertising-developer-marketing
categories: [Programming, Management, Industry, Communication]
tags: [opinionated, principles, product-research, tools-web, extra-long]
---

How to [target developers](#targeting-developers) (where traditional advertising often fails) & a [comparison of the ad channels/platforms](#channel-comparison).

## TL;DR for the TL;DR

> - choose goal
> - choose audience-appropriate platform
> - setup conservative targeting (better to under- than over-serve)
> - design [practical & relevant ads](https://www.moat.com)
> - :warning: connect to the right landing page, amplify paths people are already taking
> - run small tests before scaling ad spend

## Targeting developers

- most devs hate "traditional" (pop-ups, flashy colours) advertising
  + dev personality: sceptical, pragmatic, practical, "tribal" (trust other devs' expertise more than marketers')
- retargeting (ads follow users across sites) works well :heavy_check_mark: but requires analytics/tracking :stop_sign: [not great for devs](https://www.devmarketingguide.com)
  + maybe ok for late stage (consideration, activation, engagement, upgrades)
- paid ad campaign components:

1. **Goal**: desired reaction of [target (dev) audience](https://www.moesif.com/blog/developer-marketing/paid-ads/Best-Practices-for-Paid-Marketing-To-Developers)
   * e.g. tool **signups**, platform leads, etc.
   * if they don't yet need your tool, [build a memorable **brand**](https://www.notion.so/article/branding-developer-tools) so they remember you in future when they do need a tool
   * signups should **actually use** the tool -- follow up if not
   * free users should **upgrade** to paid plans
2. **Targeting**: where to post? who views?
   * e.g. platforms (Reddit, Facebook, Twitter, LinkedIn, YouTube, ...)
   * :bulb: ask customers which platform they prefer!
   * :warning: **context**: will a platform's users be in the right mood for your ads?
   * go **deep/specific**, e.g. target:
     - tech stack
     - role ({% glossary FE %}, {% glossary BE %}, {% glossary DevOps %}, {% glossary ML %}, {% glossary DS %})
     - company (enterprise, startup, freelancer)
     - level (junior, senior, architect)
   * use analytics/tracking/cookies ([for now](https://blog.hubspot.com/marketing/third-party-cookie-phase-out)) to filter out non-relevant targets
3. **Creative**: what to post?
   * **format** (in-feed, banner, pop-up) & **medium** (video, animation, text) should be **non-intrusive** & :warning: "as non-advertising as possible"
   * **content**: actual message to convey
     - :heavy_check_mark: don't fear some explicit, **technical jargon** and sarcastic **humour**
     - :warning: [focus](https://www.ethicalads.io/advertiser-guide) on **features** ("5ms video load time") [rather than values](https://stackoverflowsolutions.com/topic/developer-influence/create-effective-banner-ads) ("better videos quicker")
     - :warning: link to **comparison** to alternatives
     - :heavy_check_mark: link to **case studies** & **use cases**
     - :heavy_check_mark: link to **getting started**, **examples**, and **docs**
4. **Landing page**: where ad clicks lead
   * :warning: usually not good to use company homepage: too stuffed with projects unrelated to the ad
   * pick based on existing analytics (what are users currently doing), e.g.
     - amplify paths: `twitter -> blog on problem X -> product X -> signup` implies twitter ads should link to `blog on problem X`
     - shorten paths: `homepage -> product X -> docs for X -> pricing -> signup` implies ads for `X` could link to `docs for X`
     - amplifying might be better than shortening/creating new paths

## Channel comparison

*key: :heavy_check_mark::warning::stop_sign: emojis indicate how well things work.*

- experience of channels: :stop_sign: most don't work well
- [Google Display Network (GDN)](https://surfsideppc.com/google-display-ads)
  + :stop_sign: used by "most of the internet" so general (intrusive, not dev-focused)
  + :heavy_check_mark: could [*specify conversion event* for Google to optimise or *filter pages where ads are shown* to target better](https://www.poweredbysearch.com/blog/how-to-market-to-software-developers)
  + not a magic bullet
  + :warning: easy to overspend
  + there are many [guides](https://www.onlinemarketinggurus.com.au/blog/google-display-network-guide)
- [Ethical Ads](https://www.ethicalads.io)
  + :heavy_check_mark: targets devs (blogs, [readthedocs](https://readthedocs.org), etc.), context of ads is "learning/working"
  + :heavy_check_mark: small (image + brief text), non-intrusive
  + pay per impression
  + :heavy_check_mark: GDPR-compliant (no tracking -- targeting is done by page)
  + filtering by page costs more
- [Carbon Ads (BuySellAds)](https://www.carbonads.net)
  + :heavy_check_mark: [focus on devs](https://content.buysellads.com/advertisers/five-reasons-your-ads-arent-reaching-developers) (like Ethical Ads) -- mostly {% glossary ML %} and {% glossary DS %}
  + :stop_sign: more intrusive (like GDN)
- [Twitter Ads](https://ads.twitter.com)
  + :heavy_check_mark: appear in-feed
  + :warning: important to target engaging **keywords** & **"look-alike" (similar) followers**
  + :warning: good [guides](https://adespresso.com/blog/twitter-advertising-a-complete-guide) aren't dev-specific
- [Reddit Ads](https://advertising.reddithelp.com/en/categories/getting-started/create-a-reddit-ads-account)
  + :heavy_check_mark: in-feed, in-thread, or in-conversation
  + :heavy_check_mark: can target subreddits
  + :stop_sign: can only filter on location & device (not keywords nor topics)
- [StackOverflow Ads](https://stackoverflow.com/advertising)
  + :heavy_check_mark: non-intrusive, ads look like answers to questions
  + managed (not self-serve), min. contract $10~$15 k/month
- [YouTube Ads](https://www.youtube.com/ads)
  + :heavy_check_mark: **video remarketing** works well: amplify existing conversion paths by showing ads to people who visited your product/pricing/docs/high-intent-blog
  + lots of targeting options (like GDN)
  + :warning: intrusive, especially without proper targeting
- [Google Search Ads](https://blog.hubspot.com/marketing/google-adwords-ppc)
  + :heavy_check_mark: **branded search** works well: "a google tax on keywords" containing your product name (pay for a keyword to show up in search results)
  + top of [SERP](https://backlinko.com/hub/seo/serps) (intrusive default) or page bottom (feels more helpful)
  + think about **relevancy**:
    * :heavy_check_mark: brand name ("github")
    * core features/use cases ("{% glossary CI %}") -- :stop_sign: don't work well if linking to blogs
    * comon typos of both off teh abov ("gitub")
    * competitor comparison ("vs github", "github alternative")
    * :stop_sign: integrations ("slack")
    * :stop_sign: competitor ("gitlab")

:scroll::speech_balloon: Extended discussion at [ycombinator#32191615](https://news.ycombinator.com/item?id=32191615).
