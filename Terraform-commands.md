# Terraform Command Guide

Terraform is an Infrastructure as Code (IaC) tool that helps you manage and provision infrastructure using a declarative configuration language. Below is a breakdown of key `terraform` commands with examples and analogies.

---

## 1. `terraform init`
**What it does:** Initializes a Terraform project by downloading provider plugins and setting up the backend.

**Analogy:** Setting up a new workspace before starting a construction project.

**Example:**
```sh
terraform init
```

---

## 2. `terraform plan`
**What it does:** Shows what Terraform *would* do before applying changes.

**Analogy:** An architect creating a blueprint before construction.

**Example:**
```sh
terraform plan
```

---

## 3. `terraform apply`
**What it does:** Executes the planned changes and provisions infrastructure.

**Analogy:** A builder following the blueprint to construct a house.

**Example:**
```sh
terraform apply
```

---

## 4. `terraform destroy`
**What it does:** Deletes all resources managed by Terraform.

**Analogy:** Demolishing a house and clearing the land.

**Example:**
```sh
terraform destroy
```

---

## 5. `terraform fmt`
**What it does:** Formats Terraform code to be clean and consistent.

**Analogy:** Auto-formatting code to maintain readability.

**Example:**
```sh
terraform fmt
```

---

## 6. `terraform validate`
**What it does:** Checks the Terraform configuration for syntax errors.

**Analogy:** Running a spell check on a document before submission.

**Example:**
```sh
terraform validate
```

---

## 7. `terraform show`
**What it does:** Displays details of the current Terraform state.

**Analogy:** Checking a house’s blueprint after it's built.

**Example:**
```sh
terraform show
```

---

## 8. `terraform state list`
**What it does:** Lists all resources Terraform is managing.

**Analogy:** Getting a checklist of all items in a warehouse.

**Example:**
```sh
terraform state list
```

---

## 9. `terraform state rm <resource>`
**What it does:** Removes a resource from Terraform’s state without deleting it.

**Analogy:** Unregistering a car from a database without actually scrapping it.

**Example:**
```sh
terraform state rm aws_instance.example
```

---

## 10. `terraform output`
**What it does:** Displays output values from your Terraform configuration.

**Analogy:** Checking the final bill after a shopping spree.

**Example:**
```sh
terraform output instance_ip
```

---

## 11. `terraform import`
**What it does:** Brings an existing resource under Terraform’s management.

**Analogy:** Adding an old car into a new vehicle tracking system.

**Example:**
```sh
terraform import aws_instance.example i-1234567890abcdef0
```

---

## 12. `terraform graph`
**What it does:** Generates a visual representation of the resource dependencies.

**Analogy:** A mind map showing how different components are connected.

**Example:**
```sh
terraform graph | dot -Tpng > graph.png
```

---

## 13. `terraform workspace`
**What it does:** Manages multiple environments (e.g., dev, staging, production).

**Analogy:** Having different workbenches for different projects.

**Example:**
```sh
terraform workspace new dev
targetworkspace select dev
```

---

## Conclusion
These commands form the foundation of Terraform usage. Understanding them will help you efficiently manage infrastructure as code. 🚀
