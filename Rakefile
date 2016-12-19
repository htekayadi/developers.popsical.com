require 'json'
require 'yaml'

desc "change yml to json"
task :jsonify do
  File.open("api.json", "w") do |f|
    f.write(YAML.load_file('api.yml').to_json)
  end
end
