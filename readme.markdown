# Literally

Render and parse literals from ruby with JavaScript.

Aims to support BSON data types. As such, it goes beyond what literals
can do, since there is no date literal in Ruby.

# Example

    (**Not** actual console output)

    > var ruby = new Literally("ruby", "qw");
    > var str = ruby.stringify({words: ["this", "is", "a", "test"]};
    > console.log(str);
    {:words => %w(this is a test)}
    > console.log(JSON.stringify(ruby.parse(str), null, 2));
    {
      "words": [
        "this",
        "is",
        "a",
        "test"
      ]
    }

# TODO

* Identify rubinius code for inspecting & parsing
* Implement serializing a JavaScript object with JSON types to ruby
* Implement serializing a JavaScript object with a date to a ruby
  hash "literal" with a date
* Build github page for pasting JSON and showing it in ruby
* Set up jison
* Implement deserializing a Ruby hash literal with JSON types to a 
  JavaScript object
* Implement deserializing a Ruby hash literal with a date to a 
  JavaScript object
* Implement serializing multiline strings to heredocs
* Implement deserializing multiline strings to heredocs
