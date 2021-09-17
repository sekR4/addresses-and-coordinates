# Addresses and Coordinates
Finding all addresses and their corresponding latitude/longitude in Germany

## 0. Prologue
```bash
pyenv virtualenv 3.8.10 addr
pyenv activate addr
pip install -r src/requirements.txt
```

## 1. Hip to be square
We'll build a rectangle. We define its upper left point NW (latitude, longitude) as NW = (55.374194, 3.645059) and the lower right point SE = (46.887744, 15.133453). 

## Example Output OSM Nominatim
https://nominatim.openstreetmap.org/search.php?q=50.910794%2C+11.1512281&format=jsonv2
```python
[{"place_id":44063298,"licence":"Data © OpenStreetMap contributors, ODbL 1.0. https://osm.org/copyright","osm_type":"node","osm_id":3478841420,"boundingbox":["50.910744","50.910844","11.1511781","11.1512781"],"lat":"50.910794","lon":"11.1512281","display_name":"25, Pappelweg, Klettbach, Kranichfeld, Landkreis Weimarer Land, Thüringen, 99102, Deutschland","place_rank":30,"category":"place","type":"house","importance":0.001}]```