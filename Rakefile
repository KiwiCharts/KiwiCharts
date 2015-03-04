require 'xcjobs'

def destinations
  [ 'name=iPhone 6,OS=8.2' ]
end

XCJobs::Test.new('test:ios') do |t|
  t.project = 'KiwiCharts'
  t.scheme = 'KiwiCharts'
  t.configuration = 'Debug'
  t.build_dir = 'build'
  destinations.each do |destination|
    t.add_destination(destination)
  end
  t.formatter = 'xcpretty -c'
end
