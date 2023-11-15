## Contribution practices

- Pay attention when changing the type of the input/output data inside the function. Avoid if possible 
- scripts will be added to directories (example: cv), and linked the __init__.py file of that directory. 
- Follow the naming convention and the docstring style. Example

```python
    """   
    Blend a foreground image with a background using the binary mask as the alpha channel.

    Args:
        foreground_image (numpy.ndarray): The BGR image to be blended.
        binary_mask (numpy.ndarray): The binary mask in BGR format.
        level (tuple, optional): The BGR color of the background. Defaults to (128, 128, 128).

    Returns:
        numpy.ndarray: The blended image.
    """
    def blend(foreground_image, binary_mask, level=(128, 128, 128)):
```
