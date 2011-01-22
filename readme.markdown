# Literally

Render and parse literals from other languages with JavaScript.

# Example

    (**Not** actual console output)

    > var ruby = new Literally("ruby18", "qw");
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
