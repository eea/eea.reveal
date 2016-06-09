# eea.reveal

![Gephi](https://github.com/eea/eea.reveal/raw/master/docs/network-example.png)

**Beta**

This tool is used to visualise network data on the web (HTML5) and reveal hidden clusters and other relations within the network.

The network data and layout is first generated via [Gephi - The Open Graph Viz Platform](https://github.com/gephi/gephi) and the exported data can be visualised on the web via eea.reveal.

It uses two existing Gephi plugins:

 - [Gexf-JS Web Viewer](https://marketplace.gephi.org/plugin/gexf-js-web-viewer/) [Github](https://github.com/raphv/gexf-js)
 - [Sigmajs Exporter](https://marketplace.gephi.org/plugin/sigmajs-exporter/) [Github](https://github.com/oxfordinternetinstitute/gephi-plugins/tree/sigmaexporter-plugin/modules/sigmaExporter) 

## How to run the demos

### via Docker

This repo contains a sample docker-compose.yml file to deploy the HTML5 visualisations with a nginx as webserver.

```
$ git clone https://github.com/eea/eea.reveal.git
$ cd eea.reveal
$ sudo docker-compose up -d
```

An nginx server will start up on a random available port on the host. Do a ```docker-compose ps``` to see which port has been assigned. 

Go to http://localhost:PORT/ and select one of the examples.
