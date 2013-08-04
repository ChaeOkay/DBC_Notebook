-  Programmig Process
    -  Stubbing
        -  Identify a simple use case / driver test with pseudocode of the sequence of events
        -  Stub out returns of each method
        -  Benefits: Builds framework quickly
    -  Extreme Programming and SCRUM

-  SQL
    -  Primary Key - ensures no duplicates
    -  Foreign Key - checks data integrity
    -  Ruby-land to SQL-land: Structure
        -  class : table
        -  attribute : column (field)
        -  instance : row (record)
    -  Ruby-land to SQL-land: Query return
        -  array :  table
    -  SQL queries
        -  SELECT * FROM
            -  COUNT(field)
        -  WHERE
            -  LIKE
                -  % represents a wildcard
                    -  '%a' ends with a
                    -  'a%' starts with a
                    -  '%a%'  has a somewhere in the string
                -  _ represents another kind of wildcard for a single character
                    -  '500_' represents exactly 4 characters total where the last character can be anything
        -  ORDER BY
            -  ASC alphabetical order, low-to-high, default
            -  DESC high to low
        -  JOIN
            -  SELECT * FROM table1 JOIN table2 ON table2.table1_id = table1.id
        -  UPDATE
            -  UPDATE table SET field="updated" WHERE id=2
        -  COUNTING
            -  SELECT name COUNT(*) as count FROM table1 JOIN table2 ON table2.table1_id = table1.id GROUP BY name ORDER BY COUNT(*) DESC LIMIT 10;
    -  Other sqlite3 commands:
        -  .schema
        -  .tables
        -  .mode column
        -  .headers on
    -  Think about what the query results should look like first

-  ActiveRecord
    -  Example ruby method to query database

                  def where(field, target)
                    $db.execute("SELECT * FROM table WHERE #{field} = ?", "#{target}")
                  end
    -  Rake = ruby make
    -  Migrations
        -  Create a table
        -  Modify table over time
    -  Base
        -  Has common ruby methods so that they don't need to be coded everytime a new class is created
        -  Comes with enumerable like chain methods

-  Git
    -  Communicate with your teammates
    -  Branching
        -  Master branch - local
        -  Origin branch - repo
        -  Additional branching is typically for specific features - it's okay for a very small team to all work on branch master
    -  Merging Conflicts
        -  Are normal
        -  Occur when two people work on the same piece of code and try to push
            -  An error is raised
            -  You will be temporarily put in a no-branch state
            -  A message will appear in the file with the conflict, basically asking which version is correct
            -  Make the change
    -  Reverting
       -  HEAD is the state of the branch, you are always at the head. Each commit allows you the opportunity to change the state of things to that moment.
       -  git reset HEAD^, where carrots on the end say how many commits to revert back to
       -  git reset a38dsf8e, where shaw (the number) is the log identifier (git log). Only the first few numbers of the shaw are needed.
    -  It's okay to push a lot when you are building a portfolio, but professionaly, it's used when things are 100% complete
    -  Git stash saves current information without committing
    -  Git pull is a shortcut for git fetch and git merge (gets repo info and combines them into your local branch)
    -  Communicate with your teammates


-  Vocabulary
    -  Heredoc: <<-CAPS multiline code here CAPS
    -  DSL: Domain Specific Language

-  Phase 1 Assessment Feedback
    - Areas to work on:
        -  Opening
            -  Know what code to show first
            -  Show confidence and high energy from the start
        -  Select stronger work example to show when given the opportunity, a random selection may not be the best use of time
        -  Be more confident when talking about methods, state how to use them and what they return, then demonstrate
    -  Praise:
        -  Ability to learn under pressure
        -  Understanding and demonstration of Phase1 concepts in code that was reviewed

-  Advice from graduating Fence Lizzards on Phase 3
    -  Embrace disagreement
    -  Never assume a wrong way to do things
    -  Don't dismiss anyone's ideas, be fair
    -  Everyone will get annoying to you at some point
    -  Don't keep it too uptight, have fun
    -  Test your code, other people in your group will depend on it, don't be that person


