# Sigma Web Development Course

## Tutorial # 06 | SEO and Core Web Vitals in HTML

[![Sigma Web Development Course - Tutorial # 6](https://img.youtube.com/vi/CyRlWlaJnTY/maxresdefault.jpg "Tutorial # 6 SEO and Core Web Vitals in HTML")](https://www.youtube.com/watch?v=CyRlWlaJnTY&list=PLu0W_9lII9agq6TrH9XLIKQvv0iaF2X3w&index=6)

---

## Search Engine Optimization (SEO)

**SEO** stands for Search Engine Optimization. It is the art and science of improving a website to increase its visibility in free, organic search results on engines like Google.

In HTML, SEO means optimizing the website's loading speed and performance using the **Core Web Vitals** to boost the website's ranking.

**SEO** is a deep topic and a whole skill for YouTube videos and social media post not just only for Website.

## SEO in HTML

**Some elements to do SEO in HTML are below.**

### Title Tag in HTML

The Title Tag `<title>` is an essential HTML element for SEO located in the `<head>` section of a webpage that defines its title.

It appears as the clickable blue link in search engine results pages, thats why optimizing it is crucial because it does not only enhances SEO ranking but also provide users with the first impression of your content  

#### SEO Best Practices for Title Tag
 
<br>

- **Optimal Length:** Keep titles between 50–60 characters to avoid truncate (...)

<br>

- **Keyword Placement:** Place your primary keyword as close to the beginning of the title as possible (front-loading).

<br>

- **Uniqueness:** Every page on your website must have a unique title tag to avoid confusing search engines and users. 

<br>

- **Avoid Keyword Stuffing:** Do not list keywords repeatedly; this can look spammy and may result in search engines rewriting your title or penalizing your rank.

<br>

- **Branding:** For brand recognition, Include your brand name at the end, separated by a pipe (|) or hyphen (-) (e.g., `Web Development - CodeWithHarry`).

### Meta Description Tag in HTML

Meta description tag provides a brief summary of the page's content. While not visible to users on the actual page, it is frequently used by search engines.

Search Engines Might Ignore Your, engines do not always use the provided meta description. If you dont have this tag, Google, for instance, ignores it roughly **70% of the time** and generate its own snippet from the page content if it believes that better matches the user's specific query.

**Example:**
```bash
<meta name="description" content="This is a brief summary of my webpage to attract searchers.">
```


---

## Core Web Vitals

The Core Web Vitals metrics are a set of three metrics that measure real-world user experience regarding page loading, interactivity, and visual stability.

#### The Three Core Web Vitals:
1. Largest Contentful Paint (LCP)
2. Cumulative Layout Shift (CLS)
3. Interaction to Next Paint (INP)

### 1. Largest Contentful Paint (LCP)

It measures the loading performance of website and its content. It marks the point when the main (biggest) content (image or text block) finishes rendering.

> Good LCP is **2.5 seconds or faster.**

### 2. Cumulative Layout Shift (CLS)

Measures the **visual stability** of the content and elements. It determines how much unexpected shifting of page content occurs during loading.

Good CLS is **0.1 or less.**

### 3. Interaction to Next Paint (INP)

Measures **responsiveness**. It assesses how quickly a page responds to all user interactions (clicks, taps).

Good INP is **200 milliseconds or less.**

> **Note:** Interaction to Next Paint (INP) replaced First Input Delay (FID) on September 9, 2024.

---

## Inspect Tool Lighthouse

### What is Lighthouse?

Ligthouse is the a developer tool integrated in the browser that analyzes the website metrics, load speed and performance for both desktop and mobile.

It and points and suggest scope of improvements in detail by providing actionable reports to fix issues and enhance user experience.

### How to Use Lighthouse in DevTools

1. Open Browser and navigate to the webpage you want to audit.
2. Open DevTools (F12 or Right-click -> "Inspect").
3. Click the Lighthouse tab in the top navigation bar.
4. Select the device (Mobile or Desktop) and categories (Performance, SEO, etc.)
5. Click "Analyze page load" to generate the report.