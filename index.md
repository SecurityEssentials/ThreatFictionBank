## Welcome to the Threat Fiction Bank

This fiction bank has been created as part of the [FiVu Project](https://spritehub.org/2021/09/02/fivu-using-design-fiction-to-identify-future-vulnerabilities-in-bio-iot/), funded by the [Sprite+ network](https://spritehub.org/) under EPSRC grant [EP/S035869/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/S035869/1).

## The Fictions
<div id="FictionList">
<p>List to replace</p>
</div>

## Support Contact

For questions, additions or suggestions please contact **Dr Cecilia Loureiro-Koechlin** or **Dr Charles Weir**, using the [contact details here](https://spritehub.org/2021/09/02/fivu-using-design-fiction-to-identify-future-vulnerabilities-in-bio-iot/).

<!-- Magic from https://salifm.hashnode.dev/add-javascript-code-in-md-file-for-github-pages-cke4epwmf001oaks16cjggnyc to include JavaScript in an MD file.

The script - starting (async() - inserts the list of PDFs in the root directory into the FictionList div above, is based on https://stackoverflow.com/questions/39048654/how-to-enable-directory-indexing-on-github-pages

-->
<div style="display: none">
    <![CDATA[<script>
    <!--<![CDATA[--><![CDATA[
          (async () => {
    const response = await fetch('https://api.github.com/repos/SecurityEssentials/ThreatFictionBank/contents/');
    const data = await response.json();
    let htmlString = '<ul>';
    for (let file of data) {
      if (/pdf$/.test(file.path)) {
        htmlString += `<li><a href="${file.path}">${file.name}</a></li>`;
      }
    }
    htmlString += '</ul>';
    document.getElementById('FictionList').innerHTML = htmlString;
  })()
    // <![CDATA[
    </script><![CDATA[]]>
</div>
