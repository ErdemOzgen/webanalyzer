# Wappalyzer API

This repository contains a dockerized and 'API-fied' version of [Wappalyzer](https://github.com/AliasIO/Wappalyzer). It aims to make it available through an API endpoint you can call from anywhere.


## To build it:
```
docker build -t webanalyzer .
```

## To run it:
```
docker run -p 3000:3000 webanalyzer
```

## To use it:
```

curl 'localhost:3000/extract?url=https://www.nsa.gov'
```

## Output:

```json
{
  "urls": {
    "https://www.nsa.gov/": {
      "status": 200
    }
  },
  "technologies": [
    {
      "slug": "dnn",
      "name": "DNN",
      "description": null,
      "confidence": 100,
      "version": null,
      "icon": "DNN.svg",
      "website": "https://www.dnnsoftware.com/",
      "cpe": "cpe:2.3:a:dnnsoftware:dotnetnuke:*:*:*:*:*:*:*:*",
      "categories": [
        {
          "id": 1,
          "slug": "cms",
          "name": "CMS"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "microsoft-asp-net",
      "name": "Microsoft ASP.NET",
      "description": "ASP.NET is an open-source, server-side web-application framework designed for web development to produce dynamic web pages.",
      "confidence": 100,
      "version": null,
      "icon": "Microsoft ASP.NET.svg",
      "website": "https://www.asp.net",
      "cpe": "cpe:2.3:a:microsoft:asp.net:*:*:*:*:*:*:*:*",
      "categories": [
        {
          "id": 18,
          "slug": "web-frameworks",
          "name": "Web frameworks"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "bootstrap",
      "name": "Bootstrap",
      "description": "Bootstrap is a free and open-source CSS framework directed at responsive, mobile-first front-end web development. It contains CSS and JavaScript-based design templates for typography, forms, buttons, navigation, and other interface components.",
      "confidence": 100,
      "version": "3.4.1",
      "icon": "Bootstrap.svg",
      "website": "https://getbootstrap.com",
      "cpe": "cpe:2.3:a:getbootstrap:bootstrap:*:*:*:*:*:*:*:*",
      "categories": [
        {
          "id": 66,
          "slug": "ui-frameworks",
          "name": "UI frameworks"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "animate-css",
      "name": "Animate.css",
      "description": "Animate.css is a ready-to-use library collection of CSS3 animation effects.",
      "confidence": 99,
      "version": null,
      "icon": "Animate.css.svg",
      "website": "https://animate.style",
      "cpe": null,
      "categories": [
        {
          "id": 66,
          "slug": "ui-frameworks",
          "name": "UI frameworks"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "matomo-analytics",
      "name": "Matomo Analytics",
      "description": "Matomo Analytics is a free and open-source web analytics application, that runs on a PHP/MySQL web-server.",
      "confidence": 100,
      "version": null,
      "icon": "Matomo.svg",
      "website": "https://matomo.org",
      "cpe": "cpe:2.3:a:matomo:matomo:*:*:*:*:*:*:*:*",
      "categories": [
        {
          "id": 10,
          "slug": "analytics",
          "name": "Analytics"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "jquery-ui",
      "name": "jQuery UI",
      "description": "jQuery UI is a collection of GUI widgets, animated visual effects, and themes implemented with jQuery, Cascading Style Sheets, and HTML.",
      "confidence": 100,
      "version": "1.12.1",
      "icon": "jQuery UI.svg",
      "website": "https://jqueryui.com",
      "cpe": "cpe:2.3:a:jquery:jquery_ui:*:*:*:*:*:*:*:*",
      "categories": [
        {
          "id": 59,
          "slug": "javascript-libraries",
          "name": "JavaScript libraries"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "jquery-migrate",
      "name": "jQuery Migrate",
      "description": "Query Migrate is a javascript library that allows you to preserve the compatibility of your jQuery code developed for versions of jQuery older than 1.9.",
      "confidence": 100,
      "version": "3.2.0",
      "icon": "jQuery.svg",
      "website": "https://github.com/jquery/jquery-migrate",
      "cpe": null,
      "categories": [
        {
          "id": 59,
          "slug": "javascript-libraries",
          "name": "JavaScript libraries"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "jquery",
      "name": "jQuery",
      "description": "jQuery is a JavaScript library which is a free, open-source software designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and Ajax.",
      "confidence": 100,
      "version": "3.5.1",
      "icon": "jQuery.svg",
      "website": "https://jquery.com",
      "cpe": "cpe:2.3:a:jquery:jquery:*:*:*:*:*:*:*:*",
      "categories": [
        {
          "id": 59,
          "slug": "javascript-libraries",
          "name": "JavaScript libraries"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "google-analytics",
      "name": "Google Analytics",
      "description": "Google Analytics is a free web analytics service that tracks and reports website traffic.",
      "confidence": 100,
      "version": null,
      "icon": "Google Analytics.svg",
      "website": "https://google.com/analytics",
      "cpe": null,
      "categories": [
        {
          "id": 10,
          "slug": "analytics",
          "name": "Analytics"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "aos",
      "name": "AOS",
      "description": "JavaScript library to animate elements on your page as you scroll.",
      "confidence": 100,
      "version": null,
      "icon": "AOS.svg",
      "website": "https://michalsnik.github.io/aos/",
      "cpe": null,
      "categories": [
        {
          "id": 59,
          "slug": "javascript-libraries",
          "name": "JavaScript libraries"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "google-font-api",
      "name": "Google Font API",
      "description": "Google Font API is a web service that supports open-source font files that can be used on your web designs.",
      "confidence": 100,
      "version": null,
      "icon": "Google Font API.svg",
      "website": "https://google.com/fonts",
      "cpe": null,
      "categories": [
        {
          "id": 17,
          "slug": "font-scripts",
          "name": "Font scripts"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "font-awesome",
      "name": "Font Awesome",
      "description": "Font Awesome is a font and icon toolkit based on CSS and Less.",
      "confidence": 100,
      "version": null,
      "icon": "Font Awesome.svg",
      "website": "https://fontawesome.com/",
      "cpe": null,
      "categories": [
        {
          "id": 17,
          "slug": "font-scripts",
          "name": "Font scripts"
        }
      ],
      "rootPath": true
    },
    {
      "slug": "hsts",
      "name": "HSTS",
      "description": "HTTP Strict Transport Security (HSTS) informs browsers that the site should only be accessed using HTTPS.",
      "confidence": 100,
      "version": null,
      "icon": "default.svg",
      "website": "https://www.rfc-editor.org/rfc/rfc6797#section-6.1",
      "cpe": null,
      "categories": [
        {
          "id": 16,
          "slug": "security",
          "name": "Security"
        }
      ],
      "rootPath": true
    }
  ]
}
```
## License:
MIT License