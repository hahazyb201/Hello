Hello: A Geo-index and Image Recognition Based Social Network<br>
Built a web service in Go to handle posts and deployed to GKE (Google Kubernetes Cloud) for better scaling.<br>
Used ElasticSearch on GCE to store those posts and enable geo-location based search for posts nearby.<br>
Used BigTable to backup those posts with images in the posts stored in GCS (Google Cloud Storage) bucket.<br>
Utilized Google Dataflow to implement a weekly dump of posts to BigQuery for offline analysis.<br>
Utilized Google Cloud ML API and Tensorflow to train a face detection model and integrate with the Go service.<br>
<br>
Attention:<br>
1.Change the ES_URL in main.go to your own url where your elastic search server runs.<br>
2.Because Bigtable is too expensive, so I deleted the Bigtable related code.<br>
