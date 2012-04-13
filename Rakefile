require 'rubygems'
require "active_support"

desc "new post"
task :post do
  ext = ENV['JEKYLL_EXT'] || "markdown"
  unless title = ENV['TITLE']
    puts "use rake post TITLE='the post title'"
    exit(1)
  end
  post_title = "#{Time.now.to_s}-#{title.downcase.gsub(/[^\w]+/, '-')}"
  post_file = File.dirname(__FILE__) + "/_posts/#{post_title}.#{ext}"
  File.open(post_file, "w") do |f|
    f << <<-EOS.gsub(/^    /, '')
    ---
    layout: post
    title: #{title}
    ---
    
    EOS
  end
end


namespace :jekyll do
  
  desc 'clean the _site folder'
  task :clean do
  system "rm -rf _site"
  end
  
end

namespace :pygment do 
  
  desc 'clean pygmentize files' 
    task :rmv   do
    system "rm -rf css/syntax.css"
  end
  
  desc 'highlight and make the css' 
    task :make  =>  [:rmv]  do
    system "pygmentize -S monokai -f html -a .highlight > css/syntax.css"
  end
  
end