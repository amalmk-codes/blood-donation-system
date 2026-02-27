# MongoDB Migration Instructions

1. Install MongoDB Compass or use `mongoimport`.

2. Export your own MongoDB URI (from Atlas) and replace `$MONGODB_URI` below:

```bash
mongoimport --uri "YOUR_MONGODB_URI" --collection donors --file donors.json --jsonArray
mongoimport --uri "YOUR_MONGODB_URI" --collection hospitals --file hospitals.json --jsonArray
