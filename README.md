// Octokit.js
// https://github.com/octokit/core.js#readme
const octokit = new Octokit({
  auth: 'YOUR-TOKEN'
})

await octokit.request('PUT /orgs/{org}/actions/variables/{name}/repositories/{repository_id}', {
  org: 'ORG',
  name: 'NAME',
  repository_id: 'REPOSITORY_ID',
  headers: {
    'X-GitHub-Api-Version': '2022-11-28'
  }
})
