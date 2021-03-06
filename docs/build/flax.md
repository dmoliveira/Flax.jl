

- [Genie / Flax](index.md#Genie-/-Flax-1)

<a id='Flax.prepare_template' href='#Flax.prepare_template'>#</a>
**`Flax.prepare_template`** &mdash; *Function*.



```
prepare_template(s::String)
prepare_template{T}(v::Vector{T})
```

Cleans up the template before rendering (ex by removing empty nodes).


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L41-L46' class='documenter-source'>source</a><br>

<a id='Flax.attributes' href='#Flax.attributes'>#</a>
**`Flax.attributes`** &mdash; *Function*.



```
attributes(attrs::Vector{Pair{Symbol,String}} = Vector{Pair{Symbol,String}}()) :: Vector{String}
```

Parses HTML attributes.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L58-L62' class='documenter-source'>source</a><br>

<a id='Flax.normal_element' href='#Flax.normal_element'>#</a>
**`Flax.normal_element`** &mdash; *Function*.



```
normal_element(f::Function, elem::String, attrs::Vector{Pair{Symbol,String}} = Vector{Pair{Symbol,String}}()) :: HTMLString
```

Generates a regular HTML element in the form <...></...>


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L77-L81' class='documenter-source'>source</a><br>

<a id='Flax.void_element' href='#Flax.void_element'>#</a>
**`Flax.void_element`** &mdash; *Function*.



```
void_element(elem::String, attrs::Vector{Pair{Symbol,String}} = Vector{Pair{Symbol,String}}()) :: HTMLString
```

Generates a void HTML element in the form <...>


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L94-L98' class='documenter-source'>source</a><br>

<a id='Flax.skip_element' href='#Flax.skip_element'>#</a>
**`Flax.skip_element`** &mdash; *Function*.



```
skip_element(f::Function) :: HTMLString
skip_element() :: HTMLString
```

Cleans up empty elements.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L106-L111' class='documenter-source'>source</a><br>

<a id='Flax.include_template' href='#Flax.include_template'>#</a>
**`Flax.include_template`** &mdash; *Function*.



```
include_template(path::String; partial = true, func_name = "") :: String
```

Includes a template inside another.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L120-L124' class='documenter-source'>source</a><br>

<a id='Flax.html' href='#Flax.html'>#</a>
**`Flax.html`** &mdash; *Function*.



```
html(resource::Symbol, action::Symbol, layout::Symbol; vars...) :: Dict{Symbol,String}
```

Renders a HTML view corresponding to a resource and a controller action.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L172-L176' class='documenter-source'>source</a><br>

<a id='Flax.flax' href='#Flax.flax'>#</a>
**`Flax.flax`** &mdash; *Function*.



```
flax(resource::Symbol, action::Symbol, layout::Symbol; vars...) :: Dict{Symbol,String}
```

Renders a Flax view corresponding to a resource and a controller action.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L192-L196' class='documenter-source'>source</a><br>

<a id='Flax.json' href='#Flax.json'>#</a>
**`Flax.json`** &mdash; *Function*.



```
json(resource::Symbol, action::Symbol; vars...) :: Dict{Symbol,String}
```

Renders a JSON view corresponding to a resource and a controller action.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L232-L236' class='documenter-source'>source</a><br>

<a id='Flax.function_name' href='#Flax.function_name'>#</a>
**`Flax.function_name`** &mdash; *Function*.



```
function_name(file_path::String)
```

Generates random functions names for generated Flax views functions.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L252-L256' class='documenter-source'>source</a><br>

<a id='Flax.html_to_flax' href='#Flax.html_to_flax'>#</a>
**`Flax.html_to_flax`** &mdash; *Function*.



```
html_to_flax(file_path::String; partial = true) :: String
```

Converts a HTML document to a Flax document.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L263-L267' class='documenter-source'>source</a><br>

<a id='Flax.read_template_file' href='#Flax.read_template_file'>#</a>
**`Flax.read_template_file`** &mdash; *Function*.



```
read_template_file(file_path::String) :: String
```

Reads `file_path` template from disk.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L278-L282' class='documenter-source'>source</a><br>

<a id='Flax.parse_template' href='#Flax.parse_template'>#</a>
**`Flax.parse_template`** &mdash; *Function*.



```
parse_template(file_path::String; partial = true) :: String
```

Parses a HTML file into a `string` of Flax code.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L295-L299' class='documenter-source'>source</a><br>

<a id='Flax.parse_tree' href='#Flax.parse_tree'>#</a>
**`Flax.parse_tree`** &mdash; *Function*.



```
parse_tree(elem, output, depth; partial = true) :: String
```

Parses a Gumbo tree structure into a `string` of Flax code.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L306-L310' class='documenter-source'>source</a><br>

<a id='Flax.parse_tags' href='#Flax.parse_tags'>#</a>
**`Flax.parse_tags`** &mdash; *Function*.



```
parse_tags(line::Tuple{Int64,String}, strip_close_tag = false) :: String
```

Parses special Flax tags.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L384-L388' class='documenter-source'>source</a><br>

<a id='Flax.doctype' href='#Flax.doctype'>#</a>
**`Flax.doctype`** &mdash; *Function*.



```
doctype(doctype::Symbol = :html) :: String
```

Outputs document's doctype.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L399-L403' class='documenter-source'>source</a><br>

<a id='Flax.doc' href='#Flax.doc'>#</a>
**`Flax.doc`** &mdash; *Function*.



```
doc(html::String) :: String
doc(doctype::Symbol, html::String) :: String
```

Outputs document's doctype.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L409-L414' class='documenter-source'>source</a><br>

<a id='Flax.register_elements' href='#Flax.register_elements'>#</a>
**`Flax.register_elements`** &mdash; *Function*.



```
register_elements() :: Void
```

Generated functions that represent Flax functions definitions corresponding to HTML elements.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L423-L427' class='documenter-source'>source</a><br>

<a id='Flax.include_helpers' href='#Flax.include_helpers'>#</a>
**`Flax.include_helpers`** &mdash; *Function*.



```
include_helpers() :: Void
```

Loads helpers and makes them available in the view layer.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L461-L465' class='documenter-source'>source</a><br>

<a id='Flax.foreachvar' href='#Flax.foreachvar'>#</a>
**`Flax.foreachvar`** &mdash; *Function*.



```
foreachvar(f::Function, key::Symbol, v::Vector) :: String
```

Utility function for looping over a `vector` `v` in the view layer.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L477-L481' class='documenter-source'>source</a><br>

<a id='Flax.var_dump' href='#Flax.var_dump'>#</a>
**`Flax.var_dump`** &mdash; *Function*.



```
var_dump(var, html = true) :: String
```

Utility function for dumping a variable.


<a target='_blank' href='https://github.com/essenciary/Flax.jl/tree/7d8cec38f3f95070838af6e4a787f2a38d0b7f32/src/Flax.jl#L504-L508' class='documenter-source'>source</a><br>

