# Generating implicit object fragment datasets for machine learning

<p align="center">
    <img src="data/readme/teaser.png">
</p>

## Data download

The fragment data is available at <a href="https://s5-ceatic.ujaen.es/fragment-dataset-uja/">our research institute's page</a>. Please, note that there are two datasets; one is split into eight files since it is approximately 450GB, whereas the other (`vessels_200_obj_ply_no_zipped.zip`) is lighter (27 GB). The latter is intended for testing the dataset since it only contains decimated fragments of 200 models, with no individual zipping.

Otherwise, please go to `decompress` folder to learn how to decompress binary files (triangle meshes, point clouds and voxelizations). Point clouds are decompressed in C++ using the Point Cloud Library, whereas the others are decompressed using Python.

<p>
    <img src="data/body/decompress_binaries.png">
</p>

<!--## Training

To compare the performance of popular fracture assembly networks, we used the baseline code of Sellán et al. (2022). It provides DGL-Net, RGL-Net as well as a simple LSTM architecture. We tested our dataset using their artifact dataset, which is the most similar to ours (comes from scanned items), and our light dataset (200 vessels). Although the used networks are far from being perfect, there were some remarkable results such as the one in the following figure.

<p>
    <img src="data/readme/assembled_pieces.png" width="60%">
</p>-->