# Truth-Maintanence-System
A truth maintenance system, or TMS, is a knowledge representation method for representing both beliefs and their dependencies and an algorithm called the "truth maintenance algorithm" that manipulates and maintains the dependencies. The name truth maintenance is due to the ability of these systems to restore consistency.

The input of the TMS is a text ﬁle containing a sequence of actions that will force the TMS to add and retract multiple items. The system should print out the ﬁnal status of the TMS knowledge base after executing the actions in the input ﬁle.

@Global- These are global variables that acts as buffer for the rules that are inserted, accessed and deleted on the fly.

@status-It is a buffer that keeps a check on the state of the rules that are psuhed to the buffer

@rules-Rules are inserted to it in LIFO manner: Acts as buffer to hold all the rules can be taken as a list also stack 

@TMS-The main dictionary that mapd the rules to the its precedence in tmsinput file

@Functions:-
             def add_rule(self,stack, orig_rule, patterns):
                Adds the Rule to the rule buffer after parsing through regex

             def assess_rules(self):
                Asseses the rules according to the rules given and parses according the regex whitepsaces and non whitepsaces

             def delete_literals(self,literal):
                delete literals when there is a retract or extra whitepsaces added through 

            def delete_rules(rule, literal)
                delete rules according to the retract given in the TMS_input
