# Solving-CNF-SAT-using-DPLL

Algorithm Description :

  Find unit clause and assign them value so that it becomes true.
  
  Check for Contradictions for unit clause. If contradiction is found, thhen CNF is unsatisfiable.
  
  Simplify CNF from unit clause by removing clauses containing unit clause and removing literals which are NOT(unit clause) from any clause.
  
  Choose some literal : choose the literal with the highest frequency from CNF.
  
  Check for Contradictions for chosen literal : If contradiction is found, thhen CNF is unsatisfiable.
  
  Simplify CNF from chosen literal by removing clauses containing chosen literal and removing literals which are NOT(chosen literal) from any clause.
  
  Pass CNF from step-6 to DPLL.
  
  If step-7 returns 'unsatisfiable' : repeat step-6 with NOT(chosen literal from step-4)
  
  If step-8 also return 'unsatisfiable' : CNF is unsatisfiable.
  
  Base-Case : If CNF becomes empty at any point, then CNF is satisfiable.
