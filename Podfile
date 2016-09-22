platform :ios, '9.0'
use_frameworks!

target 'Eureka-Swift3' do
	pod 'Eureka', :git => 'https://github.com/xmartlabs/Eureka.git', :branch => 'Swift3'
end

target 'Eureka-Swift3Tests' do
	pod 'Eureka', :git => 'https://github.com/xmartlabs/Eureka.git', :branch => 'Swift3'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
	target.build_configurations.each do |config|
	  config.build_settings['SWIFT_VERSION'] = '3.0'
	end
  end
end