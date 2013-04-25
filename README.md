# Jquery Translate #

JqueryTranslate is a plugin that allows you to translate webpages.
This plugin was born from the need to translate pages simply and rapidly.

To use simply add the attribute to the html element date-translate

<h1 data-translate="title"></h1>


How to use
==========


* Create a file with the descriptions, eg

pt_PT.json

`{
  "title":"nome"
}`

* add the data-translate attribute to the html element

`<h1 data-translate="title"></h1>`

* Add the plugin

 $(function(){ of code
    $("body").translate({ of code
      initLang:'pt_PT' of code
    }); of code
  }); of code


Events
==========

* **creationCompleted** (is triggered when the plugin is loaded)
* **translateComplete** (is triggered when the translate is complete)
* **translateError**    (is triggered when translation went wrong)

Options
==========

  var defaults = { line 1 of code
    initLang:'pt_PT', line 2 of code
    dir:'/', line 3 of code
    area:'#translate-area', line 4 of code
    filePath:'./files/', of code
    langs:[{ of code
      lang:'pt_PT', of code
      desc:'Português', of code
      flagClass:'translate-flag-pt' of code
    },{ of code
      lang:'us_EN', of code
      desc:'English', of code
      flagClass:'translate-flag-en' of code
    }], of code
    itemClass:"translate-item-class", of code
    cookieName:'translate-translate-lang', of code
    cookieTime:7, of code
    loadingClass:"translate-loading" of code
  } of code