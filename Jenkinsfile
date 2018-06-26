node {
    checkout([
        $class: 'GitSCM',
        userRemoteConfigs: [
            [
                url: scm.getUserRemoteConfigs()[0].getUrl()
            ]
        ],
        branches: [
            [
                name: "master"
            ]
        ],
        doGenerateSubmoduleConfigurations: false,
        extensions: [
            [
                $class: 'PathRestriction',
                includedRegions: "test/**"
            ]
        ]
    ])
    
    sh "ls -l"
    echo "done"
}
