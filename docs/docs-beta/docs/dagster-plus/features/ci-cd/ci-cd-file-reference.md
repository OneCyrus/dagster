---
title: CI/CD file reference
---

:::note
This reference is applicable to Dagster+.
:::

When you import a project into Dagster+ from GitHub or Gitlab, a few `.yml` files will be added to the repository. These files are essential as they manage the deployments in Dagster+.

## branch_deployments.yml

<table
  className="table"
  style={{
    width: "100%",
  }}
>
  <tbody>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Name</strong>
      </td>
      <td>branch_deployments.yml</td>
    </tr>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Status</strong>
      </td>
      <td>Active</td>
    </tr>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Required</strong>
      </td>
      <td>
        Required to use{" "}
        <a href="/dagster-plus/managing-deployments/branch-deployments">
          Branch Deployments
        </a>
      </td>
    </tr>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Description</strong>
      </td>
      <td>
        Defines the steps required to use Branch Deployments. <br />
        <br />
        <strong>Note</strong>: This file must be manually added to the
        repository if using a{" "}
        <a href="/dagster-plus/deployment/hybrid">Hybrid deployment</a>.
      </td>
    </tr>
  </tbody>
</table>

## deploy.yml

<table
  className="table"
  style={{
    width: "100%",
  }}
>
  <tbody>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Name</strong>
      </td>
      <td>deploy.yml</td>
    </tr>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Status</strong>
      </td>
      <td>Active</td>
    </tr>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Required</strong>
      </td>
      <td>Required for Dagster+</td>
    </tr>
    <tr>
      <td
        style={{
          width: "15%",
        }}
      >
        <strong>Description</strong>
      </td>
      <td>
        Defines the steps required to deploy a project in Dagster+, including
        running checks, checking out the project directory, and deploying the
        project. Additionally, note the following:
        <ul>
          <li>
            <strong>
              If using a{" "}
              <a href="/dagster-plus/deployment/hybrid">Hybrid deployment</a>
            </strong>
            , this file must be manually added to the repository.
          </li>
          <li>
            <strong>If using dbt</strong>, some steps may need to be added to
            successfully deploy your project. Refer to the{" "}
            <a href="/integrations/dbt/using-dbt-with-dagster-plus#step-3-update-the-cicd-files">
              Using dbt with Dagster+ guide
            </a>{" "}
            for more information.
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Related

{/*
<ArticleList>
  <ArticleListItem
    title="dbt & Dagster"
    href="/integrations/dbt"
  ></ArticleListItem>
  <ArticleListItem
    title="Using dbt with Dagster+"
    href="/integrations/dbt/using-dbt-with-dagster-plus"
  ></ArticleListItem>
  <ArticleListItem
    title="dagster-dbt reference"
    href="/integrations/dbt/reference"
  ></ArticleListItem>
  <ArticleListItem
    title="Getting started with Dagster+"
    href="/dagster-plus"
  ></ArticleListItem>
  <ArticleListItem
    title="dagster_cloud.yaml reference"
    href="/dagster-plus/managing-deployments/dagster-cloud-yaml"
  ></ArticleListItem>
  <ArticleListItem
    title="Dagster project files"
    href="/guides/understanding-dagster-project-files"
  ></ArticleListItem>
</ArticleList>
*/}
