# Dockerfile sample for Jubatus

You can try jubatus with docker very rapidly.

## Usage

example of using classifier

```
$ cd classifier
$ emacs arow.json # edit config if you want
$ sudo docker build -t my_jubatus .
...
Successfully built ae963513ed52
$ sudo docker run -t -i -p 127.0.0.1:9199:9199 my_jubatus
```

### How to configure jubatus server

See documentations of...
[fv_converter configuration](http://jubat.us/en/fv_convert.html)
[classifier configuration](http://jubat.us/en/api_classifier.html)
[recommender configuration](http://jubat.us/en/api_recommender.html)
[regression configuration](http://jubat.us/en/api_regression.html)
[anomaly configuration](http://jubat.us/en/api_anomaly.html)
[nearest_neighbor configuration](http://jubat.us/en/api_nearest_neighbor.html)
[clustering configuration](http://jubat.us/en/api_clustering.html)
[stat configuration](http://jubat.us/en/api_stat.html)
[graph configuration](http://jubat.us/en/api_graph.html)
