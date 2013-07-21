Sublime text
-  tab autofills
-  command + d creates multipe cursors on matching exit. All items can be modified in place

Making Code Readable
-  decompose
-  write methods that describe (try not to use data-structure names)
-  does it sing?
-  create methods with single responcibilities
-  dry it up
-  use driver code (tests)
-  constant variables are in caps, and are global scope

Regular Expressions
-  Strings
  -  =~ => position of the matche data || nil
  -  string[regex] => matched data string || nil
  -  gsub => matched data || string
  -  match => <MatData object> || nil
  -  scan => matched data in array || []

Iteration
  -  loop iterates until it finds a break point
  -  while states a condition, and breaks when theconditions is false
  -  until state a false condition, and breaks when the condition is true
Recursion
  -  base case (limit)
  -  approach (to limit)
  -  call on self
  -  think about the call stack return (what happens after base case is met?)
  -  think about edge cases!

Scope
  -  variables are not always remembered in and out of blocks / methods
      ex1:

        me = ["orange"]
        def go(me)
          me << "apple"
        end
        go(me)
        p me    => ["orange", "apple"]

      ex2:

        me = ["orange"]
        def go(me)
          me = ["apple"]
        end
        go(me)
        p me    => ["orange"]

Nested Arrays
  -  Two ways of creating 2D array:
    -  Array.new(size) { Array.new(size) }
    -  Array.new(size, Array.new(2))
  -  Passing blocks to delcare default values
    -  Array.new(5) { |item| item**2 }

Debugging
-  Don't program and debug
  -  have a plan, program, and then debug
-  Test early, test often
-  Keep methods small, provide proper naming
-  Test extremes of ranges
-  Isolate the problem, visualize the state, assume the actual value

MVP - minimum viable product


Engineering Empathy - Feedback:
-  engageing in feedback is initimate, it takes trust from both people, grows relationship
-  Giving Feedback
  -  actionable
      -  Make a request, not a demand. Give people a choice to take action, leave room for a 'no'.
  -  specific
      -  Specificity in a request can make things easier for the other person.
  -  kind
      -  Understand that theis person is in a vulnerable situation.
      -  Truthful is not the same as nice.
      -  Try and leave judgement  and opinion.
-   Receiving Feedback
  -  Have compassion for yourself
  -  It's okay to walk away with 1%
    -  filter a little, take what works, discern what is being said
  -  Feedback can potential hurt, but hurt can quickly lead to learning.
  -  Don't mistrust your feelings
  -  how you receive feedback matters also.


Engineering Empathy - Conflict:
-  be aware of non-productive tendances : withdrawl, avoidance, attack self, attack other
-  be aware of power
  -  social rank, democratic, psychological, spiritual
-  Slow down and breath
-  Honest transparency
-  Inquiry curiosity and compassion
-  Name / recognize your internal non-productive tendancies
-  Englist your counterpart as your ally
