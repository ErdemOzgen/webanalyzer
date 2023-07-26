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
export WAP_QUERY = localhost:3000/extract?url
curl 'WAP_QUERY=https://www.nsa.gov'
```
## License:
MIT License