<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/The%20Linux%20Foundation/CGOA%3A%20Certified%20GitOps%20Associate" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Certified GitOps Associate (CGOA)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [GitOps Patterns](#gitops-patterns) (6 questions)
- [GitOps Principles](#gitops-principles) (9 questions)
- [GitOps Terminology](#gitops-terminology) (6 questions)
- [Related Practices](#related-practices) (5 questions)
- [Tooling](#tooling) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:48:15.970Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| GitOps Patterns | 6 |
| GitOps Principles | 9 |
| GitOps Terminology | 6 |
| Related Practices | 5 |
| Tooling | 4 |

---

### **GitOps Patterns**

### 1. Which engine does Helm Chart templating use to inject dynamic values into YAML manifests?

- [ ] **A)** Go-template
- [ ] **B)** Jinja2
- [ ] **C)** Jsonnet
- [ ] **D)** YAML anchors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Helm uses a Go-template engine to fill placeholders in charts with values from values.yaml files.
 
 
</details>

### 2. Select all statements that are true about Kustomize overlays.

- [ ] **A)** Overlays can patch a common base without modifying the original source
- [ ] **B)** Kustomize uses strategic merge patches or JSON patches
- [ ] **C)** Kustomize supports if/else conditional logic and loops
- [ ] **D)** A base is a common set of resources shared across environments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Kustomize defines a common base and applies patches through overlays; it does not support Helm-style conditional logic and loops.
 
 
</details>

### 3. Given the YAML values file snippet in the code block, which Helm template expression outputs the declared value?

```yaml
replicaCount: 3
```

- [ ] **A)** {{ .Values.replicaCount }}
- [ ] **B)** {{ .replicaCount }}
- [ ] **C)** {{ values.replicaCount }}
- [ ] **D)** {{ .Chart.replicaCount }}

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Helm values are accessed through .Values, so .Values.replicaCount renders the numeric value defined in values.yaml.
 
 
</details>

### 4. In the CGOA context, how does a GitOps controller make Helm deployment declarative?

- [ ] **A)** It runs 'helm install' or 'helm upgrade' based on the desired state declared in Git
- [ ] **B)** It requires Helm commands to be executed manually from a developer workstation
- [ ] **C)** It uses Helm as the only source of truth
- [ ] **D)** It converts Helm charts into Kustomize overlays

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In GitOps, the controller acts as the engine that performs helm install or upgrade according to the state declared in Git.
 
 
</details>

### 5. Which of the following correctly distinguish Helm chart templating from Kustomize overlays? Select all that apply.

- [ ] **A)** Helm uses predefined values to populate placeholders in templates
- [ ] **B)** Kustomize modifies existing YAML structures by adding, removing, or changing fields
- [ ] **C)** Both Helm and Kustomize are package managers
- [ ] **D)** Kustomize can handle complex conditional logic better than Helm

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Helm relies on value injection, while Kustomize patches YAML. Kustomize lacks conditional logic and loops found in Helm templates.
 
 
</details>

### 6. The code block contains a Kustomize configuration. What is its main purpose?

```yaml
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization
bases:
  - ../../base
patchesStrategicMerge:
  - replica_count.yaml
```

- [ ] **A)** It defines a base set of resources and applies environment-specific patches
- [ ] **B)** It stores Helm chart values for a release
- [ ] **C)** It creates a new Kubernetes API extension
- [ ] **D)** It configures a container image build pipeline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Kustomization references a base and a strategic merge patch file, which is how Kustomize overlays customize resources per environment.
 
 
</details>


---

### **GitOps Principles**

### 7. In Helm chart templating, what template engine is used to inject dynamic values into Kubernetes YAML manifests?

- [ ] **A)** Go-template
- [ ] **B)** Jinja2
- [ ] **C)** Mustache
- [ ] **D)** Handlebars

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Helm uses a Go-template engine to render dynamic values into YAML manifests while preparing Kubernetes charts.
 
 
</details>

### 8. Which two statements accurately describe how Kustomize overlays work in a base and overlay model?

- [ ] **A)** Overlays customize a common base for environments
- [ ] **B)** Overlays modify the original base source files
- [ ] **C)** Overlays can use strategic merge patches
- [ ] **D)** Overlays are exclusively a Helm feature

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Kustomize overlays customize a base without modifying the original source and can use strategic merge or JSON patches.
 
 
</details>

### 9. Looking at the code block, what GitOps customization strategy is being demonstrated by the configuration?

```yaml
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization
resources:
  - base/deployment.yaml
patches:
  - target:
      kind: Deployment
    patch: |-
      - op: replace
        path: /spec/replicas
        value: 5
```

- [ ] **A)** Kustomize overlay
- [ ] **B)** Helm values injection
- [ ] **C)** Imperative CLI command
- [ ] **D)** Cluster backup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows a Kustomization resource with a patch, indicating a Kustomize overlay approach.
 
 
</details>

