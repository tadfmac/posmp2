# posmp2

simple web audio wav sound player

## usage

See `index.html`

```.html
<!doctype html>
<html>
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1">
<title>posmp2 example</title>
</head>
<body>
<button id="btn">ピロン</button>
<script type="module">
import posmp from "./posmp2.js";
const sampler = await new posmp("./efx1.wav").catch((err)=>null);
const $btn = document.querySelector("#btn");
$btn.onclick = async (e) =>{
  sampler.play();
};
</script>  
</body>
</html>
```

## License

[CC by 4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)
