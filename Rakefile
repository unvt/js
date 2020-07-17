task :default do
  sh "git clone https://github.com/mapbox/mapbox-gl-js.git"
  sh "cd mapbox-gl-js; yarn install; yarn run build-prod-min; yarn run build-css; cp dist/* ../docs"
  sh "rm -rf mapbox-gl-js"
end
