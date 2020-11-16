Edgesite
==
## Introduction
Edgesite is a project to review whether a free Cloudflare Workers accoutn can support a near full-blown front-end website build. The website's content, and some configuration, is provided by a JSON file within this repo (/pages.json).

## Aim
The aim is to create an app that is:
* Fully deployed on a free Cloudflare Workers account (exception of the JSON file)
* A Single Page Application (SPA)
* A Progressive Web App (PWA)

### Goals
The app has been subject to W3c Validator, Page Speed Insights (performance) and Chrome DevTools Lighthouse (other categories). The scores will have to be 95+, with no errors or warning within the W3c Validator. The categories are:
* Performance _(Page Speed Insights)_
* Progressive Web App _(Chrome DevTools Lighthouse)_
* Best practices _(Chrome DevTools Lighthouse)_
* Accessibility (a11y) _(Chrome DevTools Lighthouse)_
* SEO _(Chrome DevTools Lighthouse)_
* W3c Validator: Errors _(W3c Validator)_
* W3c Validator: Warnings _(W3c Validator)_

## Technology used
* Data and configuration: JSON file on GitHub
* Edge JavaScript on Cloudflare Workers (using Wrangler and a Webpackage)
* HTML & CSS for the front-end pages
* Client-side JavaScript:
  * Web Workers for isomorphic/SPA
  * Service Workers for PWA

---

## Results

### Pages

| Objective                                       | Outcome |
|-------------------------------------------------|:-------:|
| All pages serve 200-OK status code              | Pass    |
| Pages can be crawled                            | Pass    |
| Not found page shown                            | Fail    |
| Not found page serves 404-Not Found status code | Pass    |


### Resources

| Objective                                       | Outcome |
|-------------------------------------------------|:-------:|
| Robots.txt returns 200-OK                       | Pass    |
| Robots.txt is plain/text; UTF-8                 | Pass    |
| XML sitemap is text/xml; UTF-8                  | Pass    |
| Service Worker returns 200-OK                   | Pass    |
| Service Worker is application/javascript; UTF-8 | Pass    |

### Functionality

| Objective                                       | Outcome |
|-------------------------------------------------|:-------:|
| Service Worker is installed                     | Pass    |
| App works offline                               | Pass    |
| App is SPA                                      | Pass    |

### Assessment


| Category                                        | Score   |
|-------------------------------------------------|:-------:|
| Performance                                     | 99      |
| Progressive Web App (PWA)                       | 14 / 14 |
| Best practices                                  | 100     |
| Accessibility (a11y)                            | 100     |
| SEO                                             | 100     |
| W3c Validator: Errors                           | 0       |
| W3c Validator: Warnings                         | 0       |

---

## Useful links
* Cloudflare Workers - https://developers.cloudflare.com/workers/
* PWA: Google Developers - https://developers.google.com/web/ilt/pwa
* Web Workers: Developer Mozilla - https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers

## Creator
Kevin Ellen, Director of Web Experience @ Croud