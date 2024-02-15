
# Try Vision Cognitive Azure 🚀

This repository is to store the data and the result from the use of some of the tools that are available in the Vision Cognitive Azure Portal.

Vision Studio is a set of UI-based tools that lets you explore, build, and integrate features from Azure AI Vision. Vision Studio lets you try several service features and sample their returned data in a quick, straightforward manner.


## Input Image 🖖

All the results are based in the same input image below.

![alt text](https://github.com/amandagrams/vision.cognitive.azure/blob/main/inputs/may4.png?raw=true)


## Results  👏

### Tagging Images Service

![](https://github.com/amandagrams/vision.cognitive.azure/blob/main/output/may4-tagging.png?raw=true)

```Json
{
    "apim-request-id": "1a6dafda-f09c-4fc3-91cd-6efd22f5d82e",
    "content-length": "355",
    "content-type": "application/json; charset=utf-8",
    "modelVersion": "2023-10-01",
    "metadata": {
      "width": 743,
      "height": 562
    },
    "tagsResult": {
      "values": [
        {
          "name": "mammal",
          "confidence": 0.9413042068481445
        },
        {
          "name": "yoda",
          "confidence": 0.9171218872070312
        },
        {
          "name": "cartoon",
          "confidence": 0.9078869223594666
        },
        {
          "name": "poster",
          "confidence": 0.8990607261657715
        },
        {
          "name": "fictional character",
          "confidence": 0.8579978942871094
        }
      ]
    }
  }
```
### Face Detection Service

![](https://github.com/amandagrams/vision.cognitive.azure/blob/main/output/may4-face-detection.png?raw=true)


```Json
[
  {
    "recognitionModel": "recognition_01",
    "faceRectangle": {
      "width": 148,
      "height": 184,
      "left": 213,
      "top": 99
    },
    "faceLandmarks": {
      "pupilLeft": {
        "x": 263.8,
        "y": 174.1
      },
      "pupilRight": {
        "x": 338.1,
        "y": 188.4
      },
      "noseTip": {
        "x": 303.4,
        "y": 199.3
      },
      "mouthLeft": {
        "x": 260.5,
        "y": 231.1
      },
      "mouthRight": {
        "x": 320.2,
        "y": 242.8
      },
      "eyebrowLeftOuter": {
        "x": 240.7,
        "y": 153.5
      },
      "eyebrowLeftInner": {
        "x": 288,
        "y": 156.4
      },
      "eyeLeftOuter": {
        "x": 250.9,
        "y": 173.2
      },
      "eyeLeftTop": {
        "x": 265.1,
        "y": 169.6
      },
      "eyeLeftBottom": {
        "x": 262.7,
        "y": 177.6
      },
      "eyeLeftInner": {
        "x": 276.6,
        "y": 176.1
      },
      "eyebrowRightInner": {
        "x": 324.5,
        "y": 164.1
      },
      "eyebrowRightOuter": {
        "x": 362.7,
        "y": 177.2
      },
      "eyeRightInner": {
        "x": 326.4,
        "y": 186.1
      },
      "eyeRightTop": {
        "x": 339,
        "y": 183.5
      },
      "eyeRightBottom": {
        "x": 337.7,
        "y": 191.6
      },
      "eyeRightOuter": {
        "x": 349.2,
        "y": 192.3
      },
      "noseRootLeft": {
        "x": 292.3,
        "y": 177.1
      },
      "noseRootRight": {
        "x": 314.1,
        "y": 180.2
      },
      "noseLeftAlarTop": {
        "x": 285.7,
        "y": 192.3
      },
      "noseRightAlarTop": {
        "x": 316.9,
        "y": 197.7
      },
      "noseLeftAlarOutTip": {
        "x": 276.1,
        "y": 202.3
      },
      "noseRightAlarOutTip": {
        "x": 321.2,
        "y": 211.1
      },
      "upperLipTop": {
        "x": 296.4,
        "y": 227.4
      },
      "upperLipBottom": {
        "x": 293.8,
        "y": 233.1
      },
      "underLipTop": {
        "x": 292.9,
        "y": 237.1
      },
      "underLipBottom": {
        "x": 291.3,
        "y": 245.2
      }
    },
    "faceAttributes": {
      "mask": {
        "type": "noMask",
        "noseAndMouthCovered": false
      }
    }
  }
]
```

### Extract text from images

![](https://github.com/amandagrams/vision.cognitive.azure/blob/main/output/may4-extract-text-from-image.png?raw=true)


```Json
[
    {
      "lines": [
        {
          "text": "MAY THE 4TH",
          "boundingPolygon": [
            {
              "x": 228,
              "y": 12
            },
            {
              "x": 507,
              "y": 12
            },
            {
              "x": 508,
              "y": 63
            },
            {
              "x": 228,
              "y": 63
            }
          ],
          "words": [
            {
              "text": "MAY",
              "boundingPolygon": [
                {
                  "x": 229,
                  "y": 12
                },
                {
                  "x": 320,
                  "y": 13
                },
                {
                  "x": 320,
                  "y": 64
                },
                {
                  "x": 228,
                  "y": 64
                }
              ],
              "confidence": 0.999
            },
            {
              "text": "THE",
              "boundingPolygon": [
                {
                  "x": 330,
                  "y": 13
                },
                {
                  "x": 410,
                  "y": 13
                },
                {
                  "x": 411,
                  "y": 64
                },
                {
                  "x": 330,
                  "y": 64
                }
              ],
              "confidence": 0.995
            },
            {
              "text": "4TH",
              "boundingPolygon": [
                {
                  "x": 421,
                  "y": 13
                },
                {
                  "x": 500,
                  "y": 13
                },
                {
                  "x": 501,
                  "y": 64
                },
                {
                  "x": 421,
                  "y": 64
                }
              ],
              "confidence": 0.999
            }
          ]
        },
        {
          "text": "BE WITH YOU",
          "boundingPolygon": [
            {
              "x": 231,
              "y": 427
            },
            {
              "x": 514,
              "y": 427
            },
            {
              "x": 514,
              "y": 478
            },
            {
              "x": 231,
              "y": 477
            }
          ],
          "words": [
            {
              "text": "BE",
              "boundingPolygon": [
                {
                  "x": 234,
                  "y": 427
                },
                {
                  "x": 285,
                  "y": 427
                },
                {
                  "x": 282,
                  "y": 478
                },
                {
                  "x": 232,
                  "y": 478
                }
              ],
              "confidence": 0.993
            },
            {
              "text": "WITH",
              "boundingPolygon": [
                {
                  "x": 294,
                  "y": 428
                },
                {
                  "x": 408,
                  "y": 429
                },
                {
                  "x": 405,
                  "y": 477
                },
                {
                  "x": 292,
                  "y": 478
                }
              ],
              "confidence": 0.993
            },
            {
              "text": "YOU",
              "boundingPolygon": [
                {
                  "x": 424,
                  "y": 429
                },
                {
                  "x": 506,
                  "y": 431
                },
                {
                  "x": 504,
                  "y": 476
                },
                {
                  "x": 422,
                  "y": 477
                }
              ],
              "confidence": 0.994
            }
          ]
        },
        {
          "text": "YOUNG PADAWAN",
          "boundingPolygon": [
            {
              "x": 182,
              "y": 482
            },
            {
              "x": 564,
              "y": 484
            },
            {
              "x": 563,
              "y": 536
            },
            {
              "x": 182,
              "y": 535
            }
          ],
          "words": [
            {
              "text": "YOUNG",
              "boundingPolygon": [
                {
                  "x": 183,
                  "y": 483
                },
                {
                  "x": 329,
                  "y": 485
                },
                {
                  "x": 328,
                  "y": 536
                },
                {
                  "x": 183,
                  "y": 536
                }
              ],
              "confidence": 0.994
            },
            {
              "text": "PADAWAN",
              "boundingPolygon": [
                {
                  "x": 340,
                  "y": 486
                },
                {
                  "x": 555,
                  "y": 489
                },
                {
                  "x": 553,
                  "y": 535
                },
                {
                  "x": 339,
                  "y": 536
                }
              ],
              "confidence": 0.993
            }
          ]
        }
      ]
    }
  ]
```

### Common Object Detection

![](https://github.com/amandagrams/vision.cognitive.azure/blob/main/output/may4-common-objects-detecction.png?raw=true)


```Json
{
    "apim-request-id": "cb772064-eaf1-46f7-a8c6-52a68dcf0496",
    "content-length": "191",
    "content-type": "application/json; charset=utf-8",
    "modelVersion": "2023-10-01",
    "metadata": {
      "width": 743,
      "height": 562
    },
    "objectsResult": {
      "values": [
        {
          "boundingBox": {
            "x": 97,
            "y": 64,
            "w": 374,
            "h": 495
          },
          "tags": [
            {
              "name": "primate",
              "confidence": 0.611
            }
          ]
        }
      ]
    }
  }
```

### Generate captions for an image

![](https://github.com/amandagrams/vision.cognitive.azure/blob/main/output/may4-add-captions-image.png?raw=true)


```Json
{
    "apim-request-id": "fc64d5a4-cc0f-4212-9235-1de739b46b50",
    "content-length": "176",
    "content-type": "application/json; charset=utf-8",
    "modelVersion": "2023-10-01",
    "captionResult": {
      "text": "a green alien with long green ears and green eyes",
      "confidence": 0.5991348624229431
    },
    "metadata": {
      "width": 743,
      "height": 562
    }
  }
```
## Reference 📖

 - [Analyze images in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html)
 - [Detect faces in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html)
 - [Read text in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)


## Authors 👽

- [@amandagrams](https://github.com/amandagrams)

