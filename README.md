# homepage
Homepage of Resec Yang

## doc-en
### File Structure and Purpose

- `_data/navigation.yml`: Responsible for navigation menu items.
- `_includes`: Stores HTML partials/templates.
- `_layouts`: Stores layout templates. Published posts can specify a layout; if none is specified, `default.html` is used by default.
- `_pages`: Stores written post pages, such as `about.md`, `404.md`, etc.
- `_sass`: Stores SCSS (Sass) style files such as `main.scss`, `_base.scss`, etc.
- `assets`: Stores stylesheets, fonts, and JavaScript files — considered as static resources.
- `images`: Stores image files, which can be referenced within written pages.
- `_config.yml`: Stores site configuration, such as site name, description, theme, related links, etc.
- `Gemfile`: Declares site dependencies.

### How to Modify

For simple changes, you can directly edit markdown files inside the `_pages` folder.  
For example, to edit the About page, just modify `about.md`.

To add a navigation link, you can create a new markdown file in the root directory and then configure `_data/navigation.yml` accordingly.

If you want to modify the page structure, start by looking at `default.html` inside the `_layouts` folder. However, it is recommended to make a copy first before editing.

If you want to modify the page styles, inspect files under `_includes` and `default.html` to locate the correct selectors. Then modify the corresponding style files in the `_sass` folder — or create a new SCSS file and include it in the layout template.

> Note: Markdown content is injected into the template with `{{ content }}`.  
> You can also use Liquid template code directly within markdown files.

> For a deeper understanding, refer to the official documentation of [Liquid template language](https://shopify.github.io/liquid/) and [Jekyll](https://jekyllrb.com/docs/).




## 中文版

### 文件结构及作用

- \_data/navigation.yml 负责导航
- \_includes 中存放html 模板文件
- \_layouts 中存放样式文件，在发布的post中可以选用不同的layout, 如果不指定则选用默认的 default.html
- \_pages 中存放写好的帖子 post，如about.md, 404.md等
- \_sass 中存放样式文件，如main.scss, _base.scss等
- assets 中存放样式、字体和js 脚本文件，属于是资源文件
- images 中存放图片文件,在 写好的帖子中可以引用
- \_config.yml 存放网站的配置信息，如网站名称、描述、主题、相关信息链接等等
- gemfile 存放网站的依赖包

### 修改方式
简单修改可以直接写入 _pages 文件夹下的 md 文件，如修改 about 页面，则直接修改 about.md 文件即可。

要加入导航页面链接，可以直接在根目录下加入md文件，之后配置_data/navigation.yml文件

如果需要修改页面结构，先从 _layouts 文件夹的 default.html 开始。但是建议先复制一份

如果想要修改页面样式，可以先观察\_includes 和 \_default.html 模板文件，找到对应的 选择器，在 \_sass 文件夹下修改对应的样式文件,或者直接新建 scss 文件, 在模板文件中引用就好
> 注：markdown 的内容在模板中插入为 {{ content }},
> 并且在 markdown 文件内也可以加入 liquid 代码）


> 想要详细了解，可以参考 liquid 模板语言的语法，以及 jekyll 的相关文档。
