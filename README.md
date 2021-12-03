# logic
from logic import *

one = Symbol("Number Format Exception")
two = Symbol("Random r = new Random(Double.parseDouble(x))")
three = Symbol("Divided by zero")
four = Symbol("double y = a / b;")
five = Symbol("Segmentation Fault")
six = Symbol("Low Memory")
seven = Symbol("Object o = new Object()")

knowledge = And(
    Biconditional(one, two),
    Biconditional(three, four),
    Biconditional(Not(two), five),
    And(six, one),
    Or(five,seven)
)
