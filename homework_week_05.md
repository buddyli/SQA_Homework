#Formal Methods and Model Checking

##Formal Methods
The basic idea of formal verification is to verify the correctness, or absence of faults,
of some given program code or design against its formal specifications. Therefore, the
existence of formal specifications is a prerequisite for formal verifications. Both formal
specification techniques and formal verification techniques are referred to as formal methods
 collectively in literature. When formal methods are used for software development, formal
specifications are used upstream for requirement analysis and product specifications, and
formal verifications or analyses are used downstream to verify the design and code before
additional verification and validation (V&V) activities are carried out. Therefore, the use
of formal methods can be summarized in the following two-step process:
######1. Constructing formal specijications.
The expected behavior and other properties of
the software artifacts are represented in formal models. These models of program
code, design, and expected behavior are typically product-dependent, which can be
specifically constructed for formal verification and analysis purposes. However, to
reduce cost as well as to benefit from formal development methods, these models
can be the same as the formal specifications or adapted by formalizing informal
specificationsfor the product.
######2. Performing formal verijications.
Formal analysis techniques are applied on the prod-
uct components, typically product code or formal designs, to verify their correctness
with respect to their formal specifications,or to check for certain properties. These
techniques are typically organized as a product-independentframework of rules that
serve as the basis of formal inferences or analyses. The most common type is a
set of axioms used in correctness verification, which we describe in Section 15.2.
Other frameworks used for formal verification and analysis are also described in this
chapter.



#Model Checking
Model checking is such an approach that automatically or algorithmically checks
certain properties for some software systems, the following briefly summarize the key ideas:

######A software system is modeled as a finite-state machine (FSM), with some property of interest expressed as a suitable formula, or a proposition, defined with respect to the FSM. Ideally, this FSM and the propositions are both developed during the software specification process, much like the use of formal specifications in various formal methods.
######The model checker is a software that runs an algorithm to check the validity of the proposition. If it is checked to be true, a proof is said to be produced. Otherwise, a counterexample is given, much like a failed test case that can be analyzed further for defect fixing.


