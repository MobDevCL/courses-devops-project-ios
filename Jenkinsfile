node('ios') {
	stage 'Checkout and Setup'
		checkout scm
		sh 'cd fastlane'
	stage 'Test'
		sh 'fastlane test'
	stage 'Build'
		def build_number = env.BUILD_NUMBER
		sh "fastlane build build_number:${build_number}"
}
