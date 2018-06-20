---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get User Top Answers Tags
  description: "Returns a single user's top tags by answer score.\n \nThis a subset
    of the data returned on a user's tags tab.\n \n{id} can contain a single id, to
    find it programatically look for user_id on user or shallow_user objects.\n \nThis
    method returns a list of top_tag objects."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/tags:
    get:
      summary: My Tags
      description: "Returns the tags the user identified by the access_token passed
        is active in.\n \nThis method returns a list of tags."
      operationId: returns-the-tags-the-user-identified-by-the-access-token-passed-is-active-in-this-method-returns-a-l
      x-api-path-slug: metags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
  /me/tags/{tags}/top-answers:
    get:
      summary: My Tags Top Answers
      description: "Returns the top 30 answers the user associated with the given
        access_token has posted in response to questions with the given tags.\n \nThis
        method returns a list of answers."
      operationId: returns-the-top-30-answers-the-user-associated-with-the-given-access-token-has-posted-in-response-to
      x-api-path-slug: metagstagstopanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Anwers
  /me/tags/{tags}/top-questions:
    get:
      summary: My Tags Top Questions
      description: "Returns the top 30 questions the user associated with the given
        access_token has posted in response to questions with the given tags.\n \nThis
        method returns a list of questions."
      operationId: returns-the-top-30-questions-the-user-associated-with-the-given-access-token-has-posted-in-response-
      x-api-path-slug: metagstagstopquestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Questions
  /me/timeline:
    get:
      summary: My Timeline
      description: "Returns a subset of the actions the user identified by the passed
        access_token has taken on the site.\n \nThis method returns a list of user
        timeline objects."
      operationId: returns-a-subset-of-the-actions-the-user-identified-by-the-passed-access-token-has-taken-on-the-site
      x-api-path-slug: metimeline-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Timeline
  /me/top-answer-tags:
    get:
      summary: My Top Answer Tags
      description: "Returns the user identified by access_token's top 30 tags by answer
        score.\n \nThis method returns a list of top tag objects."
      operationId: returns-the-user-identified-by-access-tokens-top-30-tags-by-answer-score-this-method-returns-a-list-
      x-api-path-slug: metopanswertags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Anwers
  /me/top-question-tags:
    get:
      summary: My Top Question Tags
      description: "Returns the user identified by access_token's top 30 tags by question
        score.\n \nThis method returns a list of top tag objects."
      operationId: returns-the-user-identified-by-access-tokens-top-30-tags-by-question-score-this-method-returns-a-lis
      x-api-path-slug: metopquestiontags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Questions
  /tags:
    get:
      summary: Get Tags
      description: "Returns the tags found on a site.\n \nThe inname parameter lets
        a consumer filter down to tags that contain a certain substring. For example,
        inname=own would return both \"download\" and \"owner\" amongst others.\n
        \nThis method returns a list of tags.\n \nThe sorts accepted by this method
        operate on the follow fields of the tag object:\n - popular - count\n - activity
        - the creation_date of the last question asked with the tag\n - name - name\n
        \ popular is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate."
      operationId: returns-the-tags-found-on-a-site-the-inname-parameter-lets-a-consumer-filter-down-to-tags-that-conta
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/moderator-only:
    get:
      summary: Get Tags Moderator Only
      description: "Returns the tags found on a site that only moderators can use.\n
        \nThe inname parameter lets a consumer filter down to tags that contain a
        certain substring. For example, inname=own would return both \"download\"
        and \"owner\" amongst others.\n \nThis method returns a list of tags.\n \nThe
        sorts accepted by this method operate on the follow fields of the tag object:\n
        - popular - count\n - activity - the creation_date of the last question asked
        with the tag\n - name - name\n  popular is the default sort.\n \n It is possible
        to create moderately complex queries using sort, min, max, fromdate, and todate."
      operationId: returns-the-tags-found-on-a-site-that-only-moderators-can-use-the-inname-parameter-lets-a-consumer-f
      x-api-path-slug: tagsmoderatoronly-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/required:
    get:
      summary: Get Tags Requred
      description: "Returns the tags found on a site that fulfill required tag constraints
        on questions.\n \nThe inname parameter lets a consumer filter down to tags
        that contain a certain substring. For example, inname=own would return both
        \"download\" and \"owner\" amongst others.\n \nThis method returns a list
        of tags.\n \nThe sorts accepted by this method operate on the follow fields
        of the tag object:\n - popular - count\n - activity - the creation_date of
        the last question asked with the tag\n - name - name\n  popular is the default
        sort.\n \n It is possible to create moderately complex queries using sort,
        min, max, fromdate, and todate."
      operationId: returns-the-tags-found-on-a-site-that-fulfill-required-tag-constraints-on-questions-the-inname-param
      x-api-path-slug: tagsrequired-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Required
  /tags/synonyms:
    get:
      summary: Get Tags Synonyms
      description: "Returns all tag synonyms found a site.\n \nWhen searching for
        synonyms of specific tags, it is better to use /tags/{tags}/synonyms over
        this method.\n \nThe sorts accepted by this method operate on the follow fields
        of the tag_synonym object:\n - creation - creation_date\n - applied - applied_count\n
        - activity - last_applied_date\n  creation is the default sort.\n \n It is
        possible to create moderately complex queries using sort, min, max, fromdate,
        and todate.\n \nThis method returns a list of tag_synonyms."
      operationId: returns-all-tag-synonyms-found-a-site-when-searching-for-synonyms-of-specific-tags-it-is-better-to-u
      x-api-path-slug: tagssynonyms-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: min
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Synonyms
  /tags/{tags}/faq:
    get:
      summary: Get Tags FAQ
      description: "Returns the frequently asked questions for the given set of tags
        in {tags}.\n \nFor a question to be returned, it must have all the tags in
        {tags} and be considered \"frequently asked\". The exact algorithm for determining
        whether a question is considered a FAQ is subject to change at any time.\n
        \n{tags} can contain up to 5 individual tags per request.\n \nThis method
        returns a list of questions."
      operationId: returns-the-frequently-asked-questions-for-the-given-set-of-tags-in-tags-for-a-question-to-be-return
      x-api-path-slug: tagstagsfaq-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tags
        description: String list (semicolon delimited)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - FAQ
  /tags/{tags}/info:
    get:
      summary: Get Tags Info
      description: "Returns tag objects representing the tags in {tags} found on the
        site.\n \nThis method diverges from the standard naming patterns to avoid
        to conflicting with existing methods, due to the free form nature of tag names.\n
        \nThis method returns a list of tags.\n \nThe sorts accepted by this method
        operate on the follow fields of the tag object:\n - popular - count\n - activity
        - the creation_date of the last question asked with the tag\n - name - name\n
        \ popular is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate."
      operationId: returns-tag-objects-representing-the-tags-in-tags-found-on-the-site-this-method-diverges-from-the-st
      x-api-path-slug: tagstagsinfo-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Information
  /tags/{tags}/related:
    get:
      summary: Get Tags Related
      description: "Returns the tags that are most related to those in {tags}.\n \nIncluding
        multiple tags in {tags} is equivalent to asking for \"tags related to tag
        #1 and tag #2\" not \"tags related to tag #1 or tag #2\".\n \ncount on tag
        objects returned is the number of question with that tag that also share all
        those in {tags}.\n \n{tags} can contain up to 4 individual tags per request.\n
        \nThis method returns a list of tags."
      operationId: returns-the-tags-that-are-most-related-to-those-in-tags-including-multiple-tags-in-tags-is-equivalen
      x-api-path-slug: tagstagsrelated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tags
        description: String list (semicolon delimited)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Related
  /tags/{tags}/synonyms:
    get:
      summary: Get Tags Synonyms
      description: "Gets all the synonyms that point to the tags identified in {tags}.
        If you're looking to discover all the tag synonyms on a site, use the /tags/synonyms
        methods instead of call this method on all tags.\n \n{tags} can contain up
        to 20 individual tags per request.\n \nThe sorts accepted by this method operate
        on the follow fields of the tag_synonym object:\n - creation - creation_date\n
        - applied - applied_count\n - activity - last_applied_date\n  creation is
        the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of tag synonyms."
      operationId: gets-all-the-synonyms-that-point-to-the-tags-identified-in-tags-if-youre-looking-to-discover-all-the
      x-api-path-slug: tagstagssynonyms-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: min
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Synonyms
  /tags/{tags}/wikis:
    get:
      summary: Get Tags Wikis
      description: "Returns the wikis that go with the given set of tags in {tags}.\n
        \nBe aware that not all tags have wikis.\n \n{tags} can contain up to 20 individual
        tags per request.\n \nThis method returns a list of tag wikis."
      operationId: returns-the-wikis-that-go-with-the-given-set-of-tags-in-tags-be-aware-that-not-all-tags-have-wikis-t
      x-api-path-slug: tagstagswikis-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tags
        description: String list (semicolon delimited)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Wikis
  /tags/{tag}/top-answerers/{period}:
    get:
      summary: Get Tags Top Answers
      description: "Returns the top 30 answerers active in a single tag, of either
        all-time or the last 30 days.\n \nThis is a view onto the data presented on
        the tag info page on the sites.\n \nThis method returns a list of tag score
        objects."
      operationId: returns-the-top-30-answerers-active-in-a-single-tag-of-either-alltime-or-the-last-30-days-this-is-a-
      x-api-path-slug: tagstagtopanswerersperiod-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: path
        name: period
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Top Answers
  /tags/{tag}/top-askers/{period}:
    get:
      summary: Get Tags Top Askers
      description: "Returns the top 30 askers active in a single tag, of either all-time
        or the last 30 days.\n \nThis is a view onto the data presented on the tag
        info page on the sites.\n \nThis method returns a list of tag score objects."
      operationId: returns-the-top-30-askers-active-in-a-single-tag-of-either-alltime-or-the-last-30-days-this-is-a-vie
      x-api-path-slug: tagstagtopaskersperiod-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: path
        name: period
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Top Askers
  /users/{ids}/tags:
    get:
      summary: Get User Tags
      description: "Returns the tags the users identified in {ids} have been active
        in.\n \nThis route corresponds roughly to user's stats tab, but does not include
        tag scores. A subset of tag scores are available (on a single user basis)
        in /users/{id}/top-answer-tags and /users/{id}/top-question-tags.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the tag object:\n - popular -
        count\n - activity - the creation_date of the last question asked with the
        tag\n - name - name\n  popular is the default sort.\n \n It is possible to
        create moderately complex queries using sort, min, max, fromdate, and todate.\n
        \nThis method returns a list of tags."
      operationId: returns-the-tags-the-users-identified-in-ids-have-been-active-in-this-route-corresponds-roughly-to-u
      x-api-path-slug: usersidstags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
  /users/{id}/tags/{tags}/top-answers:
    get:
      summary: Get User Tags Top Answers
      description: "Returns the top 30 answers a user has posted in response to questions
        with the given tags.\n \n{id} can contain a single id, to find it programatically
        look for user_id on user or shallow_user objects. {tags} is limited to 5 tags,
        passing more will result in an error.\n \nThe sorts accepted by this method
        operate on the follow fields of the answer object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of answers."
      operationId: returns-the-top-30-answers-a-user-has-posted-in-response-to-questions-with-the-given-tags-id-can-con
      x-api-path-slug: usersidtagstagstopanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: id
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
      - Answers
  /users/{id}/tags/{tags}/top-questions:
    get:
      summary: Get User Tags Top Questions
      description: "Returns the top 30 questions a user has asked with the given tags.\n
        \n{id} can contain a single id, to find it programatically look for user_id
        on user or shallow_user objects. {tags} is limited to 5 tags, passing more
        will result in an error.\n \nThe sorts accepted by this method operate on
        the follow fields of the question object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of questions."
      operationId: returns-the-top-30-questions-a-user-has-asked-with-the-given-tags-id-can-contain-a-single-id-to-find
      x-api-path-slug: usersidtagstagstopquestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: id
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
      - Questions
  /users/{id}/top-answer-tags:
    get:
      summary: Get User Top Answers Tags
      description: "Returns a single user's top tags by answer score.\n \nThis a subset
        of the data returned on a user's tags tab.\n \n{id} can contain a single id,
        to find it programatically look for user_id on user or shallow_user objects.\n
        \nThis method returns a list of top_tag objects."
      operationId: returns-a-single-users-top-tags-by-answer-score-this-a-subset-of-the-data-returned-on-a-users-tags-t
      x-api-path-slug: usersidtopanswertags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Top Answer Tags
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---