# Quicksilver-API
API gateway to Quicksilver (Message Broker) functionality.

## Endpoints

#### Users

| Endpoint               | Functionality                                                              | Message                                                                                            |
| ---------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `POST /user/register`  | [User registration](documentation/endpoints/user.md#user-registration)     | [user.registration.transactional](documentation/messages/user.registration.transactional.md)       |
| `POST /user/password`  | [User password reset](documentation/endpoints/user.md#user-password-reset) | [user.password_reset.transactional](documentation/messages/user.password_reset.transactional.md)   |


#### Campaigns

| Endpoint                    | Functionality                                                                    | Message                                                                                       |
| --------------------------- | -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `POST /campaign/signup`     | [Campaign signup](documentation/endpoints/campaign.md#campaign-signup)           | [campaign.signup.transactional](documentation/messages/campaign.signup.transactional.md)      |
| `POST /campaign/reportback` | [Campaign report back](documentation/endpoints/campaign.md#campaign-report-back) | [campaign.report_back.transactional](documentation/messages/campaign.signup.transactional.md) |

## Tests

Master build status:

[![wercker status](https://app.wercker.com/status/ee29a549f6d3b68e7b3cb101a7c9a943/s/master "wercker status")](https://app.wercker.com/project/bykey/ee29a549f6d3b68e7b3cb101a7c9a943)

Test coverage uses the following utilities:
- [Mocha](https://www.npmjs.com/package/mocha)
- [Should](https://www.npmjs.com/package/should)
- [Supertest](https://www.npmjs.com/package/supertest)

To run all of the tests defined in `/test` recursively.

```
$ npm test
```
