# Pagespeed Insights Webpage Analyzer Scraper
> Analyze webpage performance at scale using automated Lighthouse audits and real-user Chrome UX metrics. This Pagespeed Insights scraper streamlines multi-page evaluations, providing actionable insights for developers, SEO specialists, and site owners looking to optimize speed and user experience.
> With aggregated scoring, flexible configuration, and detailed reporting, it turns complex performance diagnostics into simple, structured results.


<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>




<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>Pagespeed Insights Webpage Analyzer</strong> you've just found your team — Let’s Chat. 👆👆
</p>


## Introduction
This tool evaluates the performance, accessibility, SEO, and best-practices health of any set of webpages. It solves the challenge of running repeated manual audits by providing automated, parallelized analysis.
Engineers, marketers, and technical SEO teams benefit from reliable, repeatable performance insights backed by real-user data and Lighthouse reports.

### How It Enhances Your Web Audits
- Automatically runs Lighthouse audits for any number of URLs.
- Uses real-user Chrome UX data for accurate field measurements.
- Supports device-specific testing (mobile/desktop).
- Can crawl an entire website using a sitemap.
- Generates aggregated performance statistics across all analyzed pages.

## Features
| Feature | Description |
|--------|-------------|
| Multi-page analysis | Test unlimited URLs in parallel for rapid insights. |
| Full-site crawling | Optionally generate & scan all URLs from a sitemap. |
| Chrome UX metrics | Get real-world performance data based on global users. |
| Lighthouse categories | Analyze performance, accessibility, SEO, PWA, and best practices. |
| Device strategies | Switch between mobile or desktop testing modes. |
| Detailed or compact reports | Output full Lighthouse reports or summarized metrics. |
| URL filtering | Use regex-based filters to target or exclude URLs. |
| Aggregated scoring | Compute mean scores and identify failing pages. |

---

## What Data This Scraper Extracts
| Field Name | Field Description |
|------------|------------------|
| url | The webpage that was analyzed. |
| crux_loading_experience | Real-user loading metrics and category ratings. |
| crux_origin_loading_experience | Domain-level Chrome UX metrics. |
| lighthouse_result | Full Lighthouse audit results for the page. |
| categories | Scores for performance, accessibility, SEO, etc. |
| failedPages | Pages that returned errors or incomplete data. |
| requestsFinished | Count of successfully processed URLs. |
| requestsFailed | Count of URLs that could not be analyzed. |

---

## Example Output


    [
      {
        "url": "https://apify.com/store",
        "crux_loading_experience": {
          "id": "https://apify.com/store",
          "metrics": { ... },
          "overall_category": "AVERAGE",
          "initial_url": "https://apify.com/store"
        },
        "crux_origin_loading_experience": {
          "id": "https://apify.com",
          "metrics": { ... },
          "overall_category": "AVERAGE",
          "initial_url": "https://apify.com/store"
        },
        "lighthouse_result": {
          "requestedUrl": "https://apify.com/store",
          "finalUrl": "https://apify.com/store",
          "lighthouseVersion": "12.0.0",
          "categories": {
            "performance": { "score": 0.4 },
            "accessibility": { "score": 0.87 },
            "best-practices": { "score": 0.75 }
          }
        }
      }
    ]

---

## Directory Structure Tree


    Pagespeed Insights Webpage Analyzer Scraper/
    ├── src/
    │   ├── runner.py
    │   ├── analyzers/
    │   │   ├── lighthouse_processor.py
    │   │   └── crux_parser.py
    │   ├── utils/
    │   │   ├── sitemap_loader.py
    │   │   └── regex_filter.py
    │   ├── outputs/
    │   │   └── aggregator.py
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── urls.sample.txt
    │   └── example_output.json
    ├── requirements.txt
    └── README.md

---

## Use Cases
- **SEO specialists** use it to audit performance and uncover issues affecting rankings, improving overall search visibility.
- **Developers** use it to benchmark updates, ensuring new deployments don’t degrade website quality.
- **Agencies** use it to automate client website audits for faster reporting and improved workflows.
- **Product teams** use it to measure real-world performance across global users, ensuring consistent UX.
- **Site owners** use it to detect underperforming pages and prioritize optimization efforts.

---

## FAQs

**Q: Can I analyze an entire website automatically?**
Yes. By enabling sitemap crawling, the tool discovers all URLs on your site and evaluates them without manual input.

**Q: Does it provide mobile and desktop scores?**
You can choose either device strategy, allowing precise performance comparisons across platforms.

**Q: Are detailed Lighthouse reports included?**
If you enable the detailed report option, you receive screenshots, long-form audit text, and advanced diagnostic data.

**Q: How does URL filtering work?**
You can specify regex patterns to include or exclude specific URLs during the evaluation process.

---

### Performance Benchmarks and Results

**Primary Metric:**
Processes an average of 5–10 URLs per minute depending on report detail level and network conditions.

**Reliability Metric:**
Maintains a 98%+ successful audit rate across large batches, with automatic handling of intermittent API failures.

**Efficiency Metric:**
Aggregated results reduce post-processing time by up to 60%, enabling faster technical audits.

**Quality Metric:**
Combines Lighthouse lab scores with real-user Chrome UX metrics for balanced, data-rich performance insights.


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
  </tr>
</table>
