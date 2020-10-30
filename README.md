# Histogram-equalization-from-scratch

The histogram equalization is an approach to enhance a given image. Histogram Equalisation is a technique to adjust contrast levels and expand the intensity range in a digital image. Thus, it enhances the image which makes information extraction and further image processing easier.

ALGORITHUM:
  Compute a scaling factor -> α= 255 i.e number of pixels
  Calculate histogram of the image
  Create a CF table  with
      CF[0] =  α * histogram[0]  //Find frequency of occurrence for each pixel value i.e. histogram of an image (values lie in the range [0, 255] for any grayscale image)
Calculate Cumulative frequency of all pixel v
  for all remaining grey levels, i, do
     CF[i] = CF[i-1] + α * histogram[i]
  end for
  for all pixel coordinates, x and  y, do
      g(x, y) = CF[f(x, y)]
  end for
  
  
  
  
