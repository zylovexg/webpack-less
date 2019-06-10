## npm install
## npm run dev 或者 npm run build

### 步骤：
#### 安装 npm i -d less less-loader
#### webpack 配置
```javascript
  module.exports = {
    module: {
      rules: [
        {
          test: /\.less$/,
          use: [MiniCssExtractPlugin.loader, 'css-loader', 'less-loader']
        }
      ]
    }
  }
```