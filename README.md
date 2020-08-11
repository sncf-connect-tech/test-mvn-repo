Attempting to reproduce a potential issue with Renovate `ignoreDeps` setting:

Testing with Docker for Windows:

    set GITHUB_COM_TOKEN=...
    set VERSION=latest
    docker run -e LOG_LEVEL=debug -e RENOVATE_TOKEN=%GITHUB_COM_TOKEN% renovate/renovate:%VERSION% --print-config true --autodiscover false voyages-sncf-technologies/test-mvn-repo
