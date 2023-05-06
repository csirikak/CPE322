## Lab 6 — Node.js and Pystache
## node hello.js
![image](https://user-images.githubusercontent.com/32028457/236644723-44a2f666-83a8-4bb3-989a-3ef6c90050d2.png)
## node http.js
![image](https://user-images.githubusercontent.com/32028457/236644760-885f7f59-3118-4ac4-937f-86f6162c7d70.png)
## pystache
```
C:\Users\n_j\Downloads\iot-master\lesson6>cat say_hello.mustache
Hello, {{to}}!

C:\Users\n_j\Downloads\iot-master\lesson6>cat say_hello.py
# https://github.com/defunkt/pystache
import pystache
print(pystache.render('Hi {{person}}!', {'person': 'Alexa'}))

# Create dedicated view classes to hold view logic
class SayHello(object):
    def to(self):
        return "World"
hello = SayHello()

# Use template in say_hello.mustache
renderer = pystache.Renderer()
print(renderer.render(hello))

# Pre-parse a template
parsed = pystache.parse('Hey {{#who}}{{.}}!{{/who}}')
print(parsed)
print(renderer.render(parsed, {'who': 'Google'}))
print(renderer.render(parsed, {'who': 'Siri'}))

C:\Users\n_j\Downloads\iot-master\lesson6>py say_hello.py
Hi Alexa!
Hello, World!

['Hey ', _SectionNode(key='who', index_begin=12, index_end=18, parsed=[_EscapeNode(key='.'), '!'])]
Hey Google!
Hey Siri!
```