### 10. In the context of the CGOA framework, how should Helm be used within a GitOps workflow?

- [ ] **A)** Declaratively through a GitOps controller
- [ ] **B)** Imperatively through the CLI
- [ ] **C)** Manually on each cluster
- [ ] **D)** As a replacement for Kubernetes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CGOA emphasizes declarative Helm usage, with the GitOps controller performing installs and upgrades from Git.
 
 
</details>

### 11. Which two changes in Git can cause a GitOps controller to synchronize a Helm chart or Kustomize overlay?

- [ ] **A)** A change in a Helm chart version in Git
- [ ] **B)** A change in a Kustomize overlay in Git
- [ ] **C)** A one-time manual change in the cluster
- [ ] **D)** A local edit that is not pushed to Git

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The controller watches Git for changes in chart versions and overlays, then synchronizes the cluster to match.
 
 
</details>

### 12. What does the command shown in the code block represent in the context of GitOps execution?

```bash
helm upgrade --install my-release ./chart
```

- [ ] **A)** Imperative Helm CLI usage
- [ ] **B)** Declarative GitOps reconciliation
- [ ] **C)** Kustomize overlay rendering
- [ ] **D)** Kubernetes API server admission

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows a direct Helm upgrade command, which is imperative rather than declarative GitOps execution.
 
 
</details>

### 13. Which GitOps tool relies on predefined chart values to populate placeholders in YAML templates during manifest rendering?

- [ ] **A)** Helm
- [ ] **B)** Kustomize
- [ ] **C)** Kubernetes
- [ ] **D)** Argo CD

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Helm uses values files and placeholders, while Kustomize patches existing YAML structures.
 
 
</details>

### 14. Which two statements about Helm, Kustomize, and GitOps controllers are true according to the playbook?

- [ ] **A)** Helm is a package manager, not a GitOps controller
- [ ] **B)** Kustomize supports full conditional if/else logic
- [ ] **C)** Kustomize lacks loops and conditionals found in Helm
- [ ] **D)** Argo CD is a CI tool

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Helm packages charts, while Kustomize overlays lack Helm's complex conditional logic.
 
 
</details>

### 15. What Helm templating capability is demonstrated by the logic shown in the provided code block?

```go-template
{{ if .Values.ingress.enabled }}
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: my-ingress
{{ end }}
```

- [ ] **A)** Helm conditional logic
- [ ] **B)** Kustomize JSON patch
- [ ] **C)** Kubernetes pruning
- [ ] **D)** Flux image automation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block uses Helm Go-template syntax with a conditional block, a feature Kustomize does not provide.
 
 
</details>


---

### **GitOps Terminology**

### 16. In Helm chart templating, which file does a GitOps controller read from Git to render the final desired state for a cluster?

- [ ] **A)** values.yaml
- [ ] **B)** Chart.yaml
- [ ] **C)** Dockerfile
- [ ] **D)** kustomization.yaml

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> values.yaml holds predefined variables used as placeholders in Helm templates. A GitOps controller reads it to render the final YAML manifests.
 
 
</details>

### 17. According to the GitOps playbook, which statements accurately describe Kustomize's base-and-overlay model? Select all that apply.

- [ ] **A)** A base is a common set of resources
- [ ] **B)** Overlays customize resources with patches
- [ ] **C)** Overlays require modifying the original base
- [ ] **D)** Overlays use Helm's Go-template syntax

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Kustomize defines a common base and overlays apply strategic merge or JSON patches. It does not use Go templates or alter the original base.
 
 
</details>

### 18. Review the placeholder syntax in the code block. Which tool uses this template mechanism to inject values into YAML?

```yaml
image: nginx:{{ .Values.image.tag }}
```

- [ ] **A)** Helm
- [ ] **B)** Kustomize
- [ ] **C)** Docker Compose
- [ ] **D)** Kubernetes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The expression shown is a Helm Go-template placeholder. Helm injects values from values.yaml into the final YAML manifests.
 
 
</details>

### 19. According to GitOps practices, what is Helm's proper role when used inside a GitOps workflow?

- [ ] **A)** Kubernetes package manager
- [ ] **B)** CI/CD pipeline system
- [ ] **C)** Container image builder
- [ ] **D)** Cluster source of truth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Helm is a Kubernetes package manager. In GitOps, a controller makes Helm usage declarative by installing or upgrading based on Git state.
 
 
</details>

### 20. Which distinctions between Helm and Kustomize are correct according to the GitOps playbook? Select all that apply.

- [ ] **A)** Helm relies on value injection
- [ ] **B)** Kustomize patches fields in YAML
- [ ] **C)** Helm uses Go-template logic
- [ ] **D)** Kustomize has loops and conditionals

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Helm populates placeholders from values and supports Go templates. Kustomize changes existing YAML fields without Helm's conditional logic.
 
 
</details>

### 21. The code block declares a set of resources and a patch overlay. Which Kustomize concept does it illustrate according to the playbook?

