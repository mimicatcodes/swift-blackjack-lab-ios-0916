# Uncomment this line to define a global platform for your project
# platform :ios, '9.0'

target 'swift-blackjack-lab' do
  # Comment this line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for swift-blackjack-lab
  def testing_pods
    pod 'Nimble', git: 'https://github.com/Quick/Nimble.git'
    pod 'Quick', git: 'https://github.com/Quick/Quick.git'
    end

  target 'swift-blackjack-labTests' do
    inherit! :search_paths
    # Pods for testing
    testing_pods
  end

end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '3.0'
        end
    end
end
