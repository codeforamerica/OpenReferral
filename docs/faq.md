# Frequently Asked Questions

This FAQ provides context for the Open Referral Initiative and its Human Services Data Specification (HSDS). You can read more about Open Referral at [https://openreferral.org](https://openreferral.org)


### What is Open Referral? 

The Open Referral Initiative is a network of people and organizations working to promote the accessibility of information about health, human, and social services — i.e. _community resource directory data_.

Our Human Service Data Specification (HSDS, AKA ‘the Open Referral format’) is a data exchange format that enables resource directory data to be shared among heterogeneous information systems. The Human Service Data API suite (HSDA) is a set of standardized OpenAPI protocols.

Open Referral’s ecosystem includes a range of open source tools and web applications that facilitate the flow of resource directory information. See [examples of these tools and apps here](https://openreferral.org/about/technology-overview/).

More tools are in development by members of Open Referral’s network, members of which are primarily assembled in [our Google Group](https://groups.google.com/forum/#!forum/openreferral) and [our Slack team](https://openreferral.org/get-involved/join-our-slack-team/).


### Who started Open Referral? 

Greg Bloom is the instigator and lead organizer of Open Referral, which emerged from work done in the DC Open211 project, and which was first described [Towards a Community Data Commons](http://http//beyondtransparency.org/chapters/part-5/towards-a-community-data-commons/), an essay published in Code for America’s 2013 book _Beyond Transparency_.

Our work was initially co-sponsored by [Code for America](https://www.codeforamerica.org/blog/2014/08/05/open-referral-initiative-a-standard-for-the-safety-net/) and the Ohana Project, with funding from the Knight Foundation.


### Who is the audience for Open Referral? Who benefits?

There are three types of _ultimate_ stakeholders for Open Referral: 1) people in need of help of some kind (_‘help-seekers’_); 2) people who are in some kind of position to assist such help-seekers (_‘service providers’_); and 3) _‘analysts’_ — i.e. researchers, policymakers, funders and anyone seeking to understand the patterns of resource allocation in their community.

The _primary_ users of Open Referral are _database administrators –_ anyone involved in aggregating, maintaining, and/or developing systems that produce or consume community resource directory data. Our objective is to help such database administrators share higher quality resource directory data at lower cost, with the goal of making it easier for people to find such information across a wide array of channels.

Read more about each of these types of users [here in our User Personas documentation](https://docs.google.com/document/d/1XqueBVbRVgR0BVGjDbUdN4suUYfMKm7yJm1f3nRsGtY/edit?usp=drive_web).


### How is this project relevant to me? 

Open Referral helps people and organizations grapple with the complex problem of maintaining and publishing reliable information about the health, human, and social services available to people in need.

Most of our work does not involve writing code. We facilitate collaborative action among institutions that have mutual interest in cooperation.

That said, Open Referral is an open network. Anyone is free to use our data specification and tools in pursuit of our shared goals.

If you have resource directory data that you wish to make more available — or if there’s an organization in your community that might make its data more broadly accessible, then you could get to work right away.

Read more in our Contributors Guide. Reach out to info@openreferral.org to get directly in touch.


### If I maintain a community resource directory — or if I partner with an organization that does — how would I get started? 

You can start by testing the viability of our format for your context. That may entail [mapping your database's schema to the Human Services Data Specification](http://docs.openreferral.org/en/latest/hsds/formatting/).

Once you've mapped your schema to ours, analyze the gaps. (You can ask questions or submit suggestions for improvements to our schema in [our Issues Queue](https://github.com/openreferral/specification/issues). Read more in [our Contributors Guide](https://github.com/openreferral/specification/blob/master/CONTRIBUTING.md).)

Then you can write a script to transform your data into this open format.

Finally, you can deploy an open source resource database (like [ORServices](https://sarapis.org/human-services/orservices/)), load your transformed data in, and start building new tools that can help people in your community use this data in new ways.

If you have questions about how this might be useful in your community, please reach out to info@openreferral.org


### How are decisions made about the Open Referral specifications?

Our governance model is structured around three activities: 1) a semi-regular Assembly video call, open to all participants [see an archive of these videos [here](https://www.youtube.com/channel/UCtbojLVi_ti_MWyGD2-AM4A)], 2) convenings of diverse stakeholders in Open Referral workshops [read the reportback [here](https://docs.google.com/document/d/1kivG6TTw1LKhJRAQHeqH7fTIxZZaDojXRRBYEd_ltWw/edit)], and 3) ad hoc ‘workgroups’ consisting of leaders with a varied set of perspectives and experiences [see the workgroup archive [here](http://groups.google.com/forum/#!forum/openreferral-workgroup)].

Of all the feedback received from many different contributors, we assign priority to the perspectives of the lead stakeholders of our pilot projects. This feedback is submitted to Open Referral's deputized technical leads, who ultimately make decisions with documentation and established methods for future review.

[Open Referral’s initial governance model is [described in more detail in this memo](https://docs.google.com/document/d/16sZXY6nQZJqq-TJaaLY2K3pE2G__q1myYX8JC3ZKHmk/edit). You can also read more about the nature of this ‘polycentric’ approach to governance in [Derek Coursen’s blog post here](http://openreferral.org/toward-seamless-information-referral-polycentric-experiment/).]


### What is the Human Services Data Specification (HSDS)?

AKA 'the Open Referral format,' the HSDS is a data interchange format that enables resource directory data to be published in bulk for use by many systems. HSDS provides a common vocabulary for information about services, the organizations that provide them, and the locations where they can be accessed. HSDS is essentially an _interlingua_ — in other words, it’s a common language that can be used by anyone to enable community resource directories to ’talk’ to each other. [[See the data specification in Github](https://github.com/OpenReferral/specification) or on [our Documentation Site](https://openreferral.readthedocs.io/).]


### What is in the Human Services Data Specification (HSDS)?

First, HSDS identifies a vocabulary of terms that describe what a service is, the institution that provides it, where the service can be accessed, and how to access it. These terms are designated as ‘required,’ ‘recommended,’ and ‘optional.’ The spec provides instructions for formatting these terms, with examples.

On a more technical level, HSDS also includes a [logical model](http://docs.openreferral.org/en/latest/hsds/logical_model/) that diagrams the relationships between these terms.

Finally, HSDS provides guidance for structuring and packaging data so that it can be published on the web and/or exchanged between systems. [See: [Github](https://github.com/codeforamerica/openreferral/specification) or [our documentation site](https://openreferral.readthedocs.io/).]


### What is not in the Human Services Data Specification (HSDS)? 

HSDS does not attempt to describe every type of information that might be relevant to people working with resource directory data. We have attempted to maintain a strict focus on specifying only relevant factual attributes that are shared by _most_ services. That means we excluded many kinds of information that are unique to specific kinds of services (such as the accreditation of child care providers, or the availability of beds in a shelter).

HSDS also does not specify a taxonomy of types of services and types of personal attributes that determine eligibility for various types of services. Many such taxonomies already exist, so HSDS merely provides instructions for how to overlay a taxonomy of the user’s choosing. By default, information systems that use HSDS can use the open source [Open Eligibility taxonomy](http://openeligibility.org/). (Expect future cycles of the Open Referral initiative to take on these issues more directly; however, for now we are merely looking to learn from the different ways in which various users address these common problems.)

Finally, HSDS does not specify any information regarding how referrals actually get made (i.e. setting appointments, following up, etc) or feedback regarding the quality of those services. These kinds of information are critically important, but inherently so variable and context-dependent that we don’t think it’s feasible or appropriate to specify them at this point in time.

That said, this model can and should be extended! Users can expand HSDS to meet their own needs, in their own systems. Groups of stakeholders from particular subdomains can develop extended ‘profiles’ that are tailored to their situation. ([A group of civil legal service providers](https://groups.google.com/forum/#!forum/legalaid-openreferral) have already begun working on precisely that.) In future iterations of the Open Referral process, these expansions will then be considered for inclusion as part of the primary model.


### What is the format of the HSDS? Why CSV?

With the goal of broad accessibility in mind, the initial HSDS developer Sophia Parafina chose Comma-Separated Values (CSV) as the building blocks for HSDS. CSV serves as a ‘lowest common denominator’ that is simplest to use and most accessible to users with a modicum of technical abilities, as it can be edited in a simple text editor, and ingested by almost any information system. (For more reasoning behind this decision, consider Waldo Jaquith’s recent post, [‘In Praise of CSV.’](https://usopendata.org/2015/03/10/csv/))

For version 1.0, Parafina chose to accompany a more-complex set of CSV files with a JSON datapackage (using [the Open Knowledge Foundation's frictionless data specification](http://frictionlessdata.io/)) to describe the CSVs' contents. In version 1.2, with support from Open Knowledge Foundation’s Frictionless Data Fund, [Shelby Switzer upgraded the handling of JSON datapackages. ](https://openreferral.org/introducing-open-referrals-data-transformation-toolkit/)

Members of the Open Referral community have observed that they may need more structured data formats for use cases that involve complex, sensitive, and/or large-scale uses. We recognize the validity of these perspectives, and in fact we expect the HSDS model to evolve over time. Pilot projects and community members are already discussing plans to develop complementary formats (such as XML and JSON-LD) — and as these formats are field-tested and validated, they may become formal components of HSDS in future iterations.


### How do you address the matter of taxonomy (of types of services and situations)? 

Open Referral recognizes the existence of a diverse array of taxonomies to describe types of services, organizations, and people for whom services are available. Given that such categories are inherently subjective, whereas Open Referral's format is describing only factual data, we do not prescribe a specific taxonomy. We do [recognize the existence of an array of taxonomies currently in use](https://github.com/openreferral/specification/blob/master/docs/design_principles.md#related-taxonomies), and our HSDS format [includes specifications for including any taxonomy in open data](http://docs.openreferral.org/en/latest/hsds/reference/#service_taxonomy).


### How does Open Referral handle eligibility criteria?

Good question. We don't currently specify a standardized method for structuring eligibility criteria. The kinds of eligibility rules are so variable and often complex and nuanced that we have not tried to develop a standardized set of them. By default, information systems that use HSDS can use the open source [Open Eligibility taxonomy](http://openeligibility.org/). (Expect future cycles of the Open Referral initiative to take on these issues more directly; however, for now we are merely looking to learn from the different ways in which various users address these common problems.)


### What if I collect important information that isn't included in the Human Service Data specification?

That's ok! The Human Services Data Specification is an extensible format to which additional layers of information can be added — [see guidance here](http://docs.openreferral.org/en/latest/hsds/extending/). (But we'd like to learn from your experience, so please share these insights!)


### What if the Human Service Data Specification requires kinds of information that I don't collect? 

The Open Referral format has been developed to require a pretty minimal set of information. If your resource directory doesn’t contain certain required elements, we may need to get creative. Ask in [our Issues queue](https://github.com/openreferral/specification/issues) for clarification and context, and we'll try to answer you promptly.


### What if I need help collecting this data in the first place?

Open Referral is working to build tools to help produce and verify accurate resource directory data. If you’re interested in developing such tools — and/or if you already have experience with such tools — we want to hear from you! Please reach out to info@openreferral.org to discuss.


### Who has adapted this project and can I see examples? 

We have [a network of projects around the United States, Canada, and beyond](https://openreferral.org/about/projects/). [See this network map here](http://kumu.io/Bloom/open-referral-network-map).

Some domain-specific groups have adapted our data specification to their context, such as [the Human Services Data Model](https://openreferral.org/introducing-the-humanitarian-service-data-model/) (in the field of Humanitarian Crisis Response).


### Who do I contact if I need help with this project? 

You can contact Greg Bloom ([@greggish](https://github.com/greggish) | bloom@openreferral.org), the chief organizing officer for Open Referral.


### What languages is this project in? 

Currently Open Referral is in English, though we have at least one Spanish deployment [in Madrid](https://openreferral.org/huertas-de-datos-open-referral-in-madrid/) :)

Oh, do you mean machine language? Our data specification calls for CSV files with a JSON datapackage. Our primary reference implementation, [ORServices](https://github.com/sarapis/orservices), is in Laravel.


### If I wanted to help with this project, what is the best way to do that?

Get in touch with Greg at bloom@openreferral.org. You can also start by finding other people in your community who work with information systems that keep track of the health, human, and social services available to people in need.

You could also look through [our Issues queue](https://github.com/openreferral/specification/issues), comment away, and even offer Pull Requests to our documentation with your own documentation of why. It might be a while before we are able to address your issue directly, but your feedback is very welcome as it helps us set our agenda!


### Is the project in active development?

The Human Services Data Specification is entering an upgrade phase of development, under the interim leadership of the [Open Data Services Cooperative](http://opendataservices.coop/). [Check out our issues queue](https://github.com/openreferral/specification/issues).

We are seeking sponsorship to support long-term institutional development of Open Referral and our data specification. Please reach out to info@openreferral.org for more information.


### What is the licensing on this project?

[Human Services Data Specification v2.0 is now available](https://github.com/openreferral/specification/blob/master/LICENSE) as [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).


<!-- Footnotes themselves at the bottom. -->
## Notes

[^1]:
     _This is a modified version of[ the Open Knowledge Foundation's Open Data definition](http://okfn.org/opendata/)._
