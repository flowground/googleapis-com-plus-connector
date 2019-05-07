# ![LOGO](logo.png) Google+ **flow**ground Connector

## Description

A generated **flow**ground connector for the Google+ API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/plus/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:51+03:00

## API Description

Builds on top of the Google+ platform.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Search public activities.

*Tags:* `activities`

#### Input Parameters
* `language` - _optional_ - Specify the preferred language to search with. See search language codes for available values.
* `maxResults` - _optional_ - The maximum number of activities to include in the response, which is used for paging. For any response, the actual number returned might be less than the specified maxResults.
* `orderBy` - _optional_ - Specifies how to order search results.
    Possible values: best, recent.
* `pageToken` - _optional_ - The continuation token, which is used to page through large result sets. To get the next page of results, set this parameter to the value of "nextPageToken" from the previous response. This token can be of any length.
* `query` - _required_ - Full-text search query string.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Get an activity.

*Tags:* `activities`

#### Input Parameters
* `activityId` - _required_ - The ID of the activity to get.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### List all of the comments for an activity.

*Tags:* `comments`

#### Input Parameters
* `activityId` - _required_ - The ID of the activity to get comments for.
* `maxResults` - _optional_ - The maximum number of comments to include in the response, which is used for paging. For any response, the actual number returned might be less than the specified maxResults.
* `pageToken` - _optional_ - The continuation token, which is used to page through large result sets. To get the next page of results, set this parameter to the value of "nextPageToken" from the previous response.
* `sortOrder` - _optional_ - The order in which to sort the list of comments.
    Possible values: ascending, descending.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### List all of the people in the specified collection for a particular activity.

*Tags:* `people`

#### Input Parameters
* `activityId` - _required_ - The ID of the activity to get the list of people for.
* `collection` - _required_ - The collection of people to list.
    Possible values: plusoners, resharers.
* `maxResults` - _optional_ - The maximum number of people to include in the response, which is used for paging. For any response, the actual number returned might be less than the specified maxResults.
* `pageToken` - _optional_ - The continuation token, which is used to page through large result sets. To get the next page of results, set this parameter to the value of "nextPageToken" from the previous response.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Get a comment.

*Tags:* `comments`

#### Input Parameters
* `commentId` - _required_ - The ID of the comment to get.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Search all public profiles.

*Tags:* `people`

#### Input Parameters
* `language` - _optional_ - Specify the preferred language to search with. See search language codes for available values.
* `maxResults` - _optional_ - The maximum number of people to include in the response, which is used for paging. For any response, the actual number returned might be less than the specified maxResults.
* `pageToken` - _optional_ - The continuation token, which is used to page through large result sets. To get the next page of results, set this parameter to the value of "nextPageToken" from the previous response. This token can be of any length.
* `query` - _required_ - Specify a query string for full text search of public text in all profiles.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Get a person's profile. If your app uses scope https://www.googleapis.com/auth/plus.login, this method is guaranteed to return ageRange and language.

*Tags:* `people`

#### Input Parameters
* `userId` - _required_ - The ID of the person to get the profile for. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### List all of the activities in the specified collection for a particular user.

*Tags:* `activities`

#### Input Parameters
* `collection` - _required_ - The collection of activities to list.
    Possible values: public.
* `maxResults` - _optional_ - The maximum number of activities to include in the response, which is used for paging. For any response, the actual number returned might be less than the specified maxResults.
* `pageToken` - _optional_ - The continuation token, which is used to page through large result sets. To get the next page of results, set this parameter to the value of "nextPageToken" from the previous response.
* `userId` - _required_ - The ID of the user to get activities for. The special value "me" can be used to indicate the authenticated user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### List all of the people in the specified collection.

*Tags:* `people`

#### Input Parameters
* `collection` - _required_ - The collection of people to list.
    Possible values: connected, visible.
* `maxResults` - _optional_ - The maximum number of people to include in the response, which is used for paging. For any response, the actual number returned might be less than the specified maxResults.
* `orderBy` - _optional_ - The order to return people in.
    Possible values: alphabetical, best.
* `pageToken` - _optional_ - The continuation token, which is used to page through large result sets. To get the next page of results, set this parameter to the value of "nextPageToken" from the previous response.
* `userId` - _required_ - Get the collection of people for the person identified. Use "me" to indicate the authenticated user.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-plus-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
