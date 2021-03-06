# Deleting a Cluster<a name="dws_02_0021"></a>

## Function<a name="s7aa3de1b44f14c0487bab690bb5702d6"></a>

This API is used to delete clusters. All resources, including customer data, of the deleted cluster will be released. For data security reasons, create a snapshot for the cluster that you want to delete before deleting the cluster.

## URI<a name="s9db56e76e7694a5cbfd993c7d1db0606"></a>

-   URI format

    DELETE /v1.0/\{project\_id\}/clusters/\{cluster\_id\}

-   Parameter description

    **Table  1**  URI parameter description

    <a name="tb301b46821994ee6ae8cb5d508bfd564"></a>
    <table><thead align="left"><tr id="r09f2cf7e302f4b1197b293cb5b91aa42"><th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.1"><p id="ad24f94544e3448e588d569b4cf5d3df1"><a name="ad24f94544e3448e588d569b4cf5d3df1"></a><a name="ad24f94544e3448e588d569b4cf5d3df1"></a><strong id="b84235270617228"><a name="b84235270617228"></a><a name="b84235270617228"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="a23ce55ff78b64009b06caaddea7be777"><a name="a23ce55ff78b64009b06caaddea7be777"></a><a name="a23ce55ff78b64009b06caaddea7be777"></a><strong id="b6167984116271"><a name="b6167984116271"></a><a name="b6167984116271"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="11%" id="mcps1.2.5.1.3"><p id="aa68a5c620b7741ebb873bc22f4abf72b"><a name="aa68a5c620b7741ebb873bc22f4abf72b"></a><a name="aa68a5c620b7741ebb873bc22f4abf72b"></a><strong id="b84235270617235"><a name="b84235270617235"></a><a name="b84235270617235"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="56.99999999999999%" id="mcps1.2.5.1.4"><p id="a5c07a285f796424888ea8c9b215ef172"><a name="a5c07a285f796424888ea8c9b215ef172"></a><a name="a5c07a285f796424888ea8c9b215ef172"></a><strong id="b842352706172443"><a name="b842352706172443"></a><a name="b842352706172443"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rd49c40cc2e534fb38fc1ce2158dda6da"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="adf89366c8cdf490b91f7ab0b1aa4c9d7"><a name="adf89366c8cdf490b91f7ab0b1aa4c9d7"></a><a name="adf89366c8cdf490b91f7ab0b1aa4c9d7"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a03a216c626564f1eb88d9562a41ee374"><a name="a03a216c626564f1eb88d9562a41ee374"></a><a name="a03a216c626564f1eb88d9562a41ee374"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a9bf19da6d557419eb7768b4c0d4dc441"><a name="a9bf19da6d557419eb7768b4c0d4dc441"></a><a name="a9bf19da6d557419eb7768b4c0d4dc441"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.99999999999999%" headers="mcps1.2.5.1.4 "><p id="p1266145715419"><a name="p1266145715419"></a><a name="p1266145715419"></a>Project ID. For details about how to obtain the project ID, see <a href="obtaining-a-project-id.md">Obtaining a Project ID</a>.</p>
    </td>
    </tr>
    <tr id="r3f1019a86e164120957b6c78183aed5c"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="ac8206c593fb6478d90922a1317be1af3"><a name="ac8206c593fb6478d90922a1317be1af3"></a><a name="ac8206c593fb6478d90922a1317be1af3"></a>cluster_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a723b9ebdf5d14520ac6db771eea07716"><a name="a723b9ebdf5d14520ac6db771eea07716"></a><a name="a723b9ebdf5d14520ac6db771eea07716"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a42225196447a466a8b27488e9f840018"><a name="a42225196447a466a8b27488e9f840018"></a><a name="a42225196447a466a8b27488e9f840018"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.99999999999999%" headers="mcps1.2.5.1.4 "><p id="a3c9219ff8f544b6db2665fbab0057dab"><a name="a3c9219ff8f544b6db2665fbab0057dab"></a><a name="a3c9219ff8f544b6db2665fbab0057dab"></a>ID of the cluster to be deleted</p>
    </td>
    </tr>
    </tbody>
    </table>


## Request<a name="sa64d5fde1cb94be29689b1aab5bc2bb2"></a>

-   Sample request

    ```
    DELETE /v1.0/89cd04f168b84af6be287f71730fdb4b/clusters/4ca46bf1-5c61-48ff-b4f3-0ad4e5e3ba90
    {
        "keep_last_manual_snapshot":0
    }
    ```


