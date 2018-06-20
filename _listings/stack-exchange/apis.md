---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You don???t have to read through a lot of discussion to find the best
  answer.    Like to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Tags
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange My Tags
  x-api-slug: stack-exchange
  description: "Returns the tags the user identified by the access_token passed is
    active in.\n \nThis method returns a list of tags."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/tags
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metags-get-openapi.md
- name: Stack Exchange My Tags Top Answers
  x-api-slug: stack-exchange
  description: "Returns the top 30 answers the user associated with the given access_token
    has posted in response to questions with the given tags.\n \nThis method returns
    a list of answers."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/tags/{tags}/top-answers
  tags: Tags,Anwers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metagstagstopanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metagstagstopanswers-get-openapi.md
- name: Stack Exchange My Tags Top Questions
  x-api-slug: stack-exchange
  description: "Returns the top 30 questions the user associated with the given access_token
    has posted in response to questions with the given tags.\n \nThis method returns
    a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/tags/{tags}/top-questions
  tags: Tags,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metagstagstopquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metagstagstopquestions-get-openapi.md
- name: Stack Exchange My Timeline
  x-api-slug: stack-exchange
  description: "Returns a subset of the actions the user identified by the passed
    access_token has taken on the site.\n \nThis method returns a list of user timeline
    objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/timeline
  tags: Tags,Timeline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metimeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metimeline-get-openapi.md
- name: Stack Exchange My Top Answer Tags
  x-api-slug: stack-exchange
  description: "Returns the user identified by access_token's top 30 tags by answer
    score.\n \nThis method returns a list of top tag objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/top-answer-tags
  tags: Tags,Anwers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metopanswertags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metopanswertags-get-openapi.md
- name: Stack Exchange My Top Question Tags
  x-api-slug: stack-exchange
  description: "Returns the user identified by access_token's top 30 tags by question
    score.\n \nThis method returns a list of top tag objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/top-question-tags
  tags: Tags,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metopquestiontags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/metopquestiontags-get-openapi.md
- name: Stack Exchange Get Tags
  x-api-slug: stack-exchange
  description: "Returns the tags found on a site.\n \nThe inname parameter lets a
    consumer filter down to tags that contain a certain substring. For example, inname=own
    would return both \"download\" and \"owner\" amongst others.\n \nThis method returns
    a list of tags.\n \nThe sorts accepted by this method operate on the follow fields
    of the tag object:\n - popular - count\n - activity - the creation_date of the
    last question asked with the tag\n - name - name\n  popular is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tags-get-openapi.md
- name: Stack Exchange Get Tags Moderator Only
  x-api-slug: stack-exchange
  description: "Returns the tags found on a site that only moderators can use.\n \nThe
    inname parameter lets a consumer filter down to tags that contain a certain substring.
    For example, inname=own would return both \"download\" and \"owner\" amongst others.\n
    \nThis method returns a list of tags.\n \nThe sorts accepted by this method operate
    on the follow fields of the tag object:\n - popular - count\n - activity - the
    creation_date of the last question asked with the tag\n - name - name\n  popular
    is the default sort.\n \n It is possible to create moderately complex queries
    using sort, min, max, fromdate, and todate."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/moderator-only
  tags: Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagsmoderatoronly-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagsmoderatoronly-get-openapi.md
- name: Stack Exchange Get Tags Requred
  x-api-slug: stack-exchange
  description: "Returns the tags found on a site that fulfill required tag constraints
    on questions.\n \nThe inname parameter lets a consumer filter down to tags that
    contain a certain substring. For example, inname=own would return both \"download\"
    and \"owner\" amongst others.\n \nThis method returns a list of tags.\n \nThe
    sorts accepted by this method operate on the follow fields of the tag object:\n
    - popular - count\n - activity - the creation_date of the last question asked
    with the tag\n - name - name\n  popular is the default sort.\n \n It is possible
    to create moderately complex queries using sort, min, max, fromdate, and todate."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/required
  tags: Tags,Required
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagsrequired-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagsrequired-get-openapi.md
- name: Stack Exchange Get Tags Synonyms
  x-api-slug: stack-exchange
  description: "Returns all tag synonyms found a site.\n \nWhen searching for synonyms
    of specific tags, it is better to use /tags/{tags}/synonyms over this method.\n
    \nThe sorts accepted by this method operate on the follow fields of the tag_synonym
    object:\n - creation - creation_date\n - applied - applied_count\n - activity
    - last_applied_date\n  creation is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of tag_synonyms."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/synonyms
  tags: Tags,Synonyms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagssynonyms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagssynonyms-get-openapi.md
