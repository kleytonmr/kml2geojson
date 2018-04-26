# Converter kml para GeoJson

GeoJSON e KML são formatos para armazenar informações espaciais. Arquivos KML são comumente encontrados no Google Earth
e aplicativos semelhantes, por isso pode ser útil converter KML em GeoJSON. A biblioteca python kml2geojson pode ser
usado para converter KML para GeoJSON. kml2geojson funciona como uma ferramenta da linha de comando ou pode ser usado
como uma biblioteca dentro de outros programas.

### Instalação

Instalação kml2geojson usando pip:
```py
pip install kml2geojson
```
Use como ferramenta de linha de comando. O kml2geojson pode ser usado como uma ferramenta na linha de comando. Você pode usá-lo desta maneira se tiver alguns arquivos kml que você só precisa converter, sem qualquer programação adicional.

O uso geral do kml2geojson é:
```py
1 k2g [options] kml_file output_dir
```
Para uso básico, podemos executar:
```py
1 k2g test.kml json_files
```
Que converterá o arquivo "test.kml" em "test.json" (uma "Coleção de recursos" do GeoJSON) e colocará a saída em um diretório "json_files". Se o diretório "json_files" não existir, ele será criado.

Para ver recursos mais avançados, execute:
```py
1 k2g ---help
```

Ou verifique a [documentação](https://rawgit.com/araichev/kml2geojson/master/docs/_build/singlehtml/index.html) kml2geojson
-----

Use As a library
kml2geojson can also be called as a library so you can convert kml to geojson within other programs.

Basic conversion using the kml2geojson library can be done with:

1 kml2geojson.main.convert(kml_file, output_directory)

1 import kml2geojson
2 kml2geojson.main.convert('./test.kml', '../data/json_files')

See more advanced options at the the kml2geojson documentation. (https://rawgit.com/araichev/kml2geojson/master/docs/_build/singlehtml/index.html)

---------------
https://gis.stackexchange.com/questions/73768/converting-geojson-to-python-objects


