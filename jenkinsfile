pipeline{
	agent any
		stage('One') {
			steps {
				echo 'Line in stage PhOne steps'
				}
				}
		stage('Two') {
			steps {
				echo 'Line in stage PhTwo steps'
				input(Go ahead?')
				}
				}
		stage('Three') {
			when {
				not {
					branch "master"
				}
			     }
			steps {
				echo 'Line in stage PhThree steps: Hello'
				}
			}
}