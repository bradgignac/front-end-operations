# Abstract

The rise of Javascript frameworks such as Angular, Ember, and Backbone have caused
a shift in application code from the server to the client. However, most operations
teams and tooling still revolve around server-side applications. This talk will
take a look at how the team behind Rackspace's Cloud Control Panel is deploying
and instrumenting a large client-side application to provide real-time visibility
into the performance of our application.

# Outline

- Title Slide
  - Introduce Myself
  - Introduce Rackspace
  - bradgignac.com, @bradgignac
- What is Operations?
  - Work to be done, not a specific role - neck beard photo.
  - Shipping code to production and keeping it running.
  - How do I know my application is doing what it should be?
    - Is the site down?
    - Are users encountering bugs?
    - Are users seeing errors?
    - Are some users seeing errors?
    - Not a simple question to answer.
  - Control Panel Overview
    - Single Page Application
    - XXX KLOC, broken down by front-end and back-end
    - Deploys/Day or Deploys/Year
    - Feature Flags, X permutations of our application at any given time.
- Why Front-End Operations?
  - Operating Systems and Browsers
  - Distributed Computing - Mention the Fallacies of Distributed Computing.
- Server Side Operations - Should I go over typical tools for familiarity?
- Client Side Operations
  - Build - "Getting your assets ready for production."
    - Images
      - GIF/JPEG/PNG vs SVG
      - Spriting vs Base64
      - Image Optimization
    - JS and CSS - Concatenation, Minification, Namespace Leakage, Modules
  - Test - Should I include this? Do I need more content?
    - Linting
    - Unit Tests
    - Integration Tests
    - Cross-Browser Tests
    - Screenshot Tests
  - Deployment - Modules, Versioning, Caching, CDN
  - Performance - RUM, YSlow/PageSpeed, Benchmark.js, Layout Trashing, CPU Usage, Memory Usage, Page Weight
  - Monitoring - Analytics, Error Reporting, Instrumentation, Logging, Statistics
- What else?
- What's coming next?
  - SPDY and HTTP2
- Thank You
  - bradgignac.com, @bradgignac

---

- Instrumentation
  - New Relic
  - Proxy Instrumentation
  - Web Sockets
  - Statsd + Graphite
  - Logging + Graylog
  - Exception Handling
  - Core Metrics + Analytics

- How to include experimentation?
- How do SPDY and HTTP2 change our techniques?
- Review front-end operations conference talks.
- Review Yahoo's Beacon tool.
- How to balance tools vs techniques?
