# Abstract

The rise of Javascript frameworks such as Angular, Ember, and Backbone have caused
a shift in application code from the server to the client. However, most operations
teams and tooling still revolve around server-side applications. This talk will
take a look at how the team behind Rackspace's Cloud Control Panel is deploying
and instrumenting a large client-side application to provide real-time visibility
into the performance of our application.

# Outline

X Title Slide
  - Introduce Myself
  - Introduce Rackspace
  - bradgignac.com, @bradgignac
- What is Operations?
  - Questions?
  - Pipeline (Build -> Testing -> Deployment -> Monitoring)
X Why Front-End Operations?
  - Move from jQuery -> Rich UIs and SPAs
    !!! Cloud Control Panel examples
  - Distributed Computing - Mention the Fallacies of Distributed Computing.
    !!! Cloud Control Panel examples
  - Many Versions of our Application
    !!! Cloud Control Panel examples
    - Total Versions = Operating Systems and Browsers +
                       RBAC Roles +
                       Fetaure Flags
- Client-Side Operations
  - Build
    - Packaging Images
    - Packaging Stylesheets
    - Packaging Javascript
  - Testing
  - Deployment
  - Monitoring
    - Logging
    - Instrumentation
    - Error Tracking
    - Performance

# Outline (Old)

- Client Side Operations
  - Build - "Getting your assets ready for production."
    - Images
      - GIF/JPEG/PNG vs SVG
      - Spriting vs Base64
      - Image Optimization
    - Stylesheets
      - Concatenation
      - Minification
      - Gzipping
    - JavaScripts
       - Concatenation
       - Minification
       - Gzipping
       - Namespace Leakage
       - Modules
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
