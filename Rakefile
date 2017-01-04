require 'json'
require 'yaml'

desc "change yml to json, rake gen[v1]"
task :gen, [:version] do |t, args|
  File.open("#{args[:version]}/api.json", "w") do |f|
    f.write(YAML.load_file("#{args[:version]}/api.yml").to_json)
  end
end
