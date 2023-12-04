# Image resolution extraction

### Description
Component that extracts image resolution data from the images

### Inputs / outputs

**This component consumes:**

- image: binary

**This component produces:**

- image: binary
- image_width: int32
- image_height: int32

### Arguments

This component takes no arguments.

### Usage

You can add this component to your pipeline using the following code:

```python
from fondant.pipeline import ComponentOp


extract_image_resolution_op = ComponentOp.from_registry(
    name="extract_image_resolution",
    arguments={
        # Add arguments
    }
)
pipeline.add_op(extract_image_resolution_op, dependencies=[...])  #Add previous component as dependency
```
