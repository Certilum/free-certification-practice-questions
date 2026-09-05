<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/NVIDIA/NVIDIA%20Certified%20Professional%3A%20OpenUSD%20Development" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>NVIDIA Certified Professional - OpenUSD Development</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Composition](#composition) (7 questions)
- [Content Aggregation](#content-aggregation) (3 questions)
- [Customizing USD](#customizing-usd) (3 questions)
- [Data Exchange](#data-exchange) (4 questions)
- [Data Modeling](#data-modeling) (4 questions)
- [Debugging and Troubleshooting](#debugging-and-troubleshooting) (3 questions)
- [Pipeline Development](#pipeline-development) (4 questions)
- [Visualization](#visualization) (2 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:41.842Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Composition | 7 |
| Content Aggregation | 3 |
| Customizing USD | 3 |
| Data Exchange | 4 |
| Data Modeling | 4 |
| Debugging and Troubleshooting | 3 |
| Pipeline Development | 4 |
| Visualization | 2 |

---

### **Composition**

### 1. Which composition arc has the strongest opinion in the LIVRPS hierarchy?

- [ ] **A)** Local layer
- [ ] **B)** Inherits
- [ ] **C)** References
- [ ] **D)** Specializes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Local layer is the strongest opinion in the hierarchy and provides the final word on attribute values.
 
 
</details>

### 2. Which two statements accurately describe Payloads and References?

- [ ] **A)** Payloads can be loaded or unloaded dynamically.
- [ ] **B)** References are the most common method for reusing assets.
- [ ] **C)** Payloads have the same strength as References.
- [ ] **D)** Payloads are stronger than Local opinions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Payloads may be loaded/unloaded and References are common. Payloads are not identical to References in strength, and Local is stronger.
 
 
</details>

### 3. In the code block, what does the references arc do for the Chair prim?

```usda
def "Chair" (
    references = @chairBase.usd@
    specializes = </ChairBase>
)
{
}

```

- [ ] **A)** It pulls the entire structure of the referenced asset into Chair.
- [ ] **B)** It makes Chair the strongest layer in the stage.
- [ ] **C)** It unloads the referenced asset for performance.
- [ ] **D)** It prevents any attribute overrides.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A reference pulls in the entire structure of another USD file; it does not make the prim a layer or unload content.
 
 
</details>

### 4. What is the fundamental logic used by USD to navigate layers and composition arcs?

- [ ] **A)** Composition Engine Traversal
- [ ] **B)** Prim Indexing and Caching
- [ ] **C)** Stage Population Latency
- [ ] **D)** Payload Loading/Unloading

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The composition engine traverses layers and arcs, applying LIVRPS to select the active value.
 
 
</details>

### 5. Which two statements about Inherits and Specializes are correct?

- [ ] **A)** Inherits are more dynamic than references.
- [ ] **B)** Specializes is stronger than Inherits.
- [ ] **C)** Specializes is the weakest composition arc in LIVRPS.
- [ ] **D)** Inherits and Specializes have the same strength.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Inherits update dynamically if the target changes; Specializes is the weakest arc below Inherits.
 
 
</details>

### 6. In the code block, why can the Car prim override the purpose attribute from the Vehicle class?

```usda
class Vehicle
{
    string purpose = "prop"
}

def "Car" (
    specializes = </Vehicle>
)
{
    string purpose = "hero"
}

```

- [ ] **A)** The specializing prim's local opinion takes precedence over the class definition.
- [ ] **B)** The class prim is not allowed to define attributes.
- [ ] **C)** References are weaker than specializes.
- [ ] **D)** Metadata cannot be inherited by specializers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Overriding a value in a specializing prim takes precedence over the class definition per USD strength ordering.
 
 
</details>

### 7. What is a defining characteristic of Class prims in USD?

- [ ] **A)** They are templates that are not intended to be rendered.
- [ ] **B)** They are always rendered as objects.
- [ ] **C)** They cannot inherit attributes.
- [ ] **D)** They are unloaded payloads.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Class prims are blueprints/templates and are not meant to appear as renderable objects.
 
 
</details>


