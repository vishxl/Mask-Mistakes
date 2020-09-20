# Mask Mistakes Detection

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]


Detect the mistakes people make while wearing masks. Using YOLO model with Darknet Framework for Multiclass Object Detection. Labels were inspired from this [article](https://www.rochesterregional.org/news/2020/07/how-not-to-wear-a-mask):

<img src="https://www.rochesterregional.org/-/media/how-to-properly-wear-a-mask-copy.jpg?w=1290&hash=98A1C0A325F8C756FEDA2A5C6DB600D5B223E88A" height="50%" width="50%" >

## Dataset Preparation
Scraping Images from Google Images using [Download All Images](https://chrome.google.com/webstore/detail/download-all-images/ifipmflagepipjokmbdecpmjbibjnakm?hl=en) Extension.

#### Search Queries
```bash
wrong mask wearing, mask mistakes, 鼻出し
```
#### Labels
```
"The Escape Hatch"
"The Earring"
"The Sniffer"
"The Stache"
"The Nose Plug"
"The Neckbeard"
```
#### Labelling and Annotation
<img src="https://raw.githubusercontent.com/tzutalin/labelImg/master/resources/icons/app.png" height="5%" width="5%" >

🖍️[LabelImg](https://github.com/tzutalin/labelImg) is a graphical image annotation tool and label object bounding boxes in images 



## Training
The files maskmis.data and maskmis.names should go in the /data folder of darknet.
Don't forget to create the train.txt and test.txt that maskmis.data calls.

Finally, start training using the following command:

<pre>$ ./darknet -i 0 detector train data/maskmis.data cfg/yolov3_maskmis.cfg darknet53.conv.74</pre>

<!--
## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install foobar
```

## Usage

```python
import foobar

foobar.pluralize('word') # returns 'words'
foobar.pluralize('goose') # returns 'geese'
foobar.singularize('phenomena') # returns 'phenomenon' 
```
-->

## Contributing
Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are greatly appreciated.
Make a Pull requests for any changes. For major changes, please open an issue first to discuss what you would like to change.
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/NewFeature`)
3. Commit your Changes (`git commit -m 'Add some NewFeature'`)
4. Push to the Branch (`git push origin feature/NewFeature`)
5. Open a Pull Request



## Demos

To-Do



## References
>[YOLO](https://pjreddie.com/darknet/yolo/): Real-Time Object Detection

>[AlexeyAB](https://github.com/AlexeyAB/darknet)


## License
[MIT](https://choosealicense.com/licenses/mit/)




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/vishxl/Mask-Mistakes?style=flat-square
[contributors-url]: https://github.com/github_username/repo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/vishxl/Mask-Mistakes?style=flat-square
[forks-url]: https://github.com/vishxl/Mask-Mistakes/network
[stars-shield]: https://img.shields.io/github/stars/vishxl/Mask-Mistakes?style=flat-square
[stars-url]: https://github.com/vishxl/Mask-Mistakes/stargazers
[issues-shield]: https://img.shields.io/github/issues/vishxl/Mask-Mistakes?style=flat-square
[issues-url]: https://github.com/vishxl/Mask-Mistakes/issues
[license-shield]: https://img.shields.io/github/license/vishxl/Mask-Mistakes?style=flat-square
[license-url]: https://github.com/vishxl/Mask-Mistakes

<!--[product-screenshot]: images/screenshot.png -->