- name: Stack Exchange Get Tags FAQ
  x-api-slug: stack-exchange
  description: "Returns the frequently asked questions for the given set of tags in
    {tags}.\n \nFor a question to be returned, it must have all the tags in {tags}
    and be considered \"frequently asked\". The exact algorithm for determining whether
    a question is considered a FAQ is subject to change at any time.\n \n{tags} can
    contain up to 5 individual tags per request.\n \nThis method returns a list of
    questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/{tags}/faq
  tags: Tags,FAQ
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagsfaq-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagsfaq-get-openapi.md
- name: Stack Exchange Get Tags Info
  x-api-slug: stack-exchange
  description: "Returns tag objects representing the tags in {tags} found on the site.\n
    \nThis method diverges from the standard naming patterns to avoid to conflicting
    with existing methods, due to the free form nature of tag names.\n \nThis method
    returns a list of tags.\n \nThe sorts accepted by this method operate on the follow
    fields of the tag object:\n - popular - count\n - activity - the creation_date
    of the last question asked with the tag\n - name - name\n  popular is the default
    sort.\n \n It is possible to create moderately complex queries using sort, min,
    max, fromdate, and todate."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/{tags}/info
  tags: Tags,Information
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagsinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagsinfo-get-openapi.md
- name: Stack Exchange Get Tags Related
  x-api-slug: stack-exchange
  description: "Returns the tags that are most related to those in {tags}.\n \nIncluding
    multiple tags in {tags} is equivalent to asking for \"tags related to tag #1 and
    tag #2\" not \"tags related to tag #1 or tag #2\".\n \ncount on tag objects returned
    is the number of question with that tag that also share all those in {tags}.\n
    \n{tags} can contain up to 4 individual tags per request.\n \nThis method returns
    a list of tags."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/{tags}/related
  tags: Tags,Related
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagsrelated-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagsrelated-get-openapi.md
- name: Stack Exchange Get Tags Synonyms
  x-api-slug: stack-exchange
  description: "Gets all the synonyms that point to the tags identified in {tags}.
    If you're looking to discover all the tag synonyms on a site, use the /tags/synonyms
    methods instead of call this method on all tags.\n \n{tags} can contain up to
    20 individual tags per request.\n \nThe sorts accepted by this method operate
    on the follow fields of the tag_synonym object:\n - creation - creation_date\n
    - applied - applied_count\n - activity - last_applied_date\n  creation is the
    default sort.\n \n It is possible to create moderately complex queries using sort,
    min, max, fromdate, and todate.\n \nThis method returns a list of tag synonyms."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/{tags}/synonyms
  tags: Tags,Synonyms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagssynonyms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagssynonyms-get-openapi.md
- name: Stack Exchange Get Tags Wikis
  x-api-slug: stack-exchange
  description: "Returns the wikis that go with the given set of tags in {tags}.\n
    \nBe aware that not all tags have wikis.\n \n{tags} can contain up to 20 individual
    tags per request.\n \nThis method returns a list of tag wikis."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/{tags}/wikis
  tags: Tags,Wikis
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagswikis-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagswikis-get-openapi.md
- name: Stack Exchange Get Tags Top Answers
  x-api-slug: stack-exchange
  description: "Returns the top 30 answerers active in a single tag, of either all-time
    or the last 30 days.\n \nThis is a view onto the data presented on the tag info
    page on the sites.\n \nThis method returns a list of tag score objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/{tag}/top-answerers/{period}
  tags: Tags,Top Answers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagtopanswerersperiod-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagtopanswerersperiod-get-openapi.md