```yaml
resources:
  - ../../base
patchesStrategicMerge:
  - replica_count.yaml
```

- [ ] **A)** Base and overlay
- [ ] **B)** Helm chart templating
- [ ] **C)** CRD installation
- [ ] **D)** Imperative kubectl

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The resources reference a common base, and patchesStrategicMerge applies environment-specific changes. This is the Kustomize base-and-overlay model.
 
 
</details>


---

### **Related Practices**

### 22. What template engine does Helm use to inject dynamic values into YAML manifests?

- [ ] **A)** Go-template
- [ ] **B)** Jinja2
- [ ] **C)** Mustache
- [ ] **D)** Handlebars

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Helm uses Go-template to inject dynamic values into YAML manifests. Jinja2, Mustache, and Handlebars are not the template engines used by Helm.
 
 
</details>

### 23. Which statements about Kustomize overlays are correct? (Select all that apply)

- [ ] **A)** Overlays customize a common base for specific environments without modifying the original source.
- [ ] **B)** Overlays rely on strategic merge patches or JSON patches to alter resources.
- [ ] **C)** Overlays require changing the original base files to apply environment-specific values.
- [ ] **D)** Overlays include built-in if/else conditional logic like Helm templates.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Kustomize uses a base and overlay model. Overlays apply strategic merge patches or JSON patches to customize resources without modifying the original base, and Kustomize does not include conditional logic.
 
 
</details>

### 24. In the code block, what is the purpose of the values shown in a Helm chart?

```yaml
image:
  repository: nginx
  tag: 1.25.3
replicas: 3
service:
  port: 80
```

- [ ] **A)** They supply default values that populate placeholders in Go templates.
- [ ] **B)** They are directly applied as Kubernetes manifest objects.
- [ ] **C)** They configure the GitOps controller's sync interval.
- [ ] **D)** They define Kustomize strategic merge patches for the cluster.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block is a Helm values file. The keys provide values that are injected into Go-template placeholders during chart rendering.
 
 
</details>

### 25. Which usage of Helm does the Certified GitOps Associate (CGOA) focus on?

- [ ] **A)** Declarative usage within GitOps
- [ ] **B)** Imperative usage through the Helm CLI
- [ ] **C)** Standalone manual package installation
- [ ] **D)** As an image builder for CI pipelines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CGOA focuses on Helm's declarative usage within GitOps; the GitOps controller performs install or upgrade operations, not imperative CLI usage.
 
 
</details>

### 26. Which statements correctly distinguish Helm's value injection from Kustomize's patching approach? (Select all that apply)

- [ ] **A)** Helm uses predefined values to populate placeholders in templates.
- [ ] **B)** Kustomize modifies existing YAML structures by adding, removing, or changing fields through overlays.
- [ ] **C)** Helm applies JSON patches directly to raw manifest files.
- [ ] **D)** Kustomize supports the same conditional logic as Helm Go-templates.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Helm injects predefined values into placeholders, while Kustomize patches YAML structures through overlays. Kustomize does not have Helm's conditional logic.
 
 
</details>


---

### **Tooling**

### 27. Which template engine does Helm use to inject dynamic values into YAML manifests?

- [ ] **A)** Go-template
- [ ] **B)** Jinja2
- [ ] **C)** Handlebars
- [ ] **D)** Mustache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Helm uses a Go-template engine to render values into YAML manifests. The Go-template syntax is a core part of how Helm injects configuration into charts.
 
 
</details>

### 28. Which statements accurately describe Kustomize overlays in a GitOps workflow?

- [ ] **A)** Overlays patch the base without modifying it
- [ ] **B)** Has Helm-style if/else and loop support
- [ ] **C)** Base defines a common resource set
- [ ] **D)** Uses Helm charts as a prerequisite

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Kustomize overlays modify a base through strategic merge or JSON patches without changing the base. Kustomize does not support Helm-style conditional logic or loops.
 
 
</details>

### 29. Study the kustomization.yaml file in the code block. In a GitOps base and overlay workflow, what does this file define?

```yaml
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization
resources:
  - ../../base
patchesStrategicMerge:
  - replica_count.yaml
```

- [ ] **A)** Defines an overlay using a patch
- [ ] **B)** Is a Helm values file
- [ ] **C)** Deletes the base resources
- [ ] **D)** Applies changes manually

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This file is a Kustomize overlay configuration. It references the base and applies a strategic merge patch. GitOps controllers apply such overlays declaratively.
 
 
</details>

### 30. In a GitOps workflow, what is the GitOps controller's role when working with Helm?

- [ ] **A)** Runs Helm commands imperatively
- [ ] **B)** Applies Git-declared Helm releases
- [ ] **C)** Compiles charts into images
- [ ] **D)** Stores charts in registries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The GitOps controller acts as the engine that installs or upgrades Helm releases based on state declared in Git. This is declarative Helm, not manual CLI execution.
 
 
</details>
