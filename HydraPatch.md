# Hydra code

s0.initVideo("https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExcDBsNTVtNWl1c294YjM2cGxrZzlqcmFkMGV1aWdpazN4MGxteXliNSZlcD12MV9naWZzX3NlYXJjaCZjdD1n/120rj8R058kOHe/giphy.mp4")
src(s0).color(1)
  .saturate(20)
  .pixelate(3000, 3000)
  .colorama(0.1)
  .posterize(100)
  .brightness(0.2)
  .luma(0.8)
  .thresh(0.5)
.add(voronoi(1000))
.add(shape(100, 0.2, 0.5).color(4))
.out(o0)




Thoughts:

Very very angry pixelated monkey trying to eat the red shape infront of it. I feel really intrigues by this software, lots of visual potential, but I really hope I learn to do video in video, it would be super helpful. I still don't know how to get a video inside the red shape.