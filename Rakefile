require 'json'
require 'yaml'

desc "change yml to json, rake gen[v1]"
task :gen, [:version] do |t, args|
  version = args[:version] || "v1"
  File.open("#{version}/api.json", "w") do |f|
    f.write(YAML.load_file("#{version}/api.yml").to_json)
  end
end

desc "copy v1/api.json to dist/v1"
task :cp do
  `cp v1/api.json dist/v1/api.json`
end

desc "build static assets"
task build: [:gen, :cp]

# TODO release to s3
# run gen[v1], gen[v2]
# copy v1/api.json to dist/v1/api.json