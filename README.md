### Test Cases of Programming Task 1: "Introduction to Optimization"

#### **Test Case 1**

**Optimization problem:**

```
max z = 4.00x1 + 5.00x2
```

**Subject to constraints:**

```
2.00x1 + 4.00x2 ≤ 560.00  
1.00x1 + 1.00x2 ≤ 170.00  
2.00x1 + 1.00x2 ≤ 300.00
```

| **Iteration** | **Simplex Tableau**                                                                                                                                                                                                                                                                                                                                 | **Pivot Element** | **Selected Row and Column**          |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------|--------------------------------------|
| **1**         | 2.00x₁ + 4.00x₂ + 1.00s₁ + 0.00s₂ + 0.00s₃ = 560.00 <br> 1.00x₁ + 1.00x₂ + 0.00s₁ + 1.00s₂ + 0.00s₃ = 170.00 <br> 2.00x₁ + 1.00x₂ + 0.00s₁ + 0.00s₂ + 1.00s₃ = 300.00 <br> -4.00x₁ + -5.00x₂ + 0.00s₁ + 0.00s₂ + 0.00s₃ = 0.00                                                                                                    | 4.00             | Row 1, Column 2                     |
| **2**         | 0.50x₁ + 1.00x₂ + 0.25s₁ + 0.00s₂ + 0.00s₃ = 140.00 <br> 0.50x₁ + 0.00x₂ + -0.25s₁ + 1.00s₂ + 0.00s₃ = 30.00 <br> 1.50x₁ + 0.00x₂ + -0.25s₁ + 0.00s₂ + 1.00s₃ = 160.00 <br> -1.50x₁ + 0.00x₂ + 1.25s₁ + 0.00s₂ + 0.00s₃ = 700.00                                                                                          | 1.50             | Row 2, Column 1                     |
| **3**         | 0.00x₁ + 1.00x₂ + 0.50s₁ + -1.00s₂ + 0.00s₃ = 110.00 <br> 1.00x₁ + 0.00x₂ + -0.50s₁ + 2.00s₂ + 0.00s₃ = 60.00 <br> 0.00x₁ + 0.00x₂ + 0.50s₁ + -3.00s₂ + 1.00s₃ = 70.00 <br> 0.00x₁ + 0.00x₂ + 0.50s₁ + 3.00s₂ + 0.00s₃ = 790.00                                                                                         | —                | —                                    |
| **Solution**  | **x₁ = 60.00, x₂ = 110.00**                                                                                                                                                                                                                                                                                                                         |                  | Objective function value: 790.00     |

---

#### **Test Case 2**

**Optimization problem:**

```
max z = 40.00x₁ + 30.00x₂
```

**Subject to constraints:**

```
1.00x₁ + 1.00x₂ ≤ 12.00  
2.00x₁ + 1.00x₂ ≤ 16.00  
-1.00x₁ + 0.00x₂ ≤ 0.00  
0.00x₁ + -1.00x₂ ≤ 0.00
```

| **Iteration** | **Simplex Tableau**                                                                                                                                                                                                                                                                                                                                 | **Pivot Element** | **Selected Row and Column**          |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------|--------------------------------------|
| **1**         | 1.00x₁ + 1.00x₂ + 1.00s₁ + 0.00s₂ + 0.00s₃ + 0.00s₄ = 12.00 <br> 2.00x₁ + 1.00x₂ + 0.00s₁ + 1.00s₂ + 0.00s₃ + 0.00s₄ = 16.00 <br> -1.00x₁ + 0.00x₂ + 0.00s₁ + 0.00s₂ + 1.00s₃ + 0.00s₄ = 0.00 <br> 0.00x₁ + -1.00x₂ + 0.00s₁ + 0.00s₂ + 0.00s₃ + 1.00s₄ = 0.00 <br> -40.00x₁ + -30.00x₂ + 0.00s₁ + 0.00s₂ + 0.00s₃ + 0.00s₄ = 0.00 | 2.00             | Row 2, Column 1                     |
| **2**         | 0.00x₁ + 0.50x₂ + 1.00s₁ + -0.50s₂ + 0.00s₃ + 0.00s₄ = 4.00 <br> 1.00x₁ + 0.50x₂ + 0.00s₁ + 0.50s₂ + 0.00s₃ + 0.00s₄ = 8.00 <br> 0.00x₁ + 0.50x₂ + 0.00s₁ + 0.50s₂ + 1.00s₃ + 0.00s₄ = 8.00 <br> 0.00x₁ + -1.00x₂ + 0.00s₁ + 0.00s₂ + 0.00s₃ + 1.00s₄ = 0.00 <br> 0.00x₁ + -10.00x₂ + 0.00s₁ + 20.00s₂ + 0.00s₃ + 0.00s₄ = 320.00   | 1.00             | Row 1, Column 2                     |
| **3**         | 0.00x₁ + 1.00x₂ + 2.00s₁ + -1.00s₂ + 0.00s₃ + 0.00s₄ = 8.00 <br> 1.00x₁ + 0.00x₂ + -1.00s₁ + 1.00s₂ + 0.00s₃ + 0.00s₄ = 4.00 <br> 0.00x₁ + 0.00x₂ + -1.00s₁ + 1.00s₂ + 1.00s₃ + 0.00s₄ = 4.00 <br> 0.00x₁ + 0.00x₂ + 2.00s₁ + -1.00s₂ + 0.00s₃ + 1.00s₄ = 8.00 <br> 0.00x₁ + 0.00x₂ + 20.00s₁ + 10.00s₂ + 0.00s₃ + 0.00s₄ = 400.00    | —                | —                                    |
| **Solution**  | **x₁ = 4.00, x₂ = 8.00**                                                                                                                                                                                                                                                                                                                            |                  | Objective function value: 400.00     |



#### **Test Case 3**

**Optimization problem:**

```
max z = 3.00x₁ + 5.00x₂ + 4.00x₃
```

**Subject to constraints:**

```
2.00x₁ + 3.00x₂ + 0.00x₃ ≤ 8.00  
0.00x₁ + 2.00x₂ + 5.00x₃ ≤ 10.00  
3.00x₁ + 2.00x₂ + 4.00x₃ ≤ 15.00  
-1.00x₁ + 0.00x₂ + 0.00x₃ ≤ 0.00
0.00x₁ - 1.00x₂ + 0.00x₃ ≤ 0.00
0.00x₁ + 0.00x₂ - 1.00x₃ ≤ 0.00
```

