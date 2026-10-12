# Warehouse LiDAR perception

Localizing window frames in a warehouse model from a LiDAR point cloud. This was research at Carnegie Mellon University in Pittsburgh. Object detection on this task reached about 85% accuracy.

This repository is the public write-up. Pictures, clouds, and short videos belong in [`media/`](media/). The dataset and training runs are not published here.

## Pipeline

1. Remove ground points with RANSAC, so the floor is not treated as structure.
2. Cluster what remains with DBSCAN.
3. Classify the clusters with PointNet++.

The target objects are window frames in the warehouse model.

## Media

Add renders, cloud snapshots, and short videos to `media/` and link them from this README. Nothing is in that folder yet.
