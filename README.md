# fontcustom-example
This readme shows you how to create your own svg-based webfont.

# Installation
To install on OS X using Homebrew simply run:
```sh
brew install fontforge --with-python
brew install eot-utils
gem install fontcustom
```

On Linux? No Problem:
```sh
sudo apt-get install fontforge
wget http://people.mozilla.com/~jkew/woff/woff-code-latest.zip
unzip woff-code-latest.zip -d sfnt2woff && cd sfnt2woff && make && sudo mv sfnt2woff /usr/local/bin/
gem install fontcustom
```

# Usage
Compile once:
```sh
fontcustom compile vectors/
```
Or with a proper configuration in place:
```sh
fontcustom compile vectors/ -c vectors/fontcustom.yml
```
To create a configuration:
```sh
fontcustom config vectors/
```

# Example
Compile actionbar-icons:
```sh
fontcustom compile vectors/actionbar-icons/ -c vectors/actionbar-icons/fontcustom.yml
```