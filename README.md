# Proxy
Just a review of the proxy pattern!


Structural (changes the structure of the object composition) pattern to create a wraooer fir a renitem expensive or sensitive target, this will encapsulate the complexity/overhead
of the target in the wrapper, so the client deals with the wrapper, and the wrapper delegates to the target

This is a middleman!

For example, if we want to add aditional functionalities that are not inherit from the class, but from the proxy, for example, have logs for each method.

Imagine this case: 
We have the interface ICuenta, and two implementations (A and B). The middleware Proxy is working with 'A' account, now someone says that we are not longer working with 'A' account,
we have switched to 'B' account, the only thing you have to do is to call the proxy from outside and pass it a B implementation, if you want to add/change something, you don't have to 
go to the class, just do it on the proxy.

![image](https://github.com/user-attachments/assets/f25340b3-ea27-4a4e-95a1-37c3b2576383)
