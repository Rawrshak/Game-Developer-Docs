# Static 3D Object Asset

#### 1. Make sure the 3D Static Object follows the Asset Framework

If not, please check out the tutorial below first:

{% content-ref url="../3d-static-object-in-game-framework.md" %}
[3d-static-object-in-game-framework.md](../3d-static-object-in-game-framework.md)
{% endcontent-ref %}

#### 2. Create Parent Object and set asset to child object

Create a new empty Game Object

![Created empty 'FRS' object](<../../../../.gitbook/assets/image (25) (1).png>)

Make sure the orientation is (0,0,0), location is (0,0,0), and scale is (1,1,1)

![FRS's default location, orientation, and scale](<../../../../.gitbook/assets/image (17) (1).png>)

Drag the SCI\_FRS\_13\_HD inside the FRS game object.

![Set FRS to the parent of SCI\_FRS\_13\_HD object](<../../../../.gitbook/assets/image (4) (1).png>)

{% hint style="info" %}
Note: These logical groupings are just as an example. As all the necessary objects are under one Parent game object (in this case, FRS), it's fine to change the child grouping to your liking.
{% endhint %}

#### 3. Create a Prefab

Drag the "FRS" parent object into the Model folder to create a prefab.

![Drag the object to the project folder to create a prefab](<../../../../.gitbook/assets/image (24) (1).png>)

#### 4. Set the Prefab's AssetBundle

In the bottom of the Inspector, set the Assetbundle name. In this case, we set it to "frs"

![Set Asset Bundle name](<../../../../.gitbook/assets/image (13) (1).png>)

#### 5. Create the Asset Bundle

In the menu, select _Rawrshak -> Asset Bundles_

This opens the Rawrshak's Asset Bundles creator (Asset Packager)

Select the desired _Build Target_ to build an asset package for. In this case, select _StandaloneWindows._

![Select Build Target](<../../../../.gitbook/assets/image (26) (1).png>)

Click _Generate Asset Bundles ****_ button and wait for the asset bundle to be built.&#x20;

{% hint style="info" %}
If you selected Android, iOS, and WebGL, Unity may have to install the necessary modules during the asset bundle generation if these modules were not already installed earlier. This might take a while.
{% endhint %}

#### 6. Viewing the generated Asset Bundle

![Viewing Generated Asset Bundle information](<../../../../.gitbook/assets/image (3).png>)

You can click the row of the asset bundle that was generated to view the asset bundle information on the right.

If you click the select checkboxes, you can add the total amount of kilobytes of data you will need to upload. You can click the "Calculator" button to open [ArDrive's price calculator](https://prices.ardrive.io).

{% hint style="warning" %}
The Asset Information viewer is editable so that the developer may copy it to the asset launcher. However, if the developer changes any of the information, it is not saved.&#x20;

The developer should not change any of this information as this is autogenerated.
{% endhint %}