- name: Stack Exchange Get Tags Top Askers
  x-api-slug: stack-exchange
  description: "Returns the top 30 askers active in a single tag, of either all-time
    or the last 30 days.\n \nThis is a view onto the data presented on the tag info
    page on the sites.\n \nThis method returns a list of tag score objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//tags/{tag}/top-askers/{period}
  tags: Tags,Top Askers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagtopaskersperiod-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/tagstagtopaskersperiod-get-openapi.md
- name: Stack Exchange Get User Tags
  x-api-slug: stack-exchange
  description: "Returns the tags the users identified in {ids} have been active in.\n
    \nThis route corresponds roughly to user's stats tab, but does not include tag
    scores. A subset of tag scores are available (on a single user basis) in /users/{id}/top-answer-tags
    and /users/{id}/top-question-tags.\n \n{ids} can contain up to 100 semicolon delimited
    ids, to find ids programatically look for user_id on user or shallow_user objects.\n
    \nThe sorts accepted by this method operate on the follow fields of the tag object:\n
    - popular - count\n - activity - the creation_date of the last question asked
    with the tag\n - name - name\n  popular is the default sort.\n \n It is possible
    to create moderately complex queries using sort, min, max, fromdate, and todate.\n
    \nThis method returns a list of tags."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/tags
  tags: Users,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidstags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidstags-get-openapi.md
- name: Stack Exchange Get User Tags Top Answers
  x-api-slug: stack-exchange
  description: "Returns the top 30 answers a user has posted in response to questions
    with the given tags.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects. {tags} is limited to 5 tags,
    passing more will result in an error.\n \nThe sorts accepted by this method operate
    on the follow fields of the answer object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of answers."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/tags/{tags}/top-answers
  tags: Users,Tags,Answers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtagstagstopanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtagstagstopanswers-get-openapi.md
- name: Stack Exchange Get User Tags Top Questions
  x-api-slug: stack-exchange
  description: "Returns the top 30 questions a user has asked with the given tags.\n
    \n{id} can contain a single id, to find it programatically look for user_id on
    user or shallow_user objects. {tags} is limited to 5 tags, passing more will result
    in an error.\n \nThe sorts accepted by this method operate on the follow fields
    of the question object:\n - activity - last_activity_date\n - creation - creation_date\n
    - votes - score\n  activity is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/tags/{tags}/top-questions
  tags: Users,Tags,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtagstagstopquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtagstagstopquestions-get-openapi.md
- name: Stack Exchange Get User Top Answers Tags
  x-api-slug: stack-exchange
  description: "Returns a single user's top tags by answer score.\n \nThis a subset
    of the data returned on a user's tags tab.\n \n{id} can contain a single id, to
    find it programatically look for user_id on user or shallow_user objects.\n \nThis
    method returns a list of top_tag objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/top-answer-tags
  tags: Users,Top Answer Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtopanswertags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtopanswertags-get-openapi.md
- name: Stack Exchange Get User Top Question Tags
  x-api-slug: stack-exchange
  description: "Returns a single user's top tags by question score.\n \nThis a subset
    of the data returned on a user's tags tab.\n \n{id} can contain a single id, to
    find it programatically look for user_id on user or shallow_user objects.\n \nThis
    method returns a list of top_tag objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/top-question-tags
  tags: Users,Top Question Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtopquestiontags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/usersidtopquestiontags-get-openapi.md
- name: Stack Exchange
  x-api-slug: stack-exchange
  description: After someone asks a question, members of the community propose answers.
    Others vote on those answers. Very quickly, the answers with the most votes rise
    to the top. You don???t have to read through a lot of discussion to find the best
    answer.    Like to...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tags/master/_listings/stack-exchange/openapi.md
x-common:
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---