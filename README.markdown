# Setup

1. Install pip, virtualenv & virtualenvwrapper:

        sudo easy_install pip
        sudo easy_install virtualenv
        pip install virtualenvwrapper

    Note where pip installs virtualenvwrapper.

2. Add the following two lines to your shell startup file(`~/.bash_profile` for example).

        export WORKON_HOME=~/.virtualenv
        source /usr/local/bin/virtualenvwrapper.sh

    Ensure that the `virtualenvwrapper.sh` file is prefixed with the path noted in step 1.

3. Clone this repository:

        git clone git@github.com:jquerytools/www.git

4. Setup your [virtual environment](http://www.doughellmann.com/docs/virtualenvwrapper/)

        mkvirtualenv jqt

    You can use `workon jqt` to switch to the environment after the first time.

5. Install the requirements:

        cd ~/path/to/this/repo
        pip install --upgrade -r requirements.tx

You are all set.


# Running

Ensure that you are in the correct virtual environment(`workon jqt`).

1. `hyde gen` - generates the website.
2. `hyde serve` - starts the built-in web server.

