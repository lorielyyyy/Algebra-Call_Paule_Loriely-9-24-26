#----- MAIN PROGRAM -----
def main():
  print("ALGEBRA % CALCULUS 1")
  print("FIND THE VALUE PF (x) = FORMULA: F(x) = (ax^2+bx=c) ")

  while True:
    print("\n1. Solve a linear equation(ax + b =c) ")
    print("2. Solve a quadratic equation (ax^2 +bx +c = 0) ")
    print ("3. Evaluation f(x) = ax^ 2+ bx + c ")
    print("4. Find the derivative f' (x) at a point")
    print("5. Estimate a limits as x approaches a value")
    print("6. Compute a definite intergral of f(x)")
    print("7. Quit")

    choice= input("Choose an option: ").strip()
    if choice =="1":
      a,b,c = get_float("a: "), get_float("b_: "), get_float("c: ")
      print(solve_linear(a,b,c))

    elif choice =="2":
      a,b,c = get_float("a: "), get_float("b: ") get_float("c: ")
      print(solve_quadratic(a,b,c))

    elif choice =="3":
      a,b,c = get_float("a: "), get_float("b: "), get_float("c: ") x = get_float("x: ")
      print(f"f({x}") = {f(a, b, c)} ")

    elif choice =="4":
      a,b,c = get_float("a: "), get_float("b: "), get_float("c ") x = get_float("x: ")
      exact = deravitive_exact(a, b, x)
      numeric = deravative_numeic(a, b, c, x)
      print(f"Exact f' ({x}) = {exact}")
      print (f" Numeric f' ({x})= {numeric:.6f} (via central difference) ")

    elif choice =="5":
      a,b,c = get_float(a: "), get_float(b: ), get_float("c: ") x0 = get_float("x0(the value of x approaches): ")
      print(estimate)limit(a,b,c,x0))

    elif choice == "6":
      a,b,c = get_float("a: "), get_float("b: "), get_float("c: ")
      x1 = get_float("Lower bound x1: ")
      x2 = get_float(" Upper bound x2: ")
      exact = integral_exact(a,b,c x1, x2)
      numeric = integral_trapeziod(a, b, c, x1, x2)
      print(f"Exact intregal= {exact: . 6f} ")
      print("fNumeric intregral = {numeric: .6f} via trapeziodal rule, n =1000")

    elif choice =="7":
      print("Goodbye!")
    elif:
      print("invalid choice: please chooose 1-7.")
    if_name=="-mian_"
       main()
