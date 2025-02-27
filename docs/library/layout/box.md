---
import reflex as rx
from pcweb.templates.docpage import docdemo

colorful_boxes_example = """rx.vstack(
    rx.box("Example", bg="yellow", border_radius="sm", width="20%"),
    rx.box("Example", bg="orange", border_radius="md", width="40%"),
    rx.box("Example", bg="red", border_radius="md", width="60%"),
    rx.box("Example", bg="lightblue", border_radius="lg", width="80%"),
    rx.box("Example", bg="lightgreen", border_radius="xl", width="100%"),
    width="100%",
)"""

button_box_example = """rx.box(
    rx.button("Click Me"),
    bg="lightgreen",
    border_radius="15px",
    border_color="green",
    border_width="thick",
    padding=5,
)"""

iframe_box_example = """rx.box(
    element= "iframe",
    src="https://www.youtube.com/embed/9bZkp7q19f0",
    width = "100%",
)"""

---

Box is a generic container component that can be used to group other components.

```reflex
docdemo(colorful_boxes_example)
```

Below is an example of how a box component can contain other components.

```reflex
docdemo(button_box_example)
```

Box can also compose videos and iframe elements.

```reflex
docdemo(iframe_box_example)
```