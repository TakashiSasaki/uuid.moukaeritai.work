このリポジトリには UUID をブランチ名とする複数のブランチ（これから作るのでまだないかもしれない）と uuid.moukaeritai.work というブランチがあります。
uuid.moukaeritai.work ブランチの全体が https://uuid.moukaeritai.work/ として公開されます。
UUID をブランチ名とする複数のブランチは、それぞれ祖先を共有しない、つまり unrelated なブランチです。
uuid.moukaeritai.work ブランチには、UUID をブランチ名とするブランチがそのUUIDをサブディレクトリ名としてそのままサブツリーとして含められます。
つまり uuid.moukaeritai.work ブランチのディレクトリ構造は /aaaaaaaa-bbbb-cccc-dddd-eeeeeeeeeeee/index.html のようなアイテムがたくさんあるということです。

## Documentation & Deployment Rules

- **Knowledge Base Structure**: 
  - All documentation must follow the hierarchical structure in `knowledge/`. 
  - Use `index.md` as the central hub for any new sub-sections.
  - Furthermore, this repository adheres to Google's Open Knowledge Format (OKF) specification for progressive disclosure. All `index.md` files (in the root and subdirectories) must contain appropriate YAML frontmatter (with at least `type: Index`) and a list of the directory's contents to allow agents to discover resources.
  - The `knowledge-index-generator` skill should be used to update indices after structural changes.

- **GitHub Pages Deployment**:
  - The site is deployed automatically via GitHub Actions from the `uuid.moukaeritai.work` branch.
  - Do not manually deploy files to the `gh-pages` branch.
  - Any changes to deployment logic must be made in `.github/workflows/deploy.yml`.

- **Branching Policy**:
  - `uuid.moukaeritai.work` is the default branch and the source of truth for the live site.
  - Ensure all features/docs are merged into this branch before expecting deployment.
