# fastlane-swift-basic
A fastlane simple project using fastlane swift

mkdir fastlane-test && cd fastlane-test

git init

echo "source 'https://rubygems.org' \ngem \"fastlane\"" > Gemfile

bundle install

yes | bundle exec fastlane swift init

git add .
git commit -m "add all after init"

## ------
## source "'https://rubygems.org' \n
## gem \"fastlane\", :git => \"https://github.com/kikeenrique/fastlane.git\", :branch => \"18502\"" > Gemfile

echo "source 'https://rubygems.org' \ngemspec path: File.expand_path(\"/Users/~/Developer/tools/fastlane\")" > Gemfile
bundle install

bundle exec fastlane custom --verbose
No newline at end of file
