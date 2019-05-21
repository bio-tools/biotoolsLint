# What is biotoolsLint?

**biotoolsLint is under design : coding has not started and this page may be missing information**

**biotoolsLint** is a utility for verification and reporting of content of the [ELIXIR Tools & Data Services Registry](https://bio.tools).  It will, for purposes of content quality control and labelling, verify the content according to:
* tool description syntax defined by [biotoolsSchema](https://github.com/bio-tools/biotoolsSchema)
* correct or recommended use of the [EDAM ontology](https://github.com/edamontology/edamontology/)
* curation best practice from the bio.tools [Curators Guide](https://biotools.readthedocs.io/en/latest/curators_guide.html) (in so far as these recommendations can be automatically verified)
* compliance to the [Tool Information Standard](https://bio-tools.github.io/Tool-Information-Standard/)
* miscellaneous other checks, *e.g.* broken link detection, tool name uniqueness *etc.* 


## Verifications 

The verifications are exhaustively tabulated below, including one table / element group defined in biotoolsSchema.

### Element-specific verifications

![summary group](images/tool.png)


- [Summary group](https://github.com/bio-tools/biotoolslint#summary-group)
- [Function group](https://github.com/bio-tools/biotoolslint#function-group)
- [Labels group](https://github.com/bio-tools/biotoolslint#labels-group)
- [Links group](https://github.com/bio-tools/biotoolslint#links-group)
- [Downloads group](https://github.com/bio-tools/biotoolslint#downloads-group)
- [Documentation group](https://github.com/bio-tools/biotoolslint#documentation-group)
- [Publications group](https://github.com/bio-tools/biotoolslint#publications-group)
- [Credits group](https://github.com/bio-tools/biotoolslint#credits-group)


### General verifications

- [EDAM verifications](https://github.com/bio-tools/biotoolslint#edam)
- [Genera verifications](https://github.com/bio-tools/biotoolslint#general)



## Summary group

See <a href=https://biotoolsschema.readthedocs.io/en/latest/biotoolsschema_elements.html#summary-group>schema docs</a> & <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#summary-group>curators guide</a>

![summary group](images/summary.png)

![otherid](images/otherid.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>


<!--- summary->name --->

<tr><td colspan="4"><b>name:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#name>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#name-tool>curators guide</a> </td></tr>
<tr>
    <td>Invalid cardinality (1 only allowed)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/33>33</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Name is taken (not unique within bio.tools)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/30>30<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes technical jargon</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/31>31<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes version or status info</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/26>26<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Name similarity (full-length exact match to substring of existing tool name)</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/32>32<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->description --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>description:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#description>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#description>curators guide</a> </td></tr>
<tr>
    <td>Invalid cardinality (1 only allowed)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/33>33</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Wrong or missing capitalisation and full stops</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/35>35<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes DOI(s)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/28>28<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes URL(s)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/27>27<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->homepage --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>homepage:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#homepage>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#homepage>curators guide</a> </td></tr>
<tr>
    <td>Invalid cardinality (1 only allowed)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/33>33</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Broken link</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/12>12<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Uses existing tool homepage URL</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/38>38<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->biotoolsID --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>biotoolsID:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#biotoolsid>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#id105>curators guide</a> </td></tr>

<tr>
    <td>Mismatch of biotoolsID & biotoolsCURIE</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/22>22<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->biotoolsCURIE --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>biotoolsCURIE:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#biotoolscurie>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#biotoolscurie>curators guide</a> </td></tr>

<tr>
    <td>Mismatch of biotoolsID & biotoolsCURIE</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/22>22<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->version --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>version:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#version>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#version-tool>curators guide</a> </td></tr>

<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->otherID --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>otherID:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#other-ids>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#other-ids>curators guide</a> </td></tr>

<tr><td colspan="4"><b>otherID->value</b>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>otherID->type</b>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>otherID->version</b>
<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>


## Function group

See <a href=https://biotoolsschema.readthedocs.io/en/latest/biotoolsschema_elements.html#function-group>schema docs</a> & <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#function-group>curators guide</a>

![function group](images/function.png)

![operation](images/operation.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>


<!--- function->operation --->

<tr><td colspan="4"><b>operation:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#operation>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#operation>curators guide</a> </td></tr>

<tr><td colspan="4"><b>operation->uri</b></tr>
<tr>
    <td>Duplicated EDAM concept</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/3>3</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Placeholder EDAM concept (not normally used for annotation)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/10>10</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Deprecated EDAM concept</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/6>6</a></td>
    <td>tbd</td>
</tr>
<tr><td colspan="4"><b>operation->term</b></tr>
<tr>
    <td>Invalid term</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/7>7</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Use of synonym</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/7>7</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Undefined Operation::Topic relation</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/41>41</a></td>
    <td>tbd</td>
</tr>
</table>