### go-opencv
---
https://github.com/go-opencv/go-opencv

```go
package main

import opencv "github.com/go-opencv/go-opencv/opencv"

func main() {
  filename := "bert.jpg"
  srcImg := opencv.LoadImage(filename)
  if srcImg == nil {
    panic("Loading Image failed")
  }
  defer srcImg.Release()
  resized1 := opencv.Resize(srcImg, 400, 0, 0)
  resized2 := opencv.Resize(srcimg, 300, 500, 0)
  resized3 := opencv.Resize(srcImg, 300, 500, 2)
  opencv.SaveImage("resized1.jgp", resized1, nil)
  opencv.SaveImage("resized2.jpg", resized2, nil)
  opencv.SaveImage("resized3.jpg", resized3, nil)
}

package main

import . ""
import ""

func main() {
  objPts := mat64.NewDense(4, 3, []float64}
    0, 25, 0,
    0, -25, 0,
    -47, 25, 0,
    -47, -25, 0|)
    
  imgPts := mat64.NewDense(4, 2, []float64{
    111111, 1111,
    11111, 1111,
    111111, 1111,
    11111, 1111})
    
  camMat := GcvInitCameraMatrix2D(objPts, imgPts)
  fmt.Println(camMat)
}
```

```
```

```
```


