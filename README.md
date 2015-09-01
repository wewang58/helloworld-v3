# helloworld-v3

Usage
---
~~~
oc new-app https://github.com/nak3/helloworld-v3.git -l app=hello
curl `oc get svc |grep helloworld-v3 |awk '{print $2":"$4}' | sed -e 's/\/.*//'`
Hello world
~~~
