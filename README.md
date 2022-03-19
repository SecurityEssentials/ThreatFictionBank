## Welcome to the Threat Fiction Bank

Repository for 'threat fictions': short fictional pieces to inspire developers and others carrying out cybersecurity threat assessment.

This fiction bank has been created as part of the [FiVu Project](https://spritehub.org/2021/09/02/fivu-using-design-fiction-to-identify-future-vulnerabilities-in-bio-iot/), funded by the [Sprite+ network](https://spritehub.org/) under EPSRC grant [EP/S035869/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/S035869/1).

## The Fictions

## Support Contact

For questions, additions or suggestions please contact **Dr Cecilia Loureiro-Koechlin** or **Dr Charles Weir**, using the [contact details here](https://spritehub.org/2021/09/02/fivu-using-design-fiction-to-identify-future-vulnerabilities-in-bio-iot/).

    <script>
      (async () => {
        const response = await fetch('https://api.github.com/repos/SecurityEssentials/ThreatFictionBank/contents/');
        const data = await response.json();
        let htmlString = '<ul>';
        for (let file of data) {
          htmlString += `<li><a href="${file.path}">${file.name}</a></li>`;
        }
        htmlString += '</ul>';
        document.getElementsByTagName('body')[0].innerHTML = htmlString;
      })()
    </script>
