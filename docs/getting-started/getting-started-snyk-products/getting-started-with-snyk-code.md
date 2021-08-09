# Getting started with Snyk Code

Get started with [Snyk Code](https://snyk.io/product/snyk-code/) to find, prioritize and fix potential vulnerabilities in your proprietary code.

This documentation describes using Snyk Code with the Web UI. You can also use Snyk Code as a plugin to your JetBrains IDE; see [JetBrains IDE Plugins](https://support.snyk.io/hc/en-us/articles/360004032317-JetBrains-IDE-Plugins) for more details.

* A Snyk account.
* [Snyk Open Source](https://support.snyk.io/hc/en-us/categories/360003049458-Snyk-Open-Source) or [Snyk Container](https://support.snyk.io/hc/en-us/categories/360000583498-Snyk-Container) installed \(as currently Snyk Code is distributed as an add-on\).
* Projects that include code in [a supported language](https://support.snyk.io/hc/en-us/articles/360016973477-Snyk-Code-language-and-framework-support) \(currently Java, JavaScript, and Python\).
* One of the following supported source code management systems \(SCMs\): GitHub cloud, BitBucket cloud, Gitlab cloud.

#### Stage 1: Enable Snyk Code

Snyk Code is disabled by default, so you must enable it for each organization:

1. Log in to [Snyk.io](http://snyk.io/).
2. Click on settings ![cog\_icon.png](https://support.snyk.io/hc/article_attachments/4402908592145/cog_icon.png)  &gt; **Snyk Code**.
3. Under **Enable Snyk Code**, change **Disabled** to **Enabled:** ![enable-snyk-code.png](https://support.snyk.io/hc/article_attachments/360019769157/enable-snyk-code.png)
4. Click **Save changes**.

#### Stage 2: Add source control integration

if you already have an integration set up, you can skip this step.

Choose a source code integration, to allow Snyk to work on a project.

1. Log in to [Snyk.io](http://snyk.io/).
2. Select **Integrations &gt; Source control**.
3. Click the source control system \(for example, GitHub\) to integrate with Snyk:

   ![Screenshot\_2021-06-22\_at\_10.58.18.png](https://support.snyk.io/hc/article_attachments/4402938011409/Screenshot_2021-06-22_at_10.58.18.png)

4. Fill in the account credentials as prompted \(or authenticate with your account in GitHub\), to grant Snyk access permissions for integration.

See [DevOps integrations & languages](https://support.snyk.io/hc/en-us/articles/360011733538-DevOps-integrations-languages) for more details

if you already have projects added, you can skip this step.

Add projects to test with Snyk, by choosing repositories for Snyk to test and monitor.

1. Select **Projects** from [snyk.io](http://snyk.io/).
2. Select the tool to add the project from \(for example GitHub\): ![https://support.snyk.io/hc/article\_attachments/360012555458/Open-Source-Add-Projects.png](https://support.snyk.io/hc/article_attachments/360012555458/Open-Source-Add-Projects.png)
3. In **Personal and Organization repositories**, select the repositories to use: ![https://support.snyk.io/hc/article\_attachments/360012555518/IaC\_-\_select\_repo.png](https://support.snyk.io/hc/article_attachments/360012555518/IaC_-_select_repo.png)
4. Click **Add selected repositories** to import the selected repositories into your projects. This sets Snyk to run a regular check \(daily by default\) for your proprietary code vulnerabilities.
5. A progress bar appears: click **View log** to see log results.
6. Project import completes.

Currently Snyk Code does not support the **Exclude folders** option during import. Please contact us if you need more information.

See [Snyk projects](https://support.snyk.io/hc/en-us/sections/360004724958-Snyk-projects) for more details.

#### Stage 4: View vulnerabilities

You can now view vulnerability results for imported projects. The **Projects** tab appears by default after import, showing vulnerability information for projects you've imported.

1. Click on an imported project to see vulnerability information for that project, including the number of issues found, grouped by severity :

   ![View-Vulns1.png](https://support.snyk.io/hc/article_attachments/360015653898/View-Vulns1.png)

2. Click on an entry to open the issues view for that entry. For each issue, this shows the exploitable code snippet and a description of the code flaw that may lead to this vulnerability if not fixed: ![View-Vulns2.png](https://support.snyk.io/hc/article_attachments/360015653998/View-Vulns2.png)

See [View project information](https://support.snyk.io/hc/en-us/articles/360011450838-View-project-information) for more details.

#### Stage 5: View issue details

Click **Full Details** on an issue to view more details about it, such as:

* **Data Flow**: The issue's taint flow from the source \(the user input\) to the sink \(the operation that needs to receive clean input and can be exploited otherwise\).
* **Remediation Strategy**: An area that focuses on how to fix the problem with more details, references and code samples related to it.

### For more information

* [Snyk Code](https://support.snyk.io/hc/en-us/categories/360003257537-Snyk-Code)
* [Developer-first SAST with Snyk Code](https://snyk.io/blog/developer-first-sast-with-snyk-code/)
* [SAST vs DAST](https://snyk.io/learn/sast-vs-dast/)