-   Parameter description

    **Table  2**  Request parameter description

    <a name="tc32f843a9ead4035a871c86d7a4846cf"></a>
    <table><thead align="left"><tr id="rcf972ba57cb945bca28c72ec13f32fb4"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="a04409112453b4054b07ce0e5d3fd7aac"><a name="a04409112453b4054b07ce0e5d3fd7aac"></a><a name="a04409112453b4054b07ce0e5d3fd7aac"></a><strong id="b996190862"><a name="b996190862"></a><a name="b996190862"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.2.5.1.2"><p id="ac42ccdeeb5ca426cba55f7d3103a3e4d"><a name="ac42ccdeeb5ca426cba55f7d3103a3e4d"></a><a name="ac42ccdeeb5ca426cba55f7d3103a3e4d"></a><strong id="b595356906"><a name="b595356906"></a><a name="b595356906"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.5.1.3"><p id="a3be50d1d99d643778bb995586c600e14"><a name="a3be50d1d99d643778bb995586c600e14"></a><a name="a3be50d1d99d643778bb995586c600e14"></a><strong id="b1027434767"><a name="b1027434767"></a><a name="b1027434767"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="50.505050505050505%" id="mcps1.2.5.1.4"><p id="a028e0ec2d58b47edb787e6e49333ec7f"><a name="a028e0ec2d58b47edb787e6e49333ec7f"></a><a name="a028e0ec2d58b47edb787e6e49333ec7f"></a><strong id="b917594809"><a name="b917594809"></a><a name="b917594809"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="recb12ef1d4f24c248e72fa202d02918c"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="aa79b2667616f4f9f84a72005adac2a74"><a name="aa79b2667616f4f9f84a72005adac2a74"></a><a name="aa79b2667616f4f9f84a72005adac2a74"></a>keep_last_manual_snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="a6219947762bf4127ad4313192186f4b0"><a name="a6219947762bf4127ad4313192186f4b0"></a><a name="a6219947762bf4127ad4313192186f4b0"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.5.1.3 "><p id="a49c27493d4b44d74ae91d624f93bb313"><a name="a49c27493d4b44d74ae91d624f93bb313"></a><a name="a49c27493d4b44d74ae91d624f93bb313"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.505050505050505%" headers="mcps1.2.5.1.4 "><p id="a7c97c57ca08b420c93d593eed95ed934"><a name="a7c97c57ca08b420c93d593eed95ed934"></a><a name="a7c97c57ca08b420c93d593eed95ed934"></a>Number of snapshots that you want to reserve for a cluster</p>
    </td>
    </tr>
    </tbody>
    </table>


## Response<a name="saf8285fea2964e558a059d985c498559"></a>

Sample response

```
STATUS CODE 202
```

## Returned Value<a name="s318da95b204f47c4bef42e78b54a9089"></a>

-   Normal

    202

-   Abnormal 

    **Table  3**  Returned value description

    <a name="tfd7a877a4eed4992a077edb0bb8f7352"></a>
    <table><thead align="left"><tr id="red5a03b5306f46e0900cacc8c992c838"><th class="cellrowborder" valign="top" width="46.46%" id="mcps1.2.3.1.1"><p id="a72e8066c2a994394ba0ece17bd467376"><a name="a72e8066c2a994394ba0ece17bd467376"></a><a name="a72e8066c2a994394ba0ece17bd467376"></a><strong id="b84235270610542"><a name="b84235270610542"></a><a name="b84235270610542"></a>Returned Value</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="53.54%" id="mcps1.2.3.1.2"><p id="a2982bcdae3bb45f8b90b4baeef64cc05"><a name="a2982bcdae3bb45f8b90b4baeef64cc05"></a><a name="a2982bcdae3bb45f8b90b4baeef64cc05"></a><strong id="b1103661966"><a name="b1103661966"></a><a name="b1103661966"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r5d0fed0ce30740a49f01318c52c42592"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="ae37fb97120e94cbea677f88d0ab4edbd"><a name="ae37fb97120e94cbea677f88d0ab4edbd"></a><a name="ae37fb97120e94cbea677f88d0ab4edbd"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="ac2c1c94571004267a7297152e7edb7fc"><a name="ac2c1c94571004267a7297152e7edb7fc"></a><a name="ac2c1c94571004267a7297152e7edb7fc"></a>Request error.</p>
    </td>
    </tr>
    <tr id="r45192eae966e4de885d09edc4b3eee3c"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="adfc757440c4849e09a2516b04e8a1d01"><a name="adfc757440c4849e09a2516b04e8a1d01"></a><a name="adfc757440c4849e09a2516b04e8a1d01"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="af986420c033c45dea198eb80d6c07471"><a name="af986420c033c45dea198eb80d6c07471"></a><a name="af986420c033c45dea198eb80d6c07471"></a>Authentication failed.</p>
    </td>
    </tr>
    <tr id="r41d8f90f2d864d6b92339cf01794c677"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="a24892b03923545f48aa72a00f90ac7d3"><a name="a24892b03923545f48aa72a00f90ac7d3"></a><a name="a24892b03923545f48aa72a00f90ac7d3"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="a6ac5aa0c4d654b33aa51c2193a5b6e83"><a name="a6ac5aa0c4d654b33aa51c2193a5b6e83"></a><a name="a6ac5aa0c4d654b33aa51c2193a5b6e83"></a>You do not have the rights to perform the operation.</p>
    </td>
    </tr>
    <tr id="rb2e58285b54e40058c475f72290b1e68"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="a3a8f1a544d714b28b85c80856fe07ae5"><a name="a3a8f1a544d714b28b85c80856fe07ae5"></a><a name="a3a8f1a544d714b28b85c80856fe07ae5"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="a75dc6f72a9044650829d4fd51c48beb5"><a name="a75dc6f72a9044650829d4fd51c48beb5"></a><a name="a75dc6f72a9044650829d4fd51c48beb5"></a>The requested resource was not found.</p>
    </td>
    </tr>
    <tr id="r02aba20d19bc40bea95f3b9dc09780c1"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="ade198c372ecb4b6786369a2cd1d0a5dc"><a name="ade198c372ecb4b6786369a2cd1d0a5dc"></a><a name="ade198c372ecb4b6786369a2cd1d0a5dc"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="ad8ec7dfac3ae464f86a085852ac0db58"><a name="ad8ec7dfac3ae464f86a085852ac0db58"></a><a name="ad8ec7dfac3ae464f86a085852ac0db58"></a>Internal service error.</p>
    </td>
    </tr>
    <tr id="r77f8af8054384d23bf198428f13a207b"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="a73100e054b9840dd80134200f3624a23"><a name="a73100e054b9840dd80134200f3624a23"></a><a name="a73100e054b9840dd80134200f3624a23"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="a7d16065e572f480a95470cafcc622e7b"><a name="a7d16065e572f480a95470cafcc622e7b"></a><a name="a7d16065e572f480a95470cafcc622e7b"></a>The service is unavailable.</p>
    </td>
    </tr>
    </tbody>
    </table>


