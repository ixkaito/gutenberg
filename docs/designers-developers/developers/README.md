<!-- # Developer Documentation -->
# 開発者ドキュメント

<!-- The new editor is highly flexible, like most of WordPress. You can build custom blocks, modify the editor's appearance, add special plugins, and much more. -->
WordPress の大部分と同様に、新しいエディタは非常に柔軟です。カスタムブロックを構築したり、エディターの見た目を変更したり、独自のプラグインを追加したりすることができます。他にもたくさんあります。

<!-- ## Creating Blocks -->
## ブロックの作成

<!-- The editor is about blocks, and the main extensibility API is the Block API. It allows you to create your own static blocks, [Dynamic Blocks](/docs/designers-developers/developers/tutorials/block-tutorial/creating-dynamic-blocks.md) ( rendered on the server ) and also blocks capable of saving data to Post Meta for more structured content. -->
このエディターの本質はブロックであり、最も重要な拡張 API はブロック API です。独自の静的ブロック、[動的ブロック](/docs/designers-developers/developers/tutorials/block-tutorial/creating-dynamic-blocks.md) (サーバ上でレンダリングされる) 、または構造化されたコンテンツのために、投稿メタにデータを保存できるブロックを、あなた自身で作ることを可能にしてくれます。

<!-- If you want to learn more about block creation, the [Blocks Tutorial](/docs/designers-developers/developers/tutorials/block-tutorial/readme.md) is the best place to start. -->
ブロック作成についてもっと詳しく知りたい場合は、[ブロックチュートリアル](/docs/designers-developers/developers/tutorials/block-tutorial/readme.md)から始めるのがもっともよいでしょう。

<!-- ## Extending Blocks -->
## ブロックの拡張

It is also possible to modify the behavior of existing blocks or even remove them completely using filters.

Learn more in the [Block Filters](/docs/designers-developers/developers/filters/block-filters.md) section.

<!-- ## Extending the Editor UI -->
## エディター UI の拡張

Extending the editor UI can be accomplished with the `registerPlugin` API, allowing you to define all your plugin's UI elements in one place.

Refer to the [Plugins](/packages/plugins/README.md) and [Edit Post](/packages/edit-post/README.md) section for more information.

You can also filter certain aspects of the editor; this is documented on the [Editor Filters](/docs/designers-developers/developers/filters/editor-filters.md) page.

<!-- ## Meta Boxes -->
## メタボックス

Porting PHP meta boxes to blocks or sidebar plugins is highly encouraged, learn how through these [meta data tutorials](/docs/designers-developers/developers/tutorials/metabox/readme.md).

See how the new editor [supports existing Meta Boxes](/docs/designers-developers/developers/backward-compatibility/meta-box.md).

<!-- ## Theme Support -->
## テーマサポート

By default, blocks provide their styles to enable basic support for blocks in themes without any change. Themes can add/override these styles, or rely on defaults.

There are some advanced block features which require opt-in support in the theme. See [theme support](/docs/designers-developers/developers/themes/theme-support.md).

<!-- ## Autocomplete -->
## オートコンプリート

Autocompleters within blocks may be extended and overridden. Learn more about the [autocomplete](/docs/designers-developers/developers/filters/autocomplete-filters.md) filters.

<!-- ## Block Parsing and Serialization -->
## Block Parsing and Serialization

Posts in the editor move through a couple of different stages between being stored in `post_content` and appearing in the editor. Since the blocks themselves are data structures that live in memory it takes a parsing and serialization step to transform out from and into the stored format in the database.

Customizing the parser is an advanced topic that you can learn more about in the [Extending the Parser](/docs/designers-developers/developers/filters/parser-filters.md) section.
