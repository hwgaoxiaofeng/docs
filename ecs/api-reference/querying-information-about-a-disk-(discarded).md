# Querying Information About a Disk \(Discarded\)<a name="EN-US_TOPIC_0065817711"></a>

## Function<a name="en-us_topic_0057973212_section18673210"></a>

This API is used to query information about a specified disk.

## Constraints<a name="en-us_topic_0057973212_section53828184"></a>

-   This API will be discarded. You are advised to use the EVS API "Querying Details About a Single EVS Disk \(Native OpenStack API V2\)".

## URI<a name="en-us_topic_0057973212_section33841163"></a>

GET /v2/\{project\_id\}/os-volumes/\{volume\_id\}

GET /v2.1/\{project\_id\}/os-volumes/\{volume\_id\}

[Table 1](#en-us_topic_0057973212_table2814978410562)  describes the parameters in the URI.

**Table  1**  Parameter description

<a name="en-us_topic_0057973212_table2814978410562"></a>
<table><thead align="left"><tr id="en-us_topic_0057973212_row4149654710562"><th class="cellrowborder" valign="top" width="33%" id="mcps1.2.4.1.1"><p id="p5187119"><a name="p5187119"></a><a name="p5187119"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="23%" id="mcps1.2.4.1.2"><p id="p17503500"><a name="p17503500"></a><a name="p17503500"></a>Mandatory</p>
</th>
<th class="cellrowborder" valign="top" width="44%" id="mcps1.2.4.1.3"><p id="p8497414"><a name="p8497414"></a><a name="p8497414"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="en-us_topic_0057973212_row3491217610562"><td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p931403110562"><a name="en-us_topic_0057973212_p931403110562"></a><a name="en-us_topic_0057973212_p931403110562"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p1623904210562"><a name="en-us_topic_0057973212_p1623904210562"></a><a name="en-us_topic_0057973212_p1623904210562"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.3 "><p id="p37593705"><a name="p37593705"></a><a name="p37593705"></a>Specifies the project ID.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row168831648104912"><td class="cellrowborder" valign="top" width="33%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p588311484495"><a name="en-us_topic_0057973212_p588311484495"></a><a name="en-us_topic_0057973212_p588311484495"></a>volume_id</p>
</td>
<td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p5883148154912"><a name="en-us_topic_0057973212_p5883148154912"></a><a name="en-us_topic_0057973212_p5883148154912"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p788310481495"><a name="en-us_topic_0057973212_p788310481495"></a><a name="en-us_topic_0057973212_p788310481495"></a>Specifies the disk ID.</p>
</td>
</tr>
</tbody>
</table>

## Request<a name="en-us_topic_0057973212_section41255355"></a>

None

## Response<a name="en-us_topic_0057973212_section35753879"></a>

[Table 2](#en-us_topic_0057973212_table27581142)  describes the response parameters.

**Table  2**  Response parameters

<a name="en-us_topic_0057973212_table27581142"></a>
<table><thead align="left"><tr id="en-us_topic_0057973212_row31073981"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p62404314"><a name="p62404314"></a><a name="p62404314"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p3528183"><a name="p3528183"></a><a name="p3528183"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p17347392"><a name="p17347392"></a><a name="p17347392"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="en-us_topic_0057973212_row49449215"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p45963511"><a name="en-us_topic_0057973212_p45963511"></a><a name="en-us_topic_0057973212_p45963511"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p32056895"><a name="en-us_topic_0057973212_p32056895"></a><a name="en-us_topic_0057973212_p32056895"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p6109664"><a name="en-us_topic_0057973212_p6109664"></a><a name="en-us_topic_0057973212_p6109664"></a>Specifies the disk ID in UUID format.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row54986980"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p24760409"><a name="en-us_topic_0057973212_p24760409"></a><a name="en-us_topic_0057973212_p24760409"></a>displayName</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p59436098"><a name="en-us_topic_0057973212_p59436098"></a><a name="en-us_topic_0057973212_p59436098"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p57742226"><a name="en-us_topic_0057973212_p57742226"></a><a name="en-us_topic_0057973212_p57742226"></a>Specifies the disk name.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row49917988"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p16825232"><a name="en-us_topic_0057973212_p16825232"></a><a name="en-us_topic_0057973212_p16825232"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p20666548"><a name="en-us_topic_0057973212_p20666548"></a><a name="en-us_topic_0057973212_p20666548"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p33321799"><a name="en-us_topic_0057973212_p33321799"></a><a name="en-us_topic_0057973212_p33321799"></a>Specifies the disk status.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row31460736"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p65291693"><a name="en-us_topic_0057973212_p65291693"></a><a name="en-us_topic_0057973212_p65291693"></a>attachments</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p54135799"><a name="en-us_topic_0057973212_p54135799"></a><a name="en-us_topic_0057973212_p54135799"></a>Array of objects</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p44871424"><a name="en-us_topic_0057973212_p44871424"></a><a name="en-us_topic_0057973212_p44871424"></a>Specifies the attachment information about a disk.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row1189633"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p29251466"><a name="en-us_topic_0057973212_p29251466"></a><a name="en-us_topic_0057973212_p29251466"></a>availabilityZone</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p20558515"><a name="en-us_topic_0057973212_p20558515"></a><a name="en-us_topic_0057973212_p20558515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p62709254"><a name="en-us_topic_0057973212_p62709254"></a><a name="en-us_topic_0057973212_p62709254"></a>Specifies the AZ to which the disk belongs.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row27512376"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p13910022"><a name="en-us_topic_0057973212_p13910022"></a><a name="en-us_topic_0057973212_p13910022"></a>createdAt</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p52970008"><a name="en-us_topic_0057973212_p52970008"></a><a name="en-us_topic_0057973212_p52970008"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p46529834"><a name="en-us_topic_0057973212_p46529834"></a><a name="en-us_topic_0057973212_p46529834"></a>Specifies the time when the disk was created.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row16115327"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p30273100"><a name="en-us_topic_0057973212_p30273100"></a><a name="en-us_topic_0057973212_p30273100"></a>displayDescription</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p36202017"><a name="en-us_topic_0057973212_p36202017"></a><a name="en-us_topic_0057973212_p36202017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p23168261"><a name="en-us_topic_0057973212_p23168261"></a><a name="en-us_topic_0057973212_p23168261"></a>Specifies the disk description.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row7187765"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p45338124"><a name="en-us_topic_0057973212_p45338124"></a><a name="en-us_topic_0057973212_p45338124"></a>volumeType</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p48509390"><a name="en-us_topic_0057973212_p48509390"></a><a name="en-us_topic_0057973212_p48509390"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p39879225"><a name="en-us_topic_0057973212_p39879225"></a><a name="en-us_topic_0057973212_p39879225"></a>Specifies the disk type.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row23368709"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p13817278"><a name="en-us_topic_0057973212_p13817278"></a><a name="en-us_topic_0057973212_p13817278"></a>snapshotId</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p45457768"><a name="en-us_topic_0057973212_p45457768"></a><a name="en-us_topic_0057973212_p45457768"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p16629678"><a name="en-us_topic_0057973212_p16629678"></a><a name="en-us_topic_0057973212_p16629678"></a>Specifies the snapshot ID.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row15449375"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p43439845"><a name="en-us_topic_0057973212_p43439845"></a><a name="en-us_topic_0057973212_p43439845"></a>metadata</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p28966593"><a name="en-us_topic_0057973212_p28966593"></a><a name="en-us_topic_0057973212_p28966593"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p64623316"><a name="en-us_topic_0057973212_p64623316"></a><a name="en-us_topic_0057973212_p64623316"></a>Specifies the disk metadata.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row44738940"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p67084362"><a name="en-us_topic_0057973212_p67084362"></a><a name="en-us_topic_0057973212_p67084362"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p65124208"><a name="en-us_topic_0057973212_p65124208"></a><a name="en-us_topic_0057973212_p65124208"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p64903654"><a name="en-us_topic_0057973212_p64903654"></a><a name="en-us_topic_0057973212_p64903654"></a>Specifies the disk size.</p>
</td>
</tr>
</tbody>
</table>

**Table  3** **attachments**  field description

<a name="en-us_topic_0057973212_table10694153118228"></a>
<table><thead align="left"><tr id="en-us_topic_0057973212_row1770213111229"><th class="cellrowborder" valign="top" width="26.502650265026507%" id="mcps1.2.4.1.1"><p id="p16689725015"><a name="p16689725015"></a><a name="p16689725015"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="24.81248124812481%" id="mcps1.2.4.1.2"><p id="p6681718507"><a name="p6681718507"></a><a name="p6681718507"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="48.684868486848686%" id="mcps1.2.4.1.3"><p id="p0822755015"><a name="p0822755015"></a><a name="p0822755015"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="en-us_topic_0057973212_row17709183112211"><td class="cellrowborder" valign="top" width="26.502650265026507%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p5711203142219"><a name="en-us_topic_0057973212_p5711203142219"></a><a name="en-us_topic_0057973212_p5711203142219"></a>device</p>
</td>
<td class="cellrowborder" valign="top" width="24.81248124812481%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p371215313222"><a name="en-us_topic_0057973212_p371215313222"></a><a name="en-us_topic_0057973212_p371215313222"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.684868486848686%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p87146313224"><a name="en-us_topic_0057973212_p87146313224"></a><a name="en-us_topic_0057973212_p87146313224"></a>Specifies the directory to which the disk is mounted.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row11715153182215"><td class="cellrowborder" valign="top" width="26.502650265026507%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p197177319224"><a name="en-us_topic_0057973212_p197177319224"></a><a name="en-us_topic_0057973212_p197177319224"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="24.81248124812481%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p1719183182216"><a name="en-us_topic_0057973212_p1719183182216"></a><a name="en-us_topic_0057973212_p1719183182216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.684868486848686%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p97211331142215"><a name="en-us_topic_0057973212_p97211331142215"></a><a name="en-us_topic_0057973212_p97211331142215"></a>Specifies the ID of the attached resource.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row117221431132216"><td class="cellrowborder" valign="top" width="26.502650265026507%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p37244312222"><a name="en-us_topic_0057973212_p37244312222"></a><a name="en-us_topic_0057973212_p37244312222"></a>serverId</p>
</td>
<td class="cellrowborder" valign="top" width="24.81248124812481%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p11726103113222"><a name="en-us_topic_0057973212_p11726103113222"></a><a name="en-us_topic_0057973212_p11726103113222"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.684868486848686%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p18728731122219"><a name="en-us_topic_0057973212_p18728731122219"></a><a name="en-us_topic_0057973212_p18728731122219"></a>Specifies the ECS ID.</p>
</td>
</tr>
<tr id="en-us_topic_0057973212_row1729193182219"><td class="cellrowborder" valign="top" width="26.502650265026507%" headers="mcps1.2.4.1.1 "><p id="en-us_topic_0057973212_p673013122218"><a name="en-us_topic_0057973212_p673013122218"></a><a name="en-us_topic_0057973212_p673013122218"></a>volumeId</p>
</td>
<td class="cellrowborder" valign="top" width="24.81248124812481%" headers="mcps1.2.4.1.2 "><p id="en-us_topic_0057973212_p1573210319222"><a name="en-us_topic_0057973212_p1573210319222"></a><a name="en-us_topic_0057973212_p1573210319222"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.684868486848686%" headers="mcps1.2.4.1.3 "><p id="en-us_topic_0057973212_p97342312223"><a name="en-us_topic_0057973212_p97342312223"></a><a name="en-us_topic_0057973212_p97342312223"></a>Specifies the ID of the attached disk.</p>
</td>
</tr>
</tbody>
</table>

## Example Request<a name="section1916812241102"></a>

```
GET https://{endpoint}/v2/b84c367e4d1047fc9b54f28b400ddbc2/os-volumes/70b14513-faad-4646-b7ab-a065cef282b4
GET https://{endpoint}/v2.1/b84c367e4d1047fc9b54f28b400ddbc2/os-volumes/70b14513-faad-4646-b7ab-a065cef282b4
```

## Example Response<a name="section79186115409"></a>

```
{
    "volume": 
    {
        "status": "available",
        "attachments": [{}],
        "availabilityZone": "nova",
        "createdAt": "2016-05-20T07:57:56.299000",
        "displayDescription": null,
        "volumeType": null,
        "dispalyName": "test",
        "snapshotId": null,
        "metadata": {},
        "id": "70b14513-faad-4646-b7ab-a065cef282b4",
        "size": 1    
    }
}
```

## Returned Values<a name="en-us_topic_0057973212_en-us_topic_0020212692_section22960139"></a>

See  [Returned Values for General Requests](returned-values-for-general-requests.md).

