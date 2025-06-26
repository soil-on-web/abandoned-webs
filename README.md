# Abandoned Webs

A listing of abandoned websites on soil/land

Are you following a link from an ancient report to a non existing website? Create an [issue](../../issues) or [pull request](../../pulls)

Aim of this repo is to set up a list of abandoned websites related to land & soil information, on one hand to notify upcoming initiatives to consider url persistence, on the other hand to recover the lost information 
from repositories such as [archive.org](https://web.archive.org). If funding permits, it would be nice to reclaim the lost domains.

- [globalsoilmap.net](https://web.archive.org/web/20180712112423/http://globalsoilmap.net/)
- [http://www.contaminatedland.co.uk](https://web.archive.org/web/20070228165308/http://www.contaminatedland.co.uk/) 
- [http://pesera.jrc.it](https://web.archive.org/web/20040626144114/http://pesera.jrc.it/default/show.gx?_app.page=show-USR.html&Object.object_id=KM------0000000000000002) 
- [https://srtm.usgs.gov](https://web.archive.org/web/20071103132819/http://srtm.usgs.gov/) 
- [http://vitalsigns.org](http://web.archive.org/web/20220525222027/http://vitalsigns.org/get-data)
- `hijacked` [https://recare-project.eu](http://web.archive.org/web/20180219053548/https://recare-project.eu/)
- [http://www.arc.agric.za](https://web.archive.org/web/20050204061521/http://www.arc.agric.za/main/about.htm)
- [https://soilhealth7.gov.in](http://web.archive.org/web/20220915171923/https://soilhealth7.gov.in/)
- [https://www.lifeadaptamed.eu](https://www.lifeadaptamed.eu/?page_id=1650&lang=en)
- [https://carbonaction.org](https://web.archive.org/web/20220809222132/https://carbonaction.org/en/)
- [http://lifeforesmit.com](https://web.archive.org/web/20220303112921/http://lifeforesmit.com/it/)
- [http://h2020.inspiration-agenda.eu](https://web.archive.org/web/20220307214050/http://h2020.inspiration-agenda.eu/)
- `hijacked` [https://landmark2020.eu](https://web.archive.org/web/20220103222100/http://landmark2020.eu/)
- ~~`hijacked`~~ [http://www.soiltrec.eu](https://web.archive.org/web/20150907120620/http://www.soiltrec.eu/)
- [http://isosoil.eu](https://web.archive.org/web/20160109220858/http://isosoil.eu/)
- ~~`hijacked`~~ [http://www.upsoil.eu](https://web.archive.org/web/20141124001344/http://www.upsoil.eu/)
- [http://www.citychlor.eu](https://web.archive.org/web/20141124001345/http://www.citychlor.eu/)
- [http://www.timbre-project.eu](https://web.archive.org/web/20141124001344/http://www.timbre-project.eu/)
- `hijacked` [https://cobwebproject.eu/](https://web.archive.org/web/20170808073521/https://cobwebproject.eu/)
- [https://sislac.org](https://web.archive.org/web/20160726023137/http://www.sislac.org/)
- [gssoil-portal.eu](https://web.archive.org/web/20131009224121/http://gssoil-portal.eu/ingrid-portal/)
- `hijacked` [landmark2020.eu](https://web.archive.org/web/20220310125101/https://landmark2020.eu/)
- [removal-project.com](https://web.archive.org/web/20240822131212/https://www.removal-project.com/)
- [soilmissionsupport.eu](https://web.archive.org/web/20220925172454/https://www.soilmissionsupport.eu/)


## Good practices on url persistence of temporary websites

### For dissemination teams/web publishers

- Use a subdomain of an established organisation (prevents hijacking of the domain at domain expiration, indicates ownership), else pre-pay the domain ownership (not the hosting) for at least the upcoming 10 years.
- Use a persistent identifier framework, such as [DOI](https://doi.org) as identifiers for your resources (At website cancelation/move, the DOI can be rerouted to the new location).
- Set up [rewrite rules](https://en.wikipedia.org/wiki/Rewrite_engine) at website cancelation.
- Use minimal technology, yes: `html`; no: ~~wordpress, drupal, liferay, databases, react, angular, vue.js~~. Consider to use [Static Site Generators](https://about.gitlab.com/blog/2022/04/18/comparing-static-site-generators/).
- Keep website content minimal, set up a [one page website](https://www.web.com/blog/one-page-vs-multi-page-website/), from there link to external (persistent) resources.

### For report writers

Another reason why links on reports end up broken is because report writers often just copy a url from the browser bar and paste it in a report.
As a report writer, when selecting a relevant url to use in your report:

- Assess the likelyhood of persistence of the resource (if unsure, contact the authors), else consider to not include a direct link in the report. For example, do not link to a project website, but link to a registry where the project is described (for example [cordis](https://cordis.europa.eu)).
- Verify if the resource has a DOI, handle.net, w3id.org identifier attached, if so use that identifier.
- Remove all sorts of parameters at the end of the url. However before removing them, verify the url is still operational (and points to the relevant content). Try splitting the url at `#`, `?` or `/`.
- In the source of the website (view source/inspect), look for the `<link rel="canonical" href="http://example.com"/>` element in `<head>`, and use the value from `href`, this is the [canonical url](https://en.wikipedia.org/wiki/Canonical_link_element), used for example by search engines. 
