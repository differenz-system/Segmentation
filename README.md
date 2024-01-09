## Running the application

```bash
python iasam_app.py
```

* Open http://127.0.0.1:7860/ in your browser.
* Note: If you have a privacy protection extension enabled in your web browser, such as DuckDuckGo, you may not be able to retrieve the mask from your sketch.

### Options

* `--save-seg`: Save the segmentation image generated by SAM.
* `--offline`: Execute inpainting using an offline network.
* `--sam-cpu`: Perform the Segment Anything operation on CPU.

## Downloading the Model

* Launch this application.
* Click on the `Download model` button, located next to the [Segment Anything Model ID](https://github.com/facebookresearch/segment-anything#model-checkpoints). This includes the [Segment Anything in High Quality Model ID](https://github.com/SysCV/sam-hq), [Fast Segment Anything](https://github.com/CASIA-IVA-Lab/FastSAM), and [Faster Segment Anything (MobileSAM)](https://github.com/ChaoningZhang/MobileSAM).
  * Please note that the SAM is available in three sizes: Base, Large, and Huge. Remember, larger sizes consume more VRAM.
* Wait for the download to complete.
* The downloaded model file will be stored in the `models` directory of this application's repository.

## Usage

* Drag and drop your image onto the input image area.
  * Outpainting can be achieved by the `Padding options`, configuring the scale and balance, and then clicking on the `Run Padding` button.
  * The `Anime Style` checkbox enhances segmentation mask detection, particularly in anime style images, at the expense of a slight reduction in mask quality.
* Click on the `Run Segment Anything` button.
* Use sketching to point the area you want to inpaint. You can undo and adjust the pen size.
  * Hover over either the SAM image or the mask image and press the `S` key for Fullscreen mode, or the `R` key to Reset zoom.
* Click on the `Create mask` button. The mask will appear in the selected mask image area.

### Mask Adjustment

* `Expand mask region` button: Use this to slightly expand the area of the mask for broader coverage.
* `Trim mask by sketch` button: Clicking this will exclude the sketched area from the mask.
* `Add mask by sketch` button: Clicking this will add the sketched area to the mask.

### Color Change
* `Color` button: Use this pick a color from hexvalues to change the color of selected mask.

### Contact us

* Please don't hesitate to contact us if you have any issues with the code or if you have any other remarks or questions.
* We are always open for a collaboration with you.