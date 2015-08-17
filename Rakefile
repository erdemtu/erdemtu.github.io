require 'time'

# Get and parse the date
DATE = Time.now.strftime("%Y-%m-%d")
POST_TIME = Time.now.strftime("%Y-%m-%d %H:%M:%S %z")

desc 'create a new post'
task :post, :title do |t, args|
    title = args[:title]
    slug = "#{DATE}-#{title.downcase.gsub(/[^\w]+/, '-')}"

    file = File.join(
        File.dirname(__FILE__),
        '_posts',
        slug + '.md'
    )

    File.open(file, "w") do |f|
        f << <<-EOS.gsub(/^        /, '')
        ---
        layout: post
        title:  "#{title}"
        date:   #{POST_TIME}
        categories:
        ---

        EOS
    end

    system ("#{ENV['EDITOR']} #{file}")
end

desc 'Run serve'
task :serve do
  sh 'bundle exec jekyll serve'
end

desc 'Run build'
task :build do
  sh 'bundle exec jekyll build'
end
