#Unit Test Notes

##how to write Unit Test

Generally, JUnit is commonly used.

###JUnit Test

Junit provides assert* to ease test

    assertNotNull(response, object)
    assertEquals(response, expected, actual);

###Hamcrest

I prefer assertThat() provideded by **Hamcrest**

    assertThat(response, object, is(notNullValue()))
    assertThat(response, x, is(3))

assertThat() is more readable.

##What to test
1. corner case, like null, 0, extreme large/small value
2. behavior test
3. normal case, add error case found latter to prevent regression

##Reference
[Writing good unit tests, Part 2:Follow your nose](http://www.javaworld.com/article/2078028/core-java/writing-good-unit-tests--part-2--follow-your-nose.html?page=2)
