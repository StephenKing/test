node {
    checkout([
        $class: 'GitSCM',
        userRemoteConfigs: [
            [
                url: scm.url
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
