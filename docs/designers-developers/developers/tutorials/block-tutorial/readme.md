<!-- # Blocks -->
# ブロック

<!-- The purpose of this tutorial is to step through the fundamentals of creating a new block type. Beginning with the simplest possible example, each new section will incrementally build upon the last to include more of the common functionality you could expect to need when implementing your own block types. -->
このチュートリアルの目的は、新しいブロックタイプを作成するための基礎を学ぶことです。もっともシンプルな例から始め、各セクションで徐々にステップアップし、最終的には独自のブロックタイプを実装するときに必要になると思われる一般的な機能を盛り込んでいます。

<!-- To follow along with this tutorial, you can [download the accompanying WordPress plugin](https://github.com/WordPress/gutenberg-examples) which includes all of the examples for you to try on your own site. At each step along the way, you should feel free to experiment by modifying the examples with your own ideas and observing the effects they have on the block's behavior. -->
このチュートリアルに沿って進めるにあたり、あなた自身のサイトで試すためのすべての例を含んだ[添付の WordPress プラグインをダウンロード](https://github.com/WordPress/gutenberg-examples)できます。途中の各ステップで、you should feel free to experiment by modifying the examples with your own ideas and observing the effects they have on the block's behavior.

<!-- Code snippets are provided both for "classic" JavaScript (ECMAScript 5, or "ES5"), as well as newer versions of the language standard (ES2015 and newer, or "ESNext"). You can change between them using tabs found above each code example. When choosing to author your blocks with ESNext, you need to run [the JavaScript build step](/docs/designers-developers/developers/tutorials/javascript/js-build-setup/) in order to support older browsers. -->
Code snippets are provided both for "classic" JavaScript (ECMAScript 5, or "ES5"), as well as newer versions of the language standard (ES2015 and newer, or "ESNext"). You can change between them using tabs found above each code example. When choosing to author your blocks with ESNext, you need to run [the JavaScript build step](/docs/designers-developers/developers/tutorials/javascript/js-build-setup/) in order to support older browsers.

<!-- Note that it is not required to use ESNext to create a new block, and you are welcome to use classic JavaScript if you so choose. -->
Note that it is not required to use ESNext to create a new block, and you are welcome to use classic JavaScript if you so choose.
