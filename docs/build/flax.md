


<a id='Flax.prepare_template' href='#Flax.prepare_template'>#</a>
**`Flax.prepare_template`** &mdash; *Function*.



```
prepare_template(s::String)
prepare_template{T}(v::Vector{T})
```

Cleans up the template before rendering (ex by removing empty nodes).


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L41-L46' class='documenter-source'>source</a><br>

<a id='Flax.attributes' href='#Flax.attributes'>#</a>
**`Flax.attributes`** &mdash; *Function*.



```
attributes(attrs::Vector{Pair{Symbol,String}} = Vector{Pair{Symbol,String}}()) :: Vector{String}
```

Parses HTML attributes.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L58-L62' class='documenter-source'>source</a><br>

<a id='Flax.normal_element' href='#Flax.normal_element'>#</a>
**`Flax.normal_element`** &mdash; *Function*.



```
normal_element(f::Function, elem::String, attrs::Vector{Pair{Symbol,String}} = Vector{Pair{Symbol,String}}()) :: HTMLString
```

Generates a regular HTML element in the form <...></...>


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L77-L81' class='documenter-source'>source</a><br>

<a id='Flax.void_element' href='#Flax.void_element'>#</a>
**`Flax.void_element`** &mdash; *Function*.



```
void_element(elem::String, attrs::Vector{Pair{Symbol,String}} = Vector{Pair{Symbol,String}}()) :: HTMLString
```

Generates a void HTML element in the form <...>


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L94-L98' class='documenter-source'>source</a><br>

<a id='Flax.skip_element' href='#Flax.skip_element'>#</a>
**`Flax.skip_element`** &mdash; *Function*.





<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L106-L108' class='documenter-source'>source</a><br>

<a id='Flax.include_template' href='#Flax.include_template'>#</a>
**`Flax.include_template`** &mdash; *Function*.



```
include_template(path::String; partial = true, func_name = "") :: String
```

Includes a template inside another.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L117-L121' class='documenter-source'>source</a><br>

<a id='Flax.html' href='#Flax.html'>#</a>
**`Flax.html`** &mdash; *Function*.



```
html(resource::Symbol, action::Symbol, layout::Symbol; vars...) :: Dict{Symbol,String}
```

Renders a HTML view corresponding to a resource and a controller action.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L165-L169' class='documenter-source'>source</a><br>

<a id='Flax.flax' href='#Flax.flax'>#</a>
**`Flax.flax`** &mdash; *Function*.



```
flax(resource::Symbol, action::Symbol, layout::Symbol; vars...) :: Dict{Symbol,String}
```

Renders a Flax view corresponding to a resource and a controller action.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L186-L190' class='documenter-source'>source</a><br>

<a id='Flax.json' href='#Flax.json'>#</a>
**`Flax.json`** &mdash; *Function*.



```
json(resource::Symbol, action::Symbol; vars...) :: Dict{Symbol,String}
```

Renders a JSON view corresponding to a resource and a controller action.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L227-L231' class='documenter-source'>source</a><br>

<a id='Flax.function_name' href='#Flax.function_name'>#</a>
**`Flax.function_name`** &mdash; *Function*.



```
function_name(file_path::String)
```

Generates random functions names for generated Flax views functions.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L247-L251' class='documenter-source'>source</a><br>

<a id='Flax.html_to_flax' href='#Flax.html_to_flax'>#</a>
**`Flax.html_to_flax`** &mdash; *Function*.



```
html_to_flax(file_path::String; partial = true) :: String
```

Converts a HTML document to a Flax document.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L258-L262' class='documenter-source'>source</a><br>

<a id='Flax.read_template_file' href='#Flax.read_template_file'>#</a>
**`Flax.read_template_file`** &mdash; *Function*.



```
read_template_file(file_path::String) :: String
```

Reads `file_path` template from disk.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L273-L277' class='documenter-source'>source</a><br>

<a id='Flax.parse_template' href='#Flax.parse_template'>#</a>
**`Flax.parse_template`** &mdash; *Function*.



```
parse_template(file_path::String; partial = true) :: String
```

Parses a HTML file into a `string` of Flax code.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L290-L294' class='documenter-source'>source</a><br>

<a id='Flax.parse_tree' href='#Flax.parse_tree'>#</a>
**`Flax.parse_tree`** &mdash; *Function*.



```
parse_tree(elem, output, depth; partial = true) :: String
```

Parses a Gumbo tree structure into a `string` of Flax code.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L301-L305' class='documenter-source'>source</a><br>

<a id='Flax.parse_tags' href='#Flax.parse_tags'>#</a>
**`Flax.parse_tags`** &mdash; *Function*.



```
parse_tags(line::Tuple{Int64,String}, strip_close_tag = false) :: String
```

Parses special Flax tags.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L379-L383' class='documenter-source'>source</a><br>

<a id='Flax.doctype' href='#Flax.doctype'>#</a>
**`Flax.doctype`** &mdash; *Function*.



```
doctype(doctype::Symbol = :html) :: String
```

Outputs document's doctype.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L394-L398' class='documenter-source'>source</a><br>

<a id='Flax.doc' href='#Flax.doc'>#</a>
**`Flax.doc`** &mdash; *Function*.



```
doc(html::String) :: String
doc(doctype::Symbol, html::String) :: String
```

Outputs document's doctype.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L404-L409' class='documenter-source'>source</a><br>

<a id='Flax.register_elements' href='#Flax.register_elements'>#</a>
**`Flax.register_elements`** &mdash; *Function*.



```
register_elements() :: Void
```

Generated functions that represent Flax functions definitions corresponding to HTML elements.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L418-L422' class='documenter-source'>source</a><br>

<a id='Flax.include_helpers' href='#Flax.include_helpers'>#</a>
**`Flax.include_helpers`** &mdash; *Function*.



```
include_helpers() :: Void
```

Loads helpers and makes them available in the view layer.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L456-L460' class='documenter-source'>source</a><br>

<a id='Flax.foreachvar' href='#Flax.foreachvar'>#</a>
**`Flax.foreachvar`** &mdash; *Function*.



```
foreachvar(f::Function, key::Symbol, v::Vector) :: String
```

Utility function for looping over a `vector` `v` in the view layer.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L472-L476' class='documenter-source'>source</a><br>

<a id='Flax.var_dump' href='#Flax.var_dump'>#</a>
**`Flax.var_dump`** &mdash; *Function*.



```
var_dump(var, html = true) :: String
```

Utility function for dumping a variable.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/cd856af895899e61998c7e9a0a8ee655a5d8311c/src/Flax.jl#L499-L503' class='documenter-source'>source</a><br>

