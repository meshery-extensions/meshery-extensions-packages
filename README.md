<div>
    <!-- Top section -->
    <div>
        <img src="https://raw.githubusercontent.com/meshery-extensions/.github/master/profile/assets/img/meshery-extensions-github.png" usemap="#workmap"  />
    </div>
    <!-- Overview section -->
    <div align="center">
        <h3>Meshery is an extensible, self-service engineering plaform for the collaborative management of cloud and cloud native infrastructure.</h3>
        <h3 align="center"><a href="https://meshery.io/extensions">Browse all extensions</a></h3>
        <h5 align="center">
            <a href="https://meshery.io#getting-started">Installation</a> |
            <a href="https://docs.meshery.io">Documentation</a> |
            <a href="https://discuss.meshery.io">Forum</a> |
            <a href="https://play.meshery.io">Playground</a> |
            <a href="https://meshery.io/catalog">Catalog</a>
        </h5>
        <br />
    </div>
    
[Meshery Extensions](https://meshery.io/extension) are plugins or add-ons that enhance the functionality of the Meshery platform beyond its core capabilities. Meshery supports different types of extensions ([docs](https://docs.meshery.io/extensions/)):

- [Adapters](https://docs.meshery.io/concepts/architecture/adapters): Adapters allow Meshery to interface with the different cloud native infrastructure.
- [Load Generators](https://docs.meshery.io/extensibility/load-generators): for performance characterization and benchmarking
- [Integrations](https://docs.meshery.io/extensibility/integrations): model-based support for a broad variety of design and orchestration of cloud and cloud native platforms, tools, and technologies.
- [Providers](https://docs.meshery.io/extensibility/providers): for connecting to different cloud providers and infrastructure platforms
- [UI Plugins](https://docs.meshery.io/extensibility/ui): Meshery UI has a number of extension points that allow users to customize their experience with third-party plugins.
- [CLI Plugins](https://docs.meshery.io/extensibility/cli-plugins): Helm and kubectl plugins that let you create Kanvas snapshots from Helm charts, Kubernetes manifests, and the current state of your Kubernetes cluster, then upload them to Meshery.
<!-- Blog Post and Explanation section -->
<!-- Video Section -->
<h3 align="center">See Meshery and it's plugins in-action</h3>
    <img src="https://raw.githubusercontent.com/meshery/.github/master/profile/assets/img/meshery-dashboard-hero-image.png"  />
<!--     <div align="center"><i>Example extension. See other <a href="https://meshery.io/extensions">Meshery Extensions</a>.<i></div>
    <br /> -->
    <!-- Repositories section -->
    <div>
        <h2>Repo Overview</h2>
<br />

>  ⚠️ WARNING: LARGE REPO
>  Before cloning this repo to your local machine, ensure that you do so sparsely or your clone will take a long time to download / sync.
>
> Example of a sparse checkout:
> 
> ```shell
> git clone --filter=blob:none --sparse https://github.com/meshery-extensions/meshery-extensions-packages
> git sparse-checkout add assets
> ```
>
> ```shell
> git sparse-checkout init --no-cone
> vi .git/info/sparse-checkout
> /*
> !/*/
> /.github/
> git sparse-checkout reapply
> ```

ℹ️ This repository has multiple functions.

### Function 1: Cloud and Kanvas assets

**Relevant Directories**

- `/assets`: Contains 3 directories
    1. `/assets/badges`: Stores the SVG and PNG representation of badges to be used in emails.
    1. `/assets/meshmap`: Stores the animated gifs, svgs, quicktips etc,
    1. `/assets/organizations`: Stores the custom icons in PNG format namespaced under orgid.
    ```
    /assets/organizations/<org-uuid>/mobile.png
    /assets/organizations/<org-uuid>/desktop.png
    ```
    4. `/assets/kanvas`: Stores images used in Kanvas, such as in designs, roadmaps, flow-charts etc.
    5. `/assets/kanvas/getting-started/`: Stores images used in the Kanvas Getting Started section in webp format.
    

### Function 2: Meshery Cloud Remote Provider Packages
Access Meshery Cloud at https://cloud.meshery.io 

**Relevant Directories**
- `/email`: Contains html emails templates, svgs/png to be used for emails sent for `meshery-cloud` and other newsletter html templates.
- See the artifacts under each [Release](https://github.com/meshery-extensions/meshery-extensions-packages/releases).

### Function 3: Images taken by Kanvas Snapshots
Find out more at https://meshery.io/extensions/github-action-meshery-snapshot

**Relevant Directories**
- `/action-assets`: 
    - Stores the snapshots taken as part of pull requests. Each snapshot have 2 versions and are namespaced based on the year and month they were taken, for eg: snapshot against a particular PR created on 10th July 2024 will be stored at
    - Light: `/action-assets/2024@7/<design-id>-light.png` 
    - Dark version: `/action-assets/2024@7/<design-id>-dark.png`

- `/design-assets`: Stores the snapshots taken for catalog items. Every time a catalog item is updated, the corresponding snapshot for that catalog item is also updated. Catalog snapshots are referenced rom different systems, which need unauthenticated, public access to static resources, and therefore, require a permanent link. Each catalog item has two versions of the snapshot stored at:
    - Light: `/actions-assets/design-assets/<design-id-light>.png`
    - Dark: `/actions-assets/design-assets/<design-id-dark>.png`


### Function 4: Embeded Meshery Design
Meshery Design Embedding (docs](https://meshery.io/extensions)) enables you to export a design in a format that can be seamlessly integrated into websites, blogs, or platforms supporting HTML, CSS, and JavaScript. This embedded version provides an interactive representation of the design, making it easier to share with infrastructure stakeholders.

**Relevant Directories**
- `/meshery-design-embed`: Contains the exported design files, including HTML, CSS, JavaScript, and assets like images and fonts. These files can be directly embedded into web pages or applications to showcase the design interactively.

          
    </div>
    <!-- Contributing and Guidelines -->
    <div>
        <h2>Community and Contributing</h2>
        <p>Please do! Code and non-code contributions are welcome. This project is community-built and fosters collaboration. Contributors are expected to adhere to the <a href="https://github.com/cncf/foundation/blob/main/code-of-conduct.md"> CNCF Code of Conduct</a>.
        </p>
        <p>Jump into our <a href="https://slack.meshery.io">Slack</a>! Submit your <a href="https://meshery.io/newcomers">community member form</a> access to additional resources. Don't forget to join the <a href="https://meshery.io/calendar">Newcomers meeting</a> held every Thursday!
        </p>
        <img src="https://raw.githubusercontent.com/meshery/meshery/refs/heads/master/.github/assets/images/readme/community.png"
            style="margin:10px;" width="180px" alt="Community" align="right" />
        <ul>
            ✔️ <b>Star</b> ⭐ the main <a href="https://github.com/meshery/meshery">meshery repo</a><br />
            ✔️ <b>Join</b> any or all of the weekly meetings on the <a href="https://meet.meshery.io">community
                    calendar</a><br />
            ✔️ <b>Watch</b> <a
                    href="https://www.youtube.com/@mesheryio?sub_confirmation=1">community meeting
                    recordings</a><br />
            <p>✔️ <b>Access</b> resources by completing a <a href="https://meshery.io/newcomers"> community member form
                </a><br />
            ✔️ <b>Discuss</b> in a Meshery <a href="https://discuss.meshery.io">Community forum</a><br />
            ✔️ Not sure where to start? <b>Grab</b> an open issue with the <a
                    href="https://github.com/issues?q=is%3Aopen+is%3Aissue+archived%3Afalse+(org%3Ameshery+OR+org%3Aservice-mesh-performance+OR+org%3Aservice-mesh-patterns+OR+org%3Ameshery-extensions)+label%3A%22help+wanted%22">help-wanted
                    label</a><br />
        </ul>
    </div>
    <!-- Footer Section -->
    <img src="https://raw.githubusercontent.com/meshery/.github/master/profile/assets/img/footer.png" align="center" />
</div>
