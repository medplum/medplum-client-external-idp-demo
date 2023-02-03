# Medplum OAuth Demo

This is a demonstration of how to use Medplum with an External Auth Provider or "Federated Identities".

This repo is similar to [medplum-oauth-demo](https://github.com/medplum/medplum-oauth-demo), except that is uses `@medplum/core` and `MedplumClient`.

It demonstrates:

- How to call the [/oauth2/authorize endpoint](https://docs.medplum.com/api/oauth/authorize) to initiate the authorization flow
- How to call the [/oauth2/token endpoint](https://docs.medplum.com/api/oauth/token) to exchange a code for an access token
- How to call the [/oauth2/userinfo endpoint](https://docs.medplum.com/api/oauth/userinfo) to retrive the current user details
- How to call the Medplum FHIR API with the access token

## Setup

Setup your account:

- [Register for a Medplum account](https://docs.medplum.com/tutorials/app/register)
- Create a `ClientApplication`
- Set the "Redirect URI" to "http://localhost:8000/"

Now you can run this demo:

```bash
npm run dev
```

Open your web browser to <http://localhost:8000/>
