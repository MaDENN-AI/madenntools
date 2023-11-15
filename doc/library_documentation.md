## Function Documentation

**_Full documentation is available as a docstring for each function_**

### madenntools.cv

- `madenntools.cv.blend(foreground_image, binary_mask, level=(128, 128, 128))`: Blends a BGR foreground image with a BGR background using a binary mask as the alpha channel.

- `madenntools.cv.collage_images(image_and_caption_list, output_path, max_columns=3, caption_height=30)`: Creates a horizontal collage from a list of image paths and captions using OpenCV, and saves it to the specified output path.

- `madenntools.cv.collage_directories(root_dir, output_dir, max_columns=3, caption_height=30)`: Creates collages for images in subdirectories within a root directory, and saves them to the output directory. Ignores the output directory if it's found within the root directory.

### madentools.metric

- `madenntools.metric.luminance(image_rgb, sdr):` Compute luminance values from an RGB image, with an option to specify whether it's SDR or HDR.

- `madenntools.metric.fhlp(image, sdr=False):` Compute the Fraction of HighLight Pixel (FHLP) metric, which quantifies the spatial ratio of 'highlight' pixels in SDR or HDR images.

- `madenntools.metric.ehl(image, sdr=False):` Compute the Extent of HighLight (EHL) metric, measuring the average pixel distance between HDR luminance and a clamped version in SDR or HDR images.

- `madenntools.metric.all(image, sdr=False):` Compute the Average Luminance Level (ALL) metric, evaluating the average luminance level in SDR or HDR images.

- `madenntools.metric.si(image, sdr=False):` Compute the Spatial Information (SI) metric, indicating the amount of spatial detail or complexity in an image.

- `madenntools.metric.cf(image, sdr=False):` Compute the Opponent Color Metric - Colorfulness (CF) metric, assessing image quality using an opponent color space.

- `madenntools.metric.stdL(image, sdr=False):` Compute the standard deviation of luminance (stdL) metric, measuring the variation in brightness values across an image.

- `madenntools.metric.fwgp(image_RGB, sdr=False, image_name='doesnt_matter.png'):` Compute the Fraction of Pixels Outside of BT 709 and Inside of BT 2020 (FWGP) metric, indicating how many pixels are outside of BT 709 and inside BT 2020 in SDR or HDR images.