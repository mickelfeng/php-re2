Introduction
=========
php-re2 is a PHP extension which provides an interface to Google's [RE2 regular-expression library](http://code.google.com/p/re2/).

````
Backtracking engines are typically full of features and convenient syntactic sugar but can be forced into taking exponential amounts of time on even small inputs. RE2 uses automata theory to guarantee that regular expression searches run in time linear in the size of the input. RE2 implements memory limits, so that searches can be constrained to a fixed amount of memory. RE2 is engineered to use a small fixed C++ stack footprint no matter what inputs or regular expressions it must process; thus RE2 is useful in multithreaded environments where thread stacks cannot grow arbitrarily large.

On large inputs, RE2 is often much faster than backtracking engines; its use of automata theory lets it apply optimizations that the others cannot.

Unlike most automata-based engines, RE2 implements almost all the common Perl and PCRE features and syntactic sugars. It also finds the leftmost-first match, the same match that Perl would, and can return submatch information. The one significant exception is that RE2 drops support for backreferences¹ and generalized zero-width assertions, because they cannot be implemented efficiently. The syntax page gives full details.
````
