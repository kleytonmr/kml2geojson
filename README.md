# Converter kml para GeoJson

GeoJSON e KML são formatos para armazenar informações espaciais. Arquivos KML são comumente encontrados no Google Earth
e aplicativos semelhantes, por isso pode ser útil converter KML em GeoJSON. A biblioteca python kml2geojson pode ser
usado para converter KML para GeoJSON. kml2geojson funciona como uma ferramenta da linha de comando ou pode ser usado
como uma biblioteca dentro de outros programas.

### Instalação

Instalação kml2geojson usando pip:
```python
pip install kml2geojson
```
------

Use As A Command Line Tool
kml2geojson can be used as a tool from the command line. You can use it this way if you have some kml files 
that you just need to convert, without any additional programming.

The general usage of kml2geojson is:

1 k2g [options] kml_file output_dir

For basic usage we can run:

1 k2g test.kml json_files

Which will convert the file ‘test.kml’ to ‘test.json’ (a GeoJSON ‘Feature Collection‘) and put 
the output into a directory ‘json_files’. If the directory ‘json_files’ does not exist, then it is created.

To see more advanced features, run:
1 k2g --help

--------
Or checkout the kml2geojson documentation.(https://rawgit.com/araichev/kml2geojson/master/docs/_build/singlehtml/index.html)
--------

Use As a library
kml2geojson can also be called as a library so you can convert kml to geojson within other programs.

Basic conversion using the kml2geojson library can be done with:

1 kml2geojson.main.convert(kml_file, output_directory)

1 import kml2geojson
2 kml2geojson.main.convert('./test.kml', '../data/json_files')

See more advanced options at the the kml2geojson documentation. (https://rawgit.com/araichev/kml2geojson/master/docs/_build/singlehtml/index.html)

---------------
https://gis.stackexchange.com/questions/73768/converting-geojson-to-python-objects


