<h1 align="center">
  <br>
    <img src="icon.png" alt="logo" width="200">
  <br><br>
  Icons
  <br>
  <br>
</h1>

<p align="center">

This is the **light version** of the *@tal7aouy* VS Code icons. You can easly download it from the VS Code marketplace and use it with dark theme's to view those icons easly. In case of questions or propositions open an issue. 

<h2 align="center">Personalisation</h2>

To do a color personalization, run this script in the folder with all the svgs, it will replace the color with the new color :

```js
const fs = require('fs');

fs.readdir('.', (err, files) => {
    if (err) {
        throw err
    }
  
    files.forEach(file => {
        if (file.endsWith('.svg') && file.startsWith('folder')) {
            fs.readFile(file, 'utf8', function(err, data){
                // write datas
                var newData = data.replace("#f5f5f5", "YOUR_COLOR");
                fs.writeFile(file, newData, (err) => {
                    if (err)
                      console.log(err);
                });
            });
        }
    })
})
```

<h2 align="center">Contributors</h2>
</p>

| ***@titi_2115*** | ***@tal7aouy***
| - | - |
| ![image](https://avatars.githubusercontent.com/u/73474137?v=4) | ![image](https://avatars.githubusercontent.com/u/79597452?v=4)
