desc "Bootstraps the repo"
task :bootstrap do
  sh 'bundle'
  sh 'cd ExampleProject && bundle exec pod install'
end

desc "Runs the specs"
task :spec do
  sh 'xcodebuild -workspace ExampleProject/PunchUIScrollView.xcworkspace -scheme \'PunchUIScrollView\' test -sdk iphonesimulator | xcpretty -tc'
end
