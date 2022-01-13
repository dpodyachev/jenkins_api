# jenkins_api
requests

<b>jobs</b>

jenkins_url + /api/json?tree=jobs[name,color]


<b>builds</b>

jenkins_url + /job/${job_name}/api/json?tree=builds[number,status,timestamp,id,result]


<b>last build</b>

    all build info:

jenkins_url + /job/${job_name}/lastBuild/api/json

    build progress:

jenkins_url + /job/${job_name}/lastBuild/api/json?tree=result,timestamp,estimatedDuration

timestamp = start time

estimatedDuration = duration