---

### **Content Aggregation**

### 8. In the LIVRPS strength ordering, which composition arc has the strongest opinion?

- [ ] **A)** Local
- [ ] **B)** Inherits
- [ ] **C)** References
- [ ] **D)** Specializes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Local layer is the strongest opinion in the LIVRPS hierarchy and provides the final word on all attribute values.
 
 
</details>

### 9. Which statements about Payloads in USD are correct? Select all that apply.

- [ ] **A)** Payloads can be dynamically loaded or unloaded to manage performance.
- [ ] **B)** Payloads are stronger than References in the LIVRPS hierarchy.
- [ ] **C)** Payloads are architecturally identical to References and occupy the same strength position.
- [ ] **D)** Payloads allow a lightweight structural skeleton to be built before heavy data is loaded.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Payloads are similar to References but are architecturally separated for performance optimization. They can be loaded and unloaded dynamically, and they help manage large scenes by deferring heavy data loading. Payloads are weaker than References in LIVRPS ordering.
 
 
</details>

### 10. Inspect the composition arcs shown in the USD snippet in the code block. Which arc has the weakest strength in the LIVRPS hierarchy?

```usd
#usda 1.0

def "Robot" (
    inherits = </RobotBase>
    prepend references = @robot_model.usd@</Robot>
    specializes = </RobotSchema>
)
{
}

```

- [ ] **A)** Inherits
- [ ] **B)** References
- [ ] **C)** Specializes
- [ ] **D)** Local

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The LIVRPS strength order is Local > Inherits > VariantSets > References > Payloads > Specializes. Since the snippet includes Inherits, References, and Specializes, Specializes is the weakest arc shown.
 
 
</details>


---

### **Customizing USD**

### 11. In the LIVRPS strength ordering, which composition arc has the strongest opinion in the hierarchy?

- [ ] **A)** Local Layer
- [ ] **B)** Inherits
- [ ] **C)** References
- [ ] **D)** Payloads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Local layer is first in LIVRPS and represents the active authoring layer. Its opinions override Inherits, VariantSets, References, Payloads, and Specializes.
 
 
</details>

### 12. Which statements accurately describe the relationship between references and payloads in USD composition? Select all that apply.

- [ ] **A)** Payloads can be loaded or unloaded dynamically, while references are not intended for that type of deferred loading.
- [ ] **B)** In the LIVRPS ordering, references are weaker than payloads.
- [ ] **C)** References and payloads have the same strength within the LIVRPS hierarchy.
- [ ] **D)** Payloads are architecturally separated from references to support large-scale scene management and memory efficiency.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Payloads behave similarly to references but can be dynamically loaded or unloaded. In LIVRPS, references are stronger than payloads, not identical to them, and payloads are architecturally separated to improve scene management.
 
 
</details>

### 13. In the supplied USDA snippet, which prim acts as the template that the other prim specializes on?

```usd
#usda 1.0
class MaterialBase
{
    color3f:diffuseColor = (0.5, 0.5, 0.5)
}

def "RedMaterial" (
    specializesOn = </MaterialBase>
)
{
    color3f:diffuseColor = (1.0, 0.0, 0.0)
}

```

- [ ] **A)** MaterialBase
- [ ] **B)** RedMaterial
- [ ] **C)** The prim that contains the local color override
- [ ] **D)** Both prims equally

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MaterialBase is a Class prim and serves as the template. RedMaterial specializes on MaterialBase, meaning RedMaterial inherits the base schema but can override its attribute values locally.
 
 
</details>


---

### **Data Exchange**

### 14. In the LIVRPS strength ordering, which composition arc represents the strongest opinion in the hierarchy?

- [ ] **A)** Local Layer
- [ ] **B)** Inherits
- [ ] **C)** References
- [ ] **D)** Specializes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Local Layer is the strongest opinion in the LIVRPS hierarchy; it is the active working or session layer and overrides all other composition arcs.
 
 
</details>

### 15. Which statements about Payloads are correct based on USD composition principles?

