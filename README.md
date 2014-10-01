gochat-mqtt
===========

A simple chat program to demonstrate [MQTT](http://mqtt.org) with Go, using the [Eclipse Paho](http://eclipse.org/paho) Go client. This version requires the develop branch of the Paho Go library.

**Build**

Requires Go, obviously...

Set the `GOPATH` and `GOBIN` variables appropriately, then...

```
$ go get git.eclipse.org/gitroot/paho/org.eclipse.paho.mqtt.golang.git
$ cd $GOPATH/git.eclipse.org/gitroot/paho/org.eclipse.paho.mqtt.golang.git
$ git checkout develop
$ go get
$ cd -
$ go install mqttchat.go
```

**Run**

```
$ ./bin/mqttchat --help
Usage of ./bin/mqttchat:
  -name="user201": Username to be displayed
  -room="gochat": The chat room to enter. default 'gochat'
  -server="tcp://iot.eclipse.org:1883": The MQTT server to connect to
```
