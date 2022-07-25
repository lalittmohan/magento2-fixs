```mermaid
flowchart LR
    A[Business Problem] ---> |Analysis|B[Estimate Effort] ---> C[Business Case]
```
    
```mermaid
requirementDiagram
requirement test_req {
    id: 1
    text: the test text.
    risk: high
    verifymethod: test
    }

    element test_entity {
    type: simulation
    }

    test_entity - satisfies -> test_req
```

<!-- tabs:start -->

<!-- tab:Requirement -->
- **Current functionality**
- **Required functionality**
- **Scope of work**
- **Assumptions**

<!-- tab:Solution -->
 - solution approach
 - technical design
 - estimated effort
 - Solution 1
 - Solution 2

<!-- tab:Use Cases -->
 - use case 1
 - use case 2

<!-- tabs:end -->