- [ ] **A)** Payloads can be loaded or unloaded dynamically.
- [ ] **B)** Payloads are architecturally separated from References to support large-scale scene management.
- [ ] **C)** Payloads have the same composition strength as References.
- [ ] **D)** Payloads help reduce memory use by deferring heavy data until needed.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Payloads behave similarly to References but are structurally separated and sit lower in the LIVRPS order; they are designed to defer loading and optimize memory.
 
 
</details>

### 16. Examine the USD code in the code block. In this definition, which prim is the child that inherits the Class template via specializesOn?

```usda
def "Robot" (
    specializesOn = </RobotBase>
)
{
}

```

- [ ] **A)** Robot
- [ ] **B)** RobotBase
- [ ] **C)** Both Robot and RobotBase
- [ ] **D)** Neither; specializesOn does not create inheritance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The prim containing the specializesOn relationship is the child or specializing prim. Here, Robot specializes on RobotBase, so Robot is the inheriting child.
 
 
</details>

### 17. What is the architectural role of a Class prim in a USD scene?

- [ ] **A)** Class prims are templates and are not intended to be rendered.
- [ ] **B)** Class prims are always rendered as invisible placeholder objects.
- [ ] **C)** Class prims are unique objects that appear once per scene.
- [ ] **D)** Class prims are unloaded unless explicitly referenced.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Class prims are blueprints for composing prims via specializesOn; they are not meant to be instanced or rendered in the final scene.
 
 
</details>


---

### **Data Modeling**

### 18. Which of the following correctly represents the LIVRPS strength ordering used by the USD composition engine?

- [ ] **A)** Local > Inherits > VariantSets > References > Payloads > Specializes
- [ ] **B)** Local > VariantSets > Inherits > References > Payloads > Specializes
- [ ] **C)** Specializes > Payloads > References > VariantSets > Inherits > Local
- [ ] **D)** Local > Inherits > References > VariantSets > Payloads > Specializes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The LIVRPS order is deterministic: Local is strongest, followed by Inherits, VariantSets, References, Payloads, and Specializes. This ensures local opinions override weaker arcs.
 
 
</details>

### 19. Which statements accurately describe the behavior and purpose of Class prims and the specializesOn relationship?

- [ ] **A)** Class prims serve as templates or blueprints for other prims rather than renderable objects.
- [ ] **B)** The specializing prim inherits the Class attributes and can override specific values using standard USD strength ordering.
- [ ] **C)** Class prims are intended to be rendered and must be treated like any other asset in the final scene.
- [ ] **D)** specializesOn is identical to references because both use object instantiation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Class prims are templates, not renderable objects. A specializing prim inherits the Class schema and can override attribute values according to standard USD strength ordering.
 
 
</details>

### 20. Inspect the USDA snippet. Which composition arc is being used to make RedPaint inherit from _BaseMaterial?

```usda
class "_BaseMaterial"
{
    color3f baseColor = (1, 0, 0)
}

def Material "RedPaint" (
    specializes = </_BaseMaterial>
)
{
    color3f baseColor = (0.8, 0.1, 0.1)
}
```

- [ ] **A)** Specializes
- [ ] **B)** References
- [ ] **C)** Inherits
- [ ] **D)** Payload

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The specializes metadata on RedPaint creates a specializesOn arc to _BaseMaterial. This is template inheritance, not referencing or instancing.
 
 
</details>

### 21. In the LIVRPS hierarchy, which composition arc has the weakest opinion strength?

- [ ] **A)** Specializes
- [ ] **B)** Payloads
- [ ] **C)** References
- [ ] **D)** VariantSets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Specializes is the weakest composition arc in the LIVRPS hierarchy, providing base attributes that can be overridden by Local, Inherits, VariantSets, References, or Payloads.
 
 
</details>


---

### **Debugging and Troubleshooting**

### 22. According to the LIVRPS strength ordering, which composition arc has the highest opinion strength?

