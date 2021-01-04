perl-store
==========

.perl serialization class and module

This module will work only for only simple situations. All data that is not visible after calling [.perl](http://doc.perl6.org/routine/perl) method will be lost. This may be considered as limitation or feature. 

```raku

    my Bar $bar .= new(a=> 128); 
    my Foo $foo .= new(u=> 'Gore', bar => $bar);
    
    $foo.to_file('tt1.pl');
    my $tested = Foo.from_file('tt1.pl');
    
```
