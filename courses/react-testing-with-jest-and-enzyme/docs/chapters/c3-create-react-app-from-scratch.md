# Como crear una applicion React



[Ver en detalle](https://medium.com/@JedaiSaboteur/creating-a-react-app-from-scratch-f3c693b84658)


```cmd 
    npm i -D jest babel-jest
```

## babel-jest

Esta libreria es para habilitar el soporte con `Jest` ya que `babel` es usado para transformar nuestro javascript.

## configuracion



```js
// jest.config.js

const assetsPath = require.resolve("./test/file-mock.js");
const stylesPath = require.resolve("./test/style-mock.js");

module.exports = {
  moduleNameMapper: {
    "\\.(jpg|jpeg|png|gif|eot|otf|webp|svg|ttf|woff|woff2|mp4|webm|wav|mp3|m4a|aac|oga)$": assetsPath,
    "\\.(css|less)$": stylesPath,
  },
}
```

[Documentacion: moduleNameMapper](https://jestjs.io/es-ES/docs/configuration#modulenamemapper-objectstring-string--arraystring)

```batch
    mkdir __mock__
    touch ./ __mock__/fileMock.js
    echo "module.exports = 'test-file-stub';" >> ./__mock__/fileMock.js
```

# DOCUMENTATION PENDING