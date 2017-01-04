require 'json'
require 'yaml'

desc "change yml to json, rake gen[v1]"
task :gen, [:version] do |t, args|
  File.open("#{args[:version]}/api.json", "w") do |f|
    f.write(YAML.load_file("#{args[:version]}/api.yml").to_json)
  end
end

desc "copy v1/api.json to dist/v1"
task :cp do
  `cp v1/api.json dist/v1/api.json`
end

# TODO release to s3
# run gen[v1], gen[v2]
# copy v1/api.json to dist/v1/api.json