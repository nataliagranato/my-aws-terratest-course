<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

# Test IaC on AWS

_Learn how to test **Infrastructure as Code** on AWS cloud with Terratest._

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Step 1: Check missing parts in Terraform code

_Welcome to "aws-terratest-course"! :wave:_

**What is the goal of step 1 ?**: In first step we are going to familiarize with simple architecture of the infrastructure and after that we will update 1 missing part in Terraform code.

### :keyboard: Activity: Check missing parts in Terraform code

1. Open a new browser tab, and work on the steps in your second tab while you read the instructions in this tab.
2. Review architecture for simple infrastructure defined in Terraform code in [infra](infra) folder.![](../../design/architecture_diagram.png)
3. On your local machine [configure authentication for AWS provider](https://registry.terraform.io/providers/hashicorp/aws/latest/docs#authentication-and-configuration).
4. Clone created repository
5. Get latest ``main`` branch: ``git pull``.
6. Go to ``infra`` folder using command: ``cd infra``.
7. Initialize Terraform by command: ``terraform init``.
8. Review arguments for [aws_lambda_function_url](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function_url.html) resource.
9. Define ``function_name`` for resource ``aws_lambda_function_url`` and ``aws_lambda_permission``.
10. Try to deploy infrastructure using command: ``terraform apply``.
11. If succeeded, destroy infrastructure using command: ``terraform apply -destroy``.
12. Commit changes using command: ``git commit -am "Finish step 1"``.
13. Push changes using command: ``git push``.
14. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step, if your solution is correct.
15. If next step is not automatially updated, verify results in ``Actions`` tab in GitHub, fix code and repeat steps 8-13 one more time.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Contact with author](https://github.com/sebastianczech) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2023 Sebastian Czech &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
