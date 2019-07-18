<!-- HTML body -->
```
<div class="img__container">
    <canvas class="canvas" id="canvas" style="position: fixed;"></canvas>
    <img src="../assets/alan_kay.jpg" alt="original photo" class="photo">
  </div>
<script src="index.js"></script>
```

<!-- JavaScript -->
```
const canvas = document.getElementById('canvas');
const photo = document.querySelector('.photo');
let context;

if (canvas.getContext) {
  context = canvas.getContext('2d');
};

const clearTopHalf = picture => {
  console.log(context);
  context.canvas.width = picture.width;
  context.canvas.height = (picture.height / 2);
  context.fillStyle = 'rgb(255, 255, 255)';
  context.fillRect(0, 0, picture.width, (picture.height / 2));
};

clearTopHalf(photo);
```