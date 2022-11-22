## Setup

#### Install **Golang**:

* `$ sudo yum install golang`

#### Set the environment variable:

* `$ mkdir $HOME/go`
* `$ export GOPATH=$HOME/go`
* `$ export PATH=$PATH:$GOPATH/bin`

#### Install mercurial, in order to download the bcrypt package from the Google repository:

* `$ sudo yum install mercurial`

#### If you encounter a problem installing Mercurial, you can do the following:

* `$ sudo yum install python-setuptools python-devel gcc -y`
* `$ sudo easy_install Mercurial`

#### Download the package from the Google repository to generate bcrypt:

* `$ go get code.google.com/p/go.crypto/bcrypt`

#### We compile the script: 

* `$ go build clicrypt.go`

#### Test the script, trying to hash a value, via the password parameter:

* `$ ./bcrypt_generate -password="joyitaGOD"`

#### It returns the following hash:

* `$ $2a$13$oWvgAl9CYjiQE8rjzX6h4.Lf/NS2pIAb9KnfG2s9vszFy6dXmP6Ry`
