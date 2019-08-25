node('maven') {
    stage('git') {
			git 'https://github.com/wakaleo/game-of-life.git'
				}
				
	stage('build'){
				sh label: '', script: 'mvn package'
				}
	
	
	stage('Archive') {
    // some block
				archive 'target/*.war'
				junit 'target/surefire-reports/*.xml'
				}
}
