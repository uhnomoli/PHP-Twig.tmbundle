# PHP Twig tmBundle

A [TextMate][textmate] _(and [Sublime Text][sublime])_ bundle for [Twig][twig].


### Thanks

I'd like to thank a few people that have helped me out with the creation of this bundle.

* __taavi__ for fixing a bug stopping the bundle from actually working in TextMate.
* __DuoSRX__ for contributing a bunch of snippets.
* __Infininight__ in __##textmate__ _(freenode)_ for helping me a ton with the rewrite.
* __csuarez__ for contributing an updated theme.


### Notes

This is my first tmbundle and it was made and tested in [Sublime Text][sublime]. Everything should work fine, but if something doesn't please report it and I'll do my best to get it fixed.

I'm also not extremely familiar with TextMate's method of creating language syntaxes. If anyone has any input on optimizing it or on anything else, such as choices in grammar scopes, please feel free to let me know.


### Installation

TextMate, and most editors that support TextMate bundles, allow the installation of bundles simply by extracting an archive or cloning the repository into the application's bundle directory. This bundle is no different. Below is a list of common bundle directories.


#### Sublime Text 2

Linux

    $XDG_CONFIG_HOME/sublime-text-2/Packages` or `~/.Sublime Text 2/Packages

OS X

    ~/Library/Application Support/Sublime Text 2/Packages

Windows

    %APPDATA%/Sublime Text 2/Packages/

#### TextMate

    /Library/Application Support/TextMate/Bundles


### Scopes

To aid theming, here's a list of what each Twig element is scoped to.

    Tags:
        {{ }}:
            Tag:       punctuation.section.tag.twig
            Scope:     meta.tag.template.value.twig
        {% %}:
            Tag:       punctuation.section.tag.twig
            Scope:     meta.tag.template.block.twig
        {# #}:         comment.block.twig
        Embedded:
            {{ }}:     meta.tag.inline.any.html meta.tag.template.value.twig
            {% %}:     meta.tag.inline.any.html meta.tag.template.block.twig
            
    Constants:
        Language:      constant.language.twig
        Numeric:       constant.numeric.twig
        
    Operators:
        Arithmetic:    keyword.operator.arithmetic.twig
        Assignment:    keyword.operator.assignment.twig
        Bitwise:       keyword.operator.bitwise.twig
        Comparison:    keyword.operator.comparison.twig
        Logical:       keyword.operator.logical.twig
        Other:         keyword.operator.other.twig
        
    Objects:           variable.other.twig
    Properties:        variable.other.property.twig
        Accessors:
            Dot:       punctuation.separator.property.twig
            Array:
                Begin: punctuation.section.array.begin.twig
                End:   punctuation.section.array.end.twig
                
    Strings:
        Single:        string.quoted.single.twig
        Double:        string.quoted.double.twig
    Arrays:            meta.array.twig
        Accessor:
            Begin:     punctuation.section.array.begin.twig
            End:       punctuation.section.array.end.twig
        Separator:     punctuation.separator.object.twig
    Hashes:            meta.hash.twig
        Accessor:
            Begin:     punctuation.section.hash.begin.twig
            End:       punctuation.section.hash.end.twig
        Separator:     punctuation.separator.object.twig
            Keys:      punctuation.separator.key-value.twig
            
    Keywords:          keyword.control.twig
    
    Functions:         support.function.twig
        Parens:
            Begin:     punctuation.definition.parameters.begin.twig
            End:       punctuation.definition.parameters.end.twig
        Arguments:     meta.function.arguments.twig
    Filters:           support.function.twig
        Parens:
            Begin:     punctuation.definition.parameters.begin.twig
            End:       punctuation.definition.parameters.end.twig
        Arguments:     meta.function.arguments.twig
        User-Defined:  meta.function-call.other.twig
    Macros:            meta.function-call.twig


### Extras

I included a few additional things in `/Extras`. There is a screenshot _(same one as displayed below)_ of the bundle in it's current state, as well as the 3 themes I'm maintaining, plus some user contributed ones, that were updated to better accompany this bundle.


### Screenshot
[![Preview][preview-thumb]][preview]


[sublime]: http://www.sublimetext.com/
[textmate]: http://macromates.com/
[twig]: http://www.twig-project.org/
[preview]: https://github.com/Anomareh/PHP-Twig.tmbundle/raw/master/Extras/Preview/preview.png

[preview-thumb]: https://github.com/Anomareh/PHP-Twig.tmbundle/raw/master/Extras/Preview/preview-thumb.png
