# explorational programming

Let's use pry to explore within some ruby objects we already know.  We'll also learn a little bit about scope.

In your terminal start pry.
```bash
$ pry
```

1. Create a method called `hello_world`
Use the method.
2. Use `find-method` to show all the `to_s` methods.  Also try `find-method --help`

3. Create a hash and save it as `my_hash`
```ruby
my_hash = { name: 'tgaff', email: 'tgaff@tgaff.com' }
```

Then explore your hash using the `cd` and `ls` commands.  Try to call some of the instance methods available to you such as `#keys`.
```ruby
cd my_hash
ls
```

Question: Can you still use `hello_world` here?  Why?

5. While still inside `my_hash` add a new instance method called `crazy_hash` that `puts 'crazy'`.  Then `cd ..` out of `my_hash` and try to call `crazy_hash`.  

6. What object is `crazy_hash` bound to?  Do you think it will exist on new instances of Hash?  