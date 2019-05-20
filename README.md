# What is biotoolsLint?
**biotoolsLint** is a utility (under design!) for verification and reporting of content of the [ELIXIR Tools & Data Services Registry](https://bio.tools).  It will verify the content according to the bio.tools [Curators Guide](https://biotools.readthedocs.io/en/latest/curators_guide.html), Tool Information Standard(https://bio-tools.github.io/Tool-Information-Standard/) and other checks, and produce reports for puposes of content quality control and labelling.


**Table below will comprehensively list all validations (in progress)**


**Summary group:** <a href=https://biotoolsschema.readthedocs.io/en/latest/biotoolsschema_elements.html#summary-group>schema docs</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#summary-group>curators guide</a>)

<table>
<tr>
    <td>Validation</td>
    <td>Log level</td>
    <td>Issue</td>
    <td>Status</td>
</tr>
  
<tr><td colspan="4"><b>name:</b> <a href=https://biotools.readthedocs.io/en/latest/api_usage_guide.html#name>API usage</a>, <a href=https://biotools.readthedocs.io/en/latest/curators_guide.html#name-tool#curators guide>curators guide</a> </td></tr>
<tr>
    <td>Invalid cardinality (1 only allowed)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/>tbd</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Name is taken (not unique within bio.tools)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/30>30<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/>tbd<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/>tbd<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Name similarity (full-length exact match to substring of existing tool name)</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-tools/biotoolsLint/issues/>tbd<a/></td>
    <td>tbd</td>
</tr>