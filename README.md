# ComfyUI-IPAnimate

- This project generates videos frame-by-frame based on IPAdapter+ControlNet. Unlike [Steerable-motion](https://github.com/banodoco/Steerable-Motion), we do not rely on AnimateDiff, mainly because the current videos generated by AnimateDiff are relatively blurry. By using frame-by-frame control with IPAdapter+ControlNet, we can produce higher resolution and more controllable videos.

![Input Image](./demo/input.png)
![Generated Video](./demo/output.gif)

## Usage Instructions

- Similar to the structure of [Steerable-motion](https://github.com/banodoco/Steerable-Motion), we provide both linear and dynamic control modes and allow the input of external ControlNet images to offer more flexibility.

![Model](./demo/model.png)

- Main Parameters:
    - Frame length change
    - Influence intensity range
    - Relative influence of IPA and CN

- For the detailed workflow, please refer to: [demo](./demo/IPAnimate-demo.json)

## References

- [Steerable-motion](https://github.com/banodoco/Steerable-Motion)
- [Kosinkadink's ComfyUI-Advanced-ControlNet](https://github.com/Kosinkadink/ComfyUI-Advanced-ControlNet)
- [IPAdapter_plus](https://github.com/cubiq/ComfyUI_IPAdapter_plus)
