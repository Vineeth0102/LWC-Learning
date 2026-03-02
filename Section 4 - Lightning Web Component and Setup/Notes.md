<h2>Lightning Framework</h2>

The Lightning Component framework is a UI framework for developing single page applications for mobile and desktop devices.

Lightning Components using two programming models

1. Aura components Model
2. Lightning Web Component Model

<h2>Web Stack transformation</h2>

![alt text](image.png)

<h2>Aura vs LWC</h2>
<h3>Aura</h3>
<ul>
<li>Aura wad build on ES6(2009) javascript version </li>
<li>too much code to write </li>
<li>Rendering wasn't optimized</li>
<li>mordern features was not available like modules, classes and promises</li>
</ul>

<h3>LWC</h3>
    <ul>
    <li>LWC was build on mordern ES versions</li>
    <li>they have features like Shadow dom, web components, custom elements, template and slots.</li>
    </ul>

<h2>What is Lightning Web Components</h2>

Lightning Web Components is a new programming model for building Lightning components. It uses the core concepts of Web standards.

<h3>Benefits:</h3>

1. Lightweight framework
2. Better Performance
3. No need to learn different framework to develop salesforce applications
4. Interoperability with lightning Aura components
5. Better testing using Jest
6. Better Security

<h2>Coexistence and interoperability</h2>

Aura components and Lightning web components can coexist and interoperate and they share the same high level services:
<ul>
    <li>Aura components and Lightning web components can coexist on the same page.</li>
    <li>Aura components can include Lightning web components but not other way around.</li>
    <li>Aura components and Lightning web components share the same base Lightning components. Base Lightning components were alredy implemented as Lightning web components.</li>
    <li>Aura components and Lightning web components share the same underlying services (Lightning Data Service, User Interface API, etc).</li>
</ul>

<h2>Lightning Experience</h2>

Lightning Experience is the new user interface (UI) for salesforce installations; It is a significant upgarde from the salesforce classic view, brining modern apearance and functionality to the salesforce platfrom.

<h2>Salesforce Developer Experience (DX)</h2>

It is a set of tools that streamlines the entire development life cycle. It improves team development and collaboration, facilitates automated testing and continuous integration and makes the release cycle more efficent and agile.

1. Visual Studio Code
2. Salesforce CLI
3. Salesforce Extension Pack

<b>My Domain</b> - Having a custom domain is more secure, some salesforce features require it.

<h2>Dev Hub</h2>

we have to enable dev hub to

1. Create and manage orgs from the command line
2. view information about Scratch orgs
3. Link Namespace orgs

<h2>DevHub vs Scratch org</h2>

<b>Dev Hub</b> - its is the main Salesforce org that you will use to create and manage your scratch orgs.
<b>Scratch Org</b> - it us a source-driven and disposable deployment of salesforce code and metadata. Scratch orgs are driven by source, Sandboxes are copies of production.

<b>Note</b> - Scratch orgs do not replace sandboxes.

<h2>Project creation</h2>

    sfdx force:project:create -n "LWC project"
    -n : new project

<h2>Authorization of org</h2>

    sfdx force:auth:web:login -a lwcLearning -d
    -a : alias
    -d : default

<h2>Scratch Org Creation</h2>

    Add hasSampleData:"true" property to project-scratch-def.json

    sfdx force:org:create -a lwcScratchOne -d 30 -f config/project-scratch-def.json -s
    -a : alias
    -d : days(number of days scratch org alive 1 day min and 30 days max)
    -f : file location of project scratch definition json
    -s : set it to default username

<b>Note</b> : if anytime we encouter error "no org configuration for name" then run the following command.

    sfdx force:config:set defaultdevhubusername="the DX DevHub username"

