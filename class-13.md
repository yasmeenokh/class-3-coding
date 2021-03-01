# **LOCAL STORAGE FOR WEB APPLICATIONS**
For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.

* Cookies are used to create a persistent local storage of small amounts of data. However they have some disadvaneges:
1. they slow down the web application. 
2. they send unencrypted data over the internet.
3. they are limited to about 4 KB of data. 

## **History**
before HTML5; UserData was use to to store up to 64 KB of data per domain, in a hierarchical XML-based structure.

At the begening  all options avaliable either specific to a single browser, or reliant on a third-party plugin. then HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

# **HTML5 STORAGE**
Web storage or Local storage or DOM storage;it’s a way for web pages to store named key/value pairs locally, within the client web browser. this data is never transmitted to the remote web server. 
![storageData](https://lh3.googleusercontent.com/proxy/e9PbrTXkmKTcDkhZcA5ffd5LN5Gkr_o3JSv40plJflxBx1bbZV907QWxXiLvrDF1n2smq7RqJCU3F0Z6VuPd8GykYbjR6zHqZVWEfVd84c2A29xowR2B3g)

HTML web storage provides two objects for storing data on the client:

1. window.localStorage - stores data with no expiration date:

localStorage.setItem("lastname", "Smith");
document.getElementById("result").innerHTML = localStorage.getItem("lastname");

2. window.sessionStorage - stores data for one session (data is lost when the browser tab is closed)

**HTML5 supports the lastest versions of:**
1. Apple Safari
2. Google chrome
3. Mozilla firfox
4. opera 
5. some function in Internet explorer

### **USING HTML5 STORAGE**
1. method for removing the value for a given named key, and clearing the entire storage area : interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};

2. to get the total number of values in the storage area, and to iterate through all of the keys by index: interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};

### **Tracking changes**
to hook the storage event, you’ll need to check which event mechanism the browser supports.
![property](https://image.slidesharecdn.com/html5localstorage-140511235722-phpapp01/95/html5-local-storage-12-1024.jpg?cb=1399852926)


