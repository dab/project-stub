# Minimal setup to start a new [BEM](https://bem.info) project

![](https://mc.yandex.ru/watch/27701205)

<!-- Yandex.Metrika counter -->
<script type="text/javascript">
    (function (d, w, c) {
        (w[c] = w[c] || []).push(function() {
            try {
                w.yaCounter27701205 = new Ya.Metrika({
                    id:27701205,
                    webvisor:true
                });
            } catch(e) { }
        });

        var n = d.getElementsByTagName("script")[0],
            s = d.createElement("script"),
            f = function () { n.parentNode.insertBefore(s, n); };
        s.type = "text/javascript";
        s.async = true;
        s.src = (d.location.protocol == "https:" ? "https:" : "http:") + "//mc.yandex.ru/metrika/watch.js";

        if (w.opera == "[object Opera]") {
            d.addEventListener("DOMContentLoaded", f, false);
        } else { f(); }
    })(document, window, "yandex_metrika_callbacks");
</script>
<noscript><div><img src="//mc.yandex.ru/watch/27701205" style="position:absolute; left:-9999px;" alt="" /></div></noscript>
<!-- /Yandex.Metrika counter -->

This repository contains the *minimal* configuration-files and folders you will need to create a [BEM](http://bem.info) project from *scratch*.

---

## Installation Requirements:

- [node.js](http://nodejs.org/)

You may also consider [installing bem-tools locally to your environment](http://bem.info/tools/bem/installation/) for [ease of use](#an-easier-more-beautiful-way), though it is **not required**

---

## Installation:

So, how easy is it to get started with BEM?  *Super easy*.

It's as easy as...

1. ›`git clone git://github.com/bem/project-stub.git`
2. ›`cd project-stub`
3. ›`npm i`
4. ›`./node_modules/.bin/bem server`

*(hint: execute the above commands in your terminal)*

Now that `bem server` is running, check it out:

````
Navigate to: http://localhost:8080/desktop.bundles/index/index.html
````

(here, have a link: [http://localhost:8080/desktop.bundles/index/index.html](http://localhost:8080/desktop.bundles/index/index.html))

---

**That's it, it's that simple. Congratulations, your BEM project is already underway!**

---

### Was that too easy?

Here's the replay... that `npm i` command will:

1. Install a **local copy** of all required dependencies from [npm](http://npmjs.org/) into the `./node_modules` directory. (specifically: [bem-tools](http://github.com/bem/bem-tools))
2. Install `bower` dependencies.

#### Note:

What do we mean by "a **local copy** of all required dependencies"?

Well, when you run the `npm i` command, we install all of the required dependencies ([bem-tools](http://github.com/bem/bem-tools))
to the `./node_modules` directory within the **local project directory**.  This is *not* the same thing as
[installing bem-tools locally to your environment](http://bem.info/tools/bem/installation/).  This is by far the easiest, quickest way to use
[bem-tools](http://github.com/bem/bem-tools) in [a more beautiful way](#an-easier-more-beautiful-way).

---

## Usage:

### Start the Server:

    › ./node_modules/.bin/bem server

This is the ugly way to run the `bem server` command.  If you think it's ugly too and wish for [a better way](#an-easier-more-beautiful-way) keep reading...

### An Easier, More Beautiful Way:

Once you have either (a) [fixed your PATH environment variable](#fix-your-path-environment-variable), or (b)
[properly installed bem-tools to your local environment](http://bem.info/tools/bem/installation/).
You may now, more elegantly, start your `bem server` by running:

    › bem server

---

### Stopping the Server:

Stopping the server is also easy:

    [ctrl] + [c]

Pressing `[ctrl] + [c]` while the terminal is your active window will stop the server.

---

### Fix your PATH environment variable:

For a more permanent way to "easily" use the *local-to-this-project's* installation of
[bem-tools](http://github.com/bem/bem-tools) all you must do is ensure that the **path** to the `bem` executable
(`./node_modules/.bin`) is included in your `PATH` environment variable.

    > export PATH=./node_modules/.bin:$PATH

Optionally you may also add `export PATH=PATH_TO_PROJECT_DIRECTORY/node_modules/.bin:$PATH` to your `.profile`
(obviously replacing `PATH_TO_PROJECT_DIRECTORY` with the actual path to your project)

---

[BEM](http://bem.info) is an abbreviation for Block-Element-Modifier.  [BEM](http://bem.info) is a way to write code which is easy to support and develop.

For more information about the BEM metodology check out [http://bem.info](http://bem.info/).
