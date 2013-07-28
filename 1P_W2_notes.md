
Object Oriented Design
-  Treat everything as a model
-  The map is no the territory
-  Objects - state and behavior
    -  Data as attributes
    -  Logic as methods
-  Understand your assumptions before creating a class
    -  What things are appropriate to include in the map
    -  What doesn't belong in the object?

Object Modeling
-  Describe the program in a story
-  Nouns in the story are usually variables
-  Verbs in the story are usually methods

Modules
-  Hold/encapsulates shared behavior

Decoupling
-  Let objects send a message, don't reach in to find it
-  Objects should not be rude to each other
-  If an object is a person, don't reach inside their stomach to find the last eaten meal
-  Let the object decide what and how to show/share information with other objects

Design Pattern (MVC on a very small scale)
-  Models = data
-  View = display
-  Controller = message sender (bridging communication between models and views)

Law of Demeter
-  Don't use more than 2 dots
-  Only talk to your neighbor

Process
-  Write a narrative of the approach for the simplest possibility
-  Name nouns and verbs
-  Start with driver code
-  Let pattern emerge

Vocabulary
-  Abstraction - something a container holds

Symbols vs Strings
-  Symbols consume fewer resources than strings because Symbols only have 1 object ID assignment

Methods
-  Single responcibilities doesn't always mean less code

Hashes
-  Accessing a non-existant item within a hash will return nil

Constants
-  use for lookup tables

Gems and Libraries used
-  Nokogiri
-  uri
-  csv

Sublime text
-  shift + cntrl + P  brings up the search bar for package control

Pry
- !!! to exit

Class Variables
-  Shared between separate instances of  the same class

            class Tally
            @@count = 0

              def count
                @@count += 1
              end
            end

            a = Tally.new
            a.count        => 1
            a.count        => 2
            a.count        => 3

            b = Tally.new
            b.count        => 4
            b.count        => 5

Scope
-  Object - me
-  Object scope - my perspective (how I see things)

Code Tidbits
-  [Passing blocks](http://www.potstuck.com/2011/08/06/ruby-symbols-instead-of-blocks/)

             def wash
               @dishes.map(&:clean)
             end

             def clean
               @state = "clean"
             end
-  Creating subarrays

            array = %w(1cat 2dog 3fish 4apple 5banana 6orange 7big 8medium 9small)
            subarray = Array.new(3) { array.shift(3) }
-  Undefined variables

            undefined_local_variable.nil?
              => NameError: undefined local variable or method

            @undefined_instance_variable.nil?
              => true
-  Inheritance

            class Fruit
              def juicy?(options)
                options.sample
              end
            end

            def Orange < Fruit
              def juicy?
                options = [true, true, true, true, false]
                super(options)
              end
            end

            def Apple < Fruit
              def juicy?
                options = [true, true, false]
                super(options)
              end
            end

Other Tidbits
-  If you have a hammer, make sure you're using it to hit a nail
-  When you have a tool (or new ability), be mindful of appropriate useage



Engineer Empathy
Inner Critic / Superego

-  "I'm going to criticize you (good or bad) before someone else does it first."
-  Important defense mechanism for socializing, and knowing how to act
-  Is constantly running
-  Without it, will I turn into an awful person?  As an adult, no
-  Does not value "self" by continuously searching for the ideal average, it is not concerned with your truth
-  It is one of the biggest boundaries in learning
-  Ways it can be negative
     -  Direct attack to yourself
     -  Comparisson to other people, telling you that your internal barometer is not okay
     -  Comparisson to standards, real or self imposed
-  Ways it can be positive
    -  Can bring praise (but only in terms of superego standards)

-  Things to be mindful of
    -  Self reflection vs self deprecation
    -  Superego is a really good lawyer

-  Action for self
    -  Notice how you respond to the attack
    -  Name it in the 2nd person
    -  Talk to someone
    -  If it works, tell it to fuck off

-  Action with others
    -  Compassion
    -  Humanize (exaggerate)
