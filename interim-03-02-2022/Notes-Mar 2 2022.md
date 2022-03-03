SCIM Virtual Session
March 2, 2022

Chairs: Nancy Cam-Winget, Aaron Parecki
Area Director: Roman Danyliw
Notetakers: Paul Lanzi

Attending:
Nancy Cam-Widget
Julien Schneider Aubriga
Danny Zollner
Paulo Jorge N. Correia
Phil Hunt
Paul Lanzi
Matt Peterson
Janelle Allen
Danny Mayer
Aaron Parecki
Bojitha Piyathilake
Anuradha Karunarathna
Rashmini
Chmutali
Nick Wooler
Alice Wang
Qingwen Cheng
Chetan Desai
Mike Kiser


Agenda:
- Introduction of new co-chair: Aaron Parecki
- Progress updates:
    - Use Cases
    - Schema and Protocol
- IETF113 Agenda Items
- AOB

Discussion:
- Welcome to Aaron as co-chair!
- Encourage group to be more vocal on slack/email list; didn't get any proposals for agenda items for this meeting
    - Danny Z: have some suggested topics for AOB (ex: how to securely handle pictures/photos)
    - Janelle: would like to introduce github repo for doc collaboration
- Use Case Document Update (Danny/Janelle)
    - Danny had recent meeting; not sure how much progress has been made since the last draft (which was shared). Feels closer to a rewrite of the Use Cases rather than a clarification/update; deep amount of work on this.
    - for IETF113 - objective could be to outline the current thinking on the use cases and possibly a rough outline (even if the format doesn't yet comply with the RFC format/structure)? Danny Z to check with Pam Dingle on current status on this and reply back to mailing list and/or slack.
    - Noted that Elliot has content to contribute to Use Cases

- Schema and Protocol updates
    - Janelle: Suggest we need to take a pass through the errata to update the SCIM 2.0 before moving on to the 'beyond SCIM 2.0 work' otherwise discussed
        - need to distinguish between bugs and errata
        - Janelle setup Github that resembles other IETF working group's githubs to track these issues and carry forward into new drafts, dispose of, etc.
        - Plan to use 'issues' in Github to track bugs/errata/etc and also store unsubmitted + submitted document drafts in github
        - Discussion about using github automation/tooling to move from 'draft' to 'submitted', etc. Nancy noted the naming convention for the doc title changes as the doc moves through the process.
    - This process to be used for both Schema and Protocol doc updates
    - Danny Z: Do we push to move SCIM 2.0 from Proposed Draft to Internet Draft, or just focus on 'SCIM 3.0' (informal name)? Consensus was to move the standard forward. Extending 2.0 with extensions (rather than creating a compendium 3.0) is more straightforward (and we'd need to process 2.0 errata/bugs, etc. either way)
        - Allocate time in the plenary session to discuss this
        - Discussion about interoperability and backward compatibility as an undocumented objective
        - Phil: noted that mechanism (in the URL) for /v2 vs /v3 for backward compatibility, etc. Possibly not well implemented IRL because there hasn't been a major change, historically.
        - Should we have a 'best practices' document for SCIM (similar to OAuth best practices)?
            - Discussion of this and test suite as good clarifiers for SCIM spec
            - Discussion of availability of tables at IETF for interop testing and hackathon (though these require prep work)
            - Noted that interop testing is not in the IETF or this group's charter but still a good activity to discuss / support so that we can check the validity of what we're creating
    - In conclusion, there hasn't been any "pen to paper" on the updates, but anticipate this is a smaller body of work than the full rewrite that's happening with Use Cases


- Document mechanics
    - Deadline to submit documents is next week, and portal opens up again during the meeting to submit new documents
    - Preparing documents:
        - Phil H: suggest to attend the 'IETF Draft Writing Seminar' the weekend before the meeting as several structure changes have been implemented, and it's a bit tedious (though powerful).
        - Janelle: suggest using cramdown to make the markdown easier
        - Discussion about using XML vs. markdown vs. cramdown. Noted that there are tools available here: https://tools.ietf.org/ (Phil has found these work better running locally than online)
        - Paul created new slack channel: #writing-docs and posted these links

- AOB
    - Danny Z - securing user profile photos
        - Background: SCIM server sending (especially over the internet) the URIs for user profile pictures. SCIM standard today says just include the URI and the SCIM server will provide it; there is no discussion in the spec about securing the picture (with, for instance, authentication)
        - Anyone interested in writing an extension draft, contact Danny Z
        - Is this a confidentiality (privacy) or authenticity/integrity problem?
        - Discussion about challenges -  the very cross-domain nature of SCIM and how do you authenticate requests like this across domains
        - Matt: it's up to the server providing the photo to handle authentication / Phil: the SCIM server is just providing the URI, it's not actually hosting the photo
        - Phil: There is a general enhancement worth discussing which is meta-data around whether a claim (attribute) has been verified. E.g. was the email verified.
    - Janelle - Github collaboration
        - Created new github repo for working versions of documents. Is this OK to do? Nancy: As long as we have two distinct sub-projects: one for adopted documents, one for Work In Progress (WIP) documents.
        - Discussion about mechanics of draft processing
        - Nancy will take another look at this; typically only grant write access to the authors (anyone can submit pull requests). Aaron and Janelle will help Nancy with this.


- IETF 113 Proposed Agenda slots (one, 2 hour session)
    - Use Cases progress and discussion (Pam D)
    - Protocol Updates Discussion (Jannelle/Danny)
    - Schema Updates Discussion (Jannelle/Danny)
    - OIDF Shared Signals and Events (SSE) Introduction (Nancy, 10 mins)
    - SCIM SSE Events Profile (draft-hunt-scim-events) (Phil, 10 mins)
    - Nancy needs to post rough agenda by end of this week (maybe sooner)