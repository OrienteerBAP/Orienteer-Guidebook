# Calculable Properties

When configuring a property, you can set it to take a calculable value. For this, [on the **edit property** page](https://orienteer.gitbooks.io/orienteer/content/managing_classes.html) check **Calculable** and put a script to the field **Script**. Use a script in OrientDB format. 

Examples:
>select sum(a, b) as value from MyClass where @rid = ?
>select sum(e.salary) as value from Employee e where e.department = ? 

  In case of calculation just for a current row you can use short notation:

  > sum(a, b)

  instead of

  > select sum(a, b) as value from MyClass where @rid = ?


