# Nodes
There are four nodes created for this task (further documentation can be found in the node filte itself):
  - [oCam_image_node](https://github.com/umdlife/UPlatform/blob/feat/oCam/umd_vision/scripts/oCam_image_node)
  - [image_preprocessing_node](https://github.com/umdlife/UPlatform/blob/feat/oCam/umd_vision/scripts/image_preprocessing_node)
  - [image_to_barcode_node](https://github.com/umdlife/UPlatform/blob/feat/oCam/umd_vision/scripts/image_to_barcode_node)
  - [barcode_filter_node](https://github.com/umdlife/UPlatform/blob/feat/oCam/umd_vision/scripts/oCam_image_node)

# Typical Flow
![Image description](https://github.com/umdlife/UPlatform/blob/feat/oCam/umd_vision/docs/barcode_recognition/sources/barcode_node_flow.png)

# Note
It is important to know that neither the image_preprocessing_node, nor the barcode_filter_node are strictly necessary. One could remap the subscriber from the image_to_barcode_node to the publisher of the oCam_image_node and skip the preprocessing that way.
