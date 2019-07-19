clearTopHalf(picture){
  width = getWidth(picture);
  height = getHeight(picture);
  halfHeight = height / 2;

  whiteBlock = createRectangle(width, halfHeight, white); <!-- creates white rectangle -->
  pictureParts = splitPicture(0, halfHeight); <!-- splits picture into 2 parts - into array -->
  pictureParts.first().replace(whiteBlock); <!-- replaces first item of array (first part of picture) with white rectangle -->

  return pictureParts; <!-- returns array with first part replaced -->

}


functions:

getWidth(element)
getHeight(element)
createRectangle(width, height, colour)
splitPicture(pointToSplit-x, pointToSplit-y)
first()
replace(newItem)