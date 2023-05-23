# bootPalladio

This repository contains a valid Eclipse Installer index and product catalog. The catalog points to a single Palladio Product file, which is a reproduction of the Palladio Product Feature.

## How to use
First it is necessary to add the code snippet below to the `indices.xmi` file of the Eclipse Installer instance you are using. This usually is located in `<eclipse_installer_root_dir>/configuration/org.eclipse.oomph.setup/indices.xmi`

```
<detail key="https://raw.githubusercontent.com/A7exSchin/bootPalladio/main/org.eclipse.setup">
    <value>Palladio</value>
  </detail>
```
 Secondly, you need to either restart the Eclipse Installer (if it has been opened before the change was made) or start the Installer. In the advanced view in the top right corner change the catalog to `Palladio` by clicking on the arrow next to the folder icon.

 The available product view should update and display a single installable product: the Palladio Bench tooling

 ## Known issues

 - the current setup file does not include the branding feautre which results in a missing icon and splash art. The branding feature currently is not available in the updatesite.
 - it would be preferred to use the official Palladio Product Feature in the setup file, but it is not available on the palladio updatesite