- [ ] **A)** Local Layer
- [ ] **B)** Inherits
- [ ] **C)** VariantSets
- [ ] **D)** Specializes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The LIVRPS strength order is Local > Inherits > VariantSets > References > Payloads > Specializes. The Local Layer contains the strongest opinions because it represents the current working layer where direct edits are made.
 
 
</details>

### 23. Which two statements correctly describe the relationship between References and Payloads in USD composition?

- [ ] **A)** References pull in the entire structure of another USD file.
- [ ] **B)** Payloads may be loaded or unloaded dynamically for performance optimization.
- [ ] **C)** Payloads are stronger than References in the LIVRPS order.
- [ ] **D)** References and Payloads have identical strength in the hierarchy.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> References are the most common method for reusing assets and pull in the entire structure of another USD file. Payloads are similar but designed for performance, allowing dynamic loading and unloading. In LIVRPS, References are stronger than Payloads, so they are not identical in strength.
 
 
</details>

### 24. In the provided USD snippet, both a reference and a payload are authored on the same prim. If the referenced and payload assets define the same attribute with different values, which composition arc wins during traversal?

```usda
#usda 1.0
def "Robot" (
    references = @robot_base.usda@</Robot>
    payload = @robot_heavy.usda@</Robot>
)
{
}

```

- [ ] **A)** Reference
- [ ] **B)** Payload
- [ ] **C)** Inherits
- [ ] **D)** Specializes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In the LIVRPS order, References are stronger than Payloads: Local > Inherits > VariantSets > References > Payloads > Specializes. Therefore, when both arcs define conflicting opinions, the reference arc wins.
 
 
</details>


---

### **Pipeline Development**

### 25. Which composition arc holds the strongest opinion in the LIVRPS hierarchy?

- [ ] **A)** Local Layer
- [ ] **B)** Inherits
- [ ] **C)** VariantSets
- [ ] **D)** References

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Local Layer is the current working or session layer where direct edits are made, giving it the final word on attribute values.
 
 
</details>

### 26. Which two statements correctly describe Payloads compared to References?

- [ ] **A)** Payloads are designed for performance optimization.
- [ ] **B)** Payloads can be loaded or unloaded dynamically.
- [ ] **C)** References and Payloads have exactly the same strength.
- [ ] **D)** Payloads are stronger than References in LIVRPS.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Payloads are similar to references but are optimized for dynamic loading and unloading, and they sit below References in the LIVRPS order.
 
 
</details>

### 27. The code block defines a prim relationship. Which composition arc is being used?

```usda
#usda 1.0
class "BaseAsset"
{
}

def "Child" (
    specializesOn = </BaseAsset>
)
{
}

```

- [ ] **A)** Specializes
- [ ] **B)** References
- [ ] **C)** Inherits
- [ ] **D)** Payloads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The specializesOn relationship links a prim to a Class for schema inheritance and is the weakest arc in the LIVRPS order.
 
 
</details>

### 28. Which composition arc is the weakest in the LIVRPS strength ordering?

- [ ] **A)** Specializes
- [ ] **B)** Payloads
- [ ] **C)** References
- [ ] **D)** VariantSets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Specializes is the weakest form of composition, providing a base set of attributes easily overridden by any higher-strength arc.
 
 
</details>


---

### **Visualization**

### 29. In the LIVRPS hierarchy, which composition arc carries the strongest opinion and overrides all others?

- [ ] **A)** Local Layer
- [ ] **B)** References
- [ ] **C)** Inherits
- [ ] **D)** Specializes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Local Layer is the strongest opinion in USD's LIVRPS hierarchy, so it overrides all other arcs.
 
 
</details>

### 30. Which of the following statements about the USD LIVRPS strength ordering are correct? Select all that apply.

- [ ] **A)** Local Layer is strongest.
- [ ] **B)** Specializes beats Payloads.
- [ ] **C)** VariantSets beat Inherits.
- [ ] **D)** Payloads beat Specializes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> LIVRPS means Local > Inherits > VariantSets > References > Payloads > Specializes. Thus Local Layer is strongest, and Payloads are stronger than Specializes.
 
 
</details>
