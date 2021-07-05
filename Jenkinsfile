pipeline {
	agent any
	stages {
        stage('Pre-Build Email') {
		git branch: 'main', credentialsId: 'Github', url: 'https://github.com/Pravin861/Shilpastock.git'
		}
 	stage('Exeute shell') {
                steps {

                   sshPublisher(publishers: [sshPublisherDesc(configName: '', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: 'sudo sh /root/script/autheticationservice.sh', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '/', remoteDirectorySDF: false, removePrefix: '', sourceFiles: '')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
                }
		}
            }
}
