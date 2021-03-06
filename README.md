# ![Awaitility](resources/Awaitility_logo_red_small.png) 
[![Build Status](https://travis-ci.org/jayway/awaitility.svg)](https://travis-ci.org/jayway/awaitility)

Testing asynchronous systems is hard. Not only does it require handling threads, timeouts and concurrency issues, but the intent of the test code can be obscured by all these details. Awaitility is a DSL that allows you to express expectations of an asynchronous system in a concise and easy to read manner. For example:

```java
@Test
public void updatesCustomerStatus() throws Exception {
    // Publish an asynchronous event:
    publishEvent(updateCustomerStatusEvent);
    // Awaitility lets you wait until the asynchronous operation completes:
    await().atMost(5, SECONDS).until(customerStatusIsUpdated());
    ...
}
```


## News

See <a href="https://code.google.com/p/awaitility/">homepage</a>.

## Documentation

* [Getting started](https://code.google.com/p/awaitility/wiki/Getting_started)
* [User Guide](https://code.google.com/p/awaitility/wiki/Usage)
* [Awaitility Javadoc](http://awaitility.googlecode.com/svn/tags/1.6.2/apidocs/com/jayway/awaitility/Awaitility.html)


## Founded by:

[![jayway](http://www.arctiquator.com/oppenkallkod/assets/images/jayway_logo.png)](http://www.jayway.com)

[![Analytics](https://ga-beacon.appspot.com/UA-17489061-2/jayway/awaitility)](https://github.com/jayway/awaitility)
