# min-css-extract-plugin

假设 main.js 中引入了两个 css，如果用 css-loader + style-loader，那么打包的 css 会以 style 标签内联进 html 的 head 中

如果需要提取外链 css，可以用 min-css-extract-plugin

配置分为两步，第一步在 plugins 中新增 MiniCssExtractPlugin，第二步用 MiniCssExtractPlugin.loader 取代 style-loader